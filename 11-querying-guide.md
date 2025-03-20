# 11 Redshift Querying Guide

This document serves as an introduction to generating proficient Amazon Redshift queries. This is a generalized document meaning you will need to replace “schema_name” and “table_name” with the appropriate schema and table names used for your project.

**Note**: All data is stored under schemas in the projects database.

## Topics
- [Data Access](#data-access)
- [Using DBeaver to access a database](#using-dbeaver-to-access-a-database)
  - [Creating tables in a PR or TR schema in Dbeaver](#creating-tables-in-a-pr-or-tr-schema-in-dbeaver)
- [Connecting to a database through a statistical program](#connecting-to-a-database-through-a-statistical-program)
  - [Connecting to a database using SAS](#connecting-to-a-database-using-sas)
  - [Connecting to a database using R](#connecting-to-a-database-using-r)
  - [Connecting to a database using Python](#connecting-to-a-database-using-python)
  - [Connecting to a database using Stata](#connecting-to-a-database-using-stata)
- [Redshift Query Guidelines for Researchers](#redshift-query-guidelines-for-researchers)
## Data access
If you are approved to access data that are stored in a database, the data are housed in Redshift. To access those data, you will have to log in to Redshift within your workspace.

You need to replace the “user.name.project” with your **project workspace username**. The **project workspace username** is your user folder name in the U:/ drive:

![Image of Project-Based User Name](https://coleridge-initiative.github.io/adrf_onboarding_handbook/images/ap1.png)

**Note**: You will need to enter your specific user name when logging into Redshift. The password needed to access Redshift is the second password entered when logging into the ADRF as shown in the screen below: 
![Image of Password Entry](https://coleridge-initiative.github.io/adrf_onboarding_handbook/images/ap2.png)

## Using DBeaver to access a database
To establish a connection to Redshift in DBeaver, first open DBeaver by clicking on the DBeaver icon located on the ADRF desktop and then double click on the server you wish to connect to. **Note**: All data is stored under schemas in the projects database.

In the example below, we will connect to **Redshift11_projects**. After double clicking on Reshift11_projects, a window will appear asking for your **Username** and **Password**. 
- In Username, enter **"adrf\\"** followed by your **project workspace username** 
- In Password, enter the password associated with your project workspace username
![Complete the Username and Password fields](https://coleridge-initiative.github.io/adrf_onboarding_handbook/images/ap3.png)

After completing the Username and Password fields, click **OK**. You will now have access to your data stored on the Redshift11_projects server.

**Note**: Please make sure to enter **"adrf\\"** before your project workspace username in the **Username** field. If you do not enter "adrf\", or accidently include a "/" instead of a "\\", you will not be able to connect to Redshift. **If you are having trouble connecting, an incorrect entry in Username is most likely the culprit.**

### Creating tables in a PR or TR schema in Dbeaver
When users create tables in their PR (Research Project) or TR (Training Project) schema, the table is initially permissioned to the user only. This is analogous to creating a document or file in your U drive: Only you have access to the newly created table.

If you want to allow all individuals in your project workspace to access the table in the PR/TR schema, you will need to grant permission to the table to the rest of the users who have access to the PR or TR schema.

You can do this by running the following code:
`GRANT SELECT, UPDATE, DELETE, INSERT ON TABLE schema_name.table_name TO group db_xxxxxx_rw;`

**Note**: Note: In the above code example replace schma_name with the pr_ or tr_ schema assigned to your workspace and replace table_name with the name of the table on which you want to grant access. Also, in the group name `db_xxxxxx_rw`, replace `xxxxxx` with your project code. This is the last 6 characters in your project based user name. This will start with either a T or a P.

If you want to allow **only a single user** on your project to access the table, you will need to grant permission to that user. You can do this by running the following code:

`GRANT SELECT, UPDATE, DELETE, INSERT ON TABLE schema_name.table_name to "IAM:first_name.last_name.project_code";`

**Note**: In the above code example replace schma_name with the pr_ or tr_ schema assigned to your workspace and replace table_name with the name of the table on which you want to grant access. Also, in `"IAM:first_name.last_name.project_code"` update `first_name.last_name.project_code` with the user name to whom you want to grant access to.

If you have any questions, please reach out to us at [support@coleridgeinitiative.org](mailto:support@coleridgeinitiative.org)

## Connecting to a database through a statistical program

When connecting to the database using an ODBC connection, you need to use one of the following DSNs:

- `Redshift01_projects_DSN`
- `Redshift11_projects_DSN`

In the code examples below, the default DSN is `Redshift01_projects_DSN`.

**Topics:**
- [Connecting to a database using SAS](#connecting-to-a-database-using-sas)
- [Connecting to a database using R](#connecting-to-a-database-using-r)
- [Connecting to a database using Python](#connecting-to-a-database-using-python)
- [Connecting to a database using Stata](#connecting-to-a-database-using-stata)

### Connecting to a database using SAS
Use the following code to connect to a databse using SAS:

``` sas
proc sql;
connect to odbc as my con
(datasrc=Redshift01_projects_DSN user=adrf\user.name.project password=password);
select * from connection to mycon
(select * form projects.schema.table);
disconnect from mycon;
quit;
```

### Connecting to a database using R

- [Recommended method for connecting to a database using R](#recommend-method-for-connecting-to-a-database-using-r)
- [Using Renviron file to connect to a database using R](#using-renviron-file-to-connect-to-a-database-using-r)
- [Best practices for loading large amounts of data in R](#best-practices-for-loading-large-amounts-of-data-in-r)

#### Recommended method for connecting to a database using R

**Note**: To use this method, you may need to install the packages RJDBC and rstudioapi first.

``` r
library(RJDBC)

# Create username
dbusr=paste("ADRF\\", Sys.getenv("USERNAME"), sep= '')                                                                                

# Database URL
url <- paste0("jdbc:redshift:iam://adrf-redshift01.cdy8ch2udktk.us-gov-west-1.redshift.amazonaws.com:5439/projects;",
              "loginToRp=urn:amazon:webservices:govcloud;",
              "ssl=true;",
              "AutoCreate=true;",
              "idp_host=adfs.adrf.net;",
              "idp_port=443;",
              "ssl_insecure=true;",
              "plugin_name=com.amazon.redshift.plugin.AdfsCredentialsProvider")

# Redshift JDBC Driver Setting
driver <- JDBC("com.amazon.redshift.jdbc42.Driver",
               classPath = "C:\\drivers\\redshift_withsdk\\redshift-jdbc42-2.1.0.12\\redshift-jdbc42-2.1.0.12.jar",
               identifier.quote="`")
con <- dbConnect(driver, url, dbusr, rstudioapi::askForPassword())
```

#### Using Renviron file to connect to a database using R

``` r
library(RJDBC)
dbusr=Sys.getenv("DBUSER")                                                                    dbpswd=Sys.getenv("DBPASSWD")

# Database URL
url <- paste0("jdbc:redshift:iam://adrf-redshift01.cdy8ch2udktk.us-gov-west-1.redshift.amazonaws.com:5439/projects;",
"loginToRp=urn:amazon:webservices:govcloud;",
"ssl=true;",
"AutoCreate=true;",
"idp_host=adfs.adrf.net;",
"idp_port=443;",
"ssl_insecure=true;",
"plugin_name=com.amazon.redshift.plugin.AdfsCredentialsProvider")

# Redshift JDBC Driver Setting
driver <- JDBC("com.amazon.redshift.jdbc42.Driver",
classPath = "C:\\drivers\\redshift_withsdk\\redshift-jdbc42-2.1.0.12\\redshift-jdbc42-2.1.0.12.jar",
identifier.quote="`")
conn <- dbConnect(driver, url, dbusr, dbpswd)
```
**Note**: For the above code to work, please create a file name .Renviron in your user folder (user folder is something like i.e. `u:\John.doe.p00002`) And `.Renviron` file should contain the following:

``` r
DBUSER='adrf\John.doe.p00002'
DBPASSWD='xxxxxxxxxxxx'
```

_**PLEASE** replace `user id` and `password` with your project workspace specific user id and password. 

This will ensure you don’t have your id and password in R code and then you can easily share your R code with others without sharing your ID and password._

#### Best practices for loading large amounts of data in R

##### SQL Basics with R Programming
To ensure R can efficiently manage large amounts of data, please add the following lines of code to your R script before any packages are loaded:

``` r
options(java.parameters = c("-XX:+UseConcMarkSweepGC", "-Xmx8192m"))
gc()
```

##### Best practices for writing tables to Redshift

When writing an R data frame to Redshift use the following code as an example:

``` r
# Note: replace the table_name with the name of the data frame you wish to write to Redshift

DBI::dbWriteTable(conn = conn, #name of the connection 
name = "schema_name.table_name", #name of table to save df to 
value = df_name, #name of df to write to Redshift 
overwrite = TRUE) #if you want to overwrite a current table, otherwise FALSE

qry <- "GRANT SELECT ON TABLE schema.table_name TO group <group_name>;"
dbSendUpdate(conn,qry)
```

### Connecting to a database using Python
``` python
import pyodbc
import pandas as pd
cnxn = pyodbc.connect('DSN=Redshift01_projects_DSN; UID=adrf\user.name.project; PWD=password')
df = pd.read_sql("SELECT * FROM projects.schema_name.table_name", cnxn)
```

### Connecting to a database using Stata
``` stata
odbc load, exec("select * from PATH_TO_TABLE") clear dsn("Redshift11_projects_DSN") user("adrf\user.name.project") password("password")
```

## Redshift Query Guidelines for Researchers

_Developing your query_. Here’s an example workflow to follow when developing a query.

1. Study the column and table metadata, which is accessible via the table definition. Each table definition can be displayed by clicking on the [+] next the table name.
2. To get a feel for a table’s values, `SELECT * from` the tables you’re working with and LIMIT your results (Keep the LIMIT applied as you refine your columns) or use (e.g., `select * from [table name] LIMIT 1000`)
3. Narrow down the columns to the minimal set required to answer your question.
4. Apply any filters to those columns.
5. If you need to aggregate data, aggregate a small number of rows
6. Once you have a query returning the results you need, look for sections of the query to save as a Common Table Expression (CTE) to encapsulate that logic.
