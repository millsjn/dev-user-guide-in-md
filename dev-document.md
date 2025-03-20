# ADRF User Guide

_A detailed guide to help users navigate and use the **Coleridge Initiative's** Administrative Data Research Facility (ADRF) effectively._

_Last Modified:_

---

## Table of Contents
1. [Introduction](#1-introduction)  
2. [Obtaining ADRF Access](#2-obtaining-adrf-access)  
3. [Onboarding Modules and Security Training](#3-onboarding-modules-and-security-training)
4. [Do's and Don'ts for Discussing Data Hosted in the ADRF](#4-dos-and-donts-for-discussing-data-hosted-in-the-adrf)  
5. [How to Access and Use Your Project Workspace](#5-how-to-access-and-use-your-project-workspace)  
6. [Troubleshooting](#troubleshooting)  
7. [FAQ](#faq)

---

## 1. Introduction

Welcome to the [Coleridge Initiative’s](https://coleridgeinitiative.org/) Administrative Data Research Facility, or "**ADRF**" user guide. This is a living document intended to show new ADRF users how to use the platform for common tasks.

### About the Coleridge Initiative
The Coleridge Initiative’s mission is to improve the access, usability, and impact of data for public policy by fostering collaboration between government agencies, researchers, and other stakeholders. It aims to create a data ecosystem where government data can be more effectively used to inform evidence-based decision-making, policy development, and research.

### About the Administrative Data Research Facility
The Administrative Data Research Facility (ADRF) is a platform provided by the Coleridge Initiative that enables researchers to access and analyze administrative data from government agencies securely and efficiently. It offers a secure computing environment where researchers can work with sensitive data while ensuring privacy and confidentiality. The ADRF provides tools and infrastructure for data integration, analysis, and visualization, allowing researchers to conduct rigorous and reproducible studies using large-scale administrative datasets. By facilitating access to valuable data resources and promoting collaboration between researchers, government agencies, and other stakeholders, the ADRF supports evidence-based policymaking and advances research in fields such as public health, education, labor economics, and social policy.

### The Five Safes Security Framework
The ADRF follows the Five Safes Framework, a data management framework commonly used in government agencies, to ensure the safe use of sensitive and confidential data assets. It considers five dimensions in making data-related safety and security decisions: Safe Projects, Safe People, Safe Settings, Safe Data, and Safe Exports.
- **Safe Projects** - The ADRF contains only agency approved projects that have been proposed and agreed upon by project and dataset stewards. Only approved projects are housed within ADRF, only approved individuals are granted access to a given project, and project environments are kept separated from each other. These approved projects require signed agreements and only approved users can access the project workspaces within the platform.
- **Safe People** - Only approved researchers are permitted to access project workspaces and related resources. Each individual with approved access must complete security training, agree to the ADRF terms of use, and sign relevant data use agreements. Individuals must authenticate to gain access to the remote platform and all ADRF activity is monitored. 
- **Safe Settings** - The ADRF is designed to provide secure methods of data transfer for agency micro-data, specifically data that includes Personally Identifiable Information. Only agency identified and authorized personnel are invited to perform data transfers.
- **Safe Data** - Before transmission to ADRF, all data with personally identifiable or other sensitive information is hashed, and an online data stewardship application provides data stewards with information on who is accessing their data, how it is being accessed, what projects employ it, the characteristics of each data asset, and the status of user agreements. 
- **Safe Exports** - Users are prevented from unauthorized removal of any information within the secure environment.

---

## 2. Obtaining ADRF Access

### Topics
- [Account Setup](#account-setup)
- [Obtaining ADRF Access](#obtaining-adrf-access)
- [Account Registration and Onboarding](#account-registration-and-onboarding-tasks)
- [More Information](#more-information)

### Account Setup
- **Agency-affiliated researcher**. If you are an agency-affiliated researcher, your agency will set up an ADRF account for you.
- **Individual part of a training program**. If you are part of a [training program](https://coleridgeinitiative.org/applied-data-analytics-training-programs), the Coleridge Initiative team will create an account for you once you have been accepted into the program.

### Obtaining ADRF Access
- **Agency-affiliated researcher**. If you are an agency-affiliated researcher using an agency-sponsored account, you will be granted ADRF access once you complete your onboarding tasks and required data access agreements. If you are a self-paying agency-affiliated researcher, your ADRF access is conditional on receipt of payment. If your institution of Office of Sponsored Programs will be submitting payment on your behalf, please be aware of potential access delays. Whenever possible, the Coleridge Initiative advises paying with a personal credit card or institutional payment card and using the generated invoice to request reimbursement.
- **Individual part of a training program**. If you are part of a training program, you will be granted ADRF access once you complete your onboarding tasks and required data access agreements.

### Account Registration and Onboarding Tasks
- You will receive an email invitation to activate your account. The email will come from [http://okta.com](http://okta.com), so please make sure that it doesn’t get caught in your email spam filter. Follow the steps outlined in the email to set up your password and your multi-factor authentication preferences. Clink on the link below to watch a video walking through the steps.
- After activating your account, you will be logged in to the ADRF Applications page. Proceed to the **Management Portal** by clicking on the icon.
- In the **Management Portal**, you will notice a “Onboarding Tasks” section within “Admin Tasks” with a number of items you will need to complete before you can gain access to the project space. Refer to the next section for details about the onboarding process.

### More Information
If you have any questions, please contact [support@coleridgeinitiative.org](mailto:support@coleridgeinitiative.org).

---

## 3. Onboarding Modules and Security Training

### Topics
- [Management Portal](#management-portal)
- [Signing the ADRF Terms of Use Agreement](#signing-the-adrf-terms-of-use-agreement)
- [Watching the Security Training Video](#watching-the-security-training-video)
- [Complete the Security Training Quiz](#complete-the-security-training-quiz)

### Management Portal
The Management Portal web-based application is positioned primarily as the management and monitoring console for project and data stewards. It provides detailed insight on project configurations, user activity, user onboarding status, and overall cost of a project on the ADRF. We focus on four primary pillars of information a Project/Data Steward most often focuses on:
- **People** – Who are the members of projects, how often do they use the ADRF, what exports have they requested and their status, estimated cost per person/project for current month and for the project since inception, and detailed usage metrics.
- **Projects** – Details of project start/end dates, abstract description, number of members onboarded and pending, and resources the project has access to (i.e. datasets, etc).
- **Datasets** – Description of the dataset, location on the ADRF (database or file system), size, name of the data steward(s), and the link to Enterprise Data Catalog (Informatica) describing the dataset and metadata.
- **Agreements** – What agreements are related to these projects, indication of each member’s signing status, members pending signature, and term (dates) covered by the agreement(s).

As mentioned, the Management Portal application will track your ADRF usage. The protal will also consolidate your ADRF Terms of Use, Security Training Quiz, and Security Training Video into one place. In order to complete ADRF onboarding, all three of the mentioned tasks are to be completed by the user (researcher). To access the Management Portal, log in using your credentials at https://adrf.okta.com and click on the ADRF Management Portal icon:

<p align="center">
  <img src="https://coleridge-initiative.github.io/adrf_onboarding_handbook/images/mp_icon.png" alt="ADRF Management Portal Icon">
</p>

Once inside the Management Portal, you have access to your personal workspace sessions statistics along with admin tasks such as the three onboarding tasks and password management. See the example below:
<p align="center">
  <img src="https://coleridge-initiative.github.io/adrf_onboarding_handbook/images/mp_home.png" alt="Management Portal Insights Page">
</p>

### Accessing the Onboarding Tasks
To gain access to your ADRF project workspace, you must first complete 3 required ADRF onboarding tasks: 
1. **Signing the ADRF Terms of Use agreement**. Users must comply with the Terms of Use when working in the ADRF. The Agreement covers rules of behavior within ADRF and guidelines for discussing ADRF content prior to passing disclosure review. It asks users to agree to a series of principles governing dataset use, behavior, and data export procedures, and to acknowledge the consequences of violating the Terms.
2. **Completing security awareness training**. Users will get access to a security awareness video and should confirm that they have reviewed the video. The video covers security content that is then assessed during the security awareness quiz.
3. **Passing the security awareness quiz**. The security awareness quiz consists of a set of 6 questions. Users must achieve a score 5 out of 6 to pass the quiz. Unsuccessful users can retake the quiz to achieve a passing score.


Follow the steps below to access the **ADRF Onboarding Tasks**:
1. Log in to the Management Portal

2. Click on **“Admin Tasks”** in the left navigation menu.

<p align="left">
  <img src=https://coleridge-initiative.github.io/adrf_onboarding_handbook/images/admin_tasks.png alt="Click on 'Admin Tasks' in the left navigation menu">
</p>

3. Click on **“Complete Onboarding”**.

<p align="left">
  <img src=https://coleridge-initiative.github.io/adrf_onboarding_handbook/images/complete_ob.png alt="Click on 'Complete Onboarding'">
</p>

4. This will load the **Onboarding Tasks window**.

<p align="left">
  <img src=https://coleridge-initiative.github.io/adrf_onboarding_handbook/images/ob_tasks_window.png alt="Onboarding Tasks window">
</p>

5. Click on each individual task to complete it.

### Signing the ADRF Terms of Use Agreement

The Terms of Use need to be completed before you are given access to the data and project space inside the ADRF. To complete ADRF Terms of Use, complete the following steps:

1. Click on the **“Terms of Use”** tile.

<p align="left">
  <img src=https://coleridge-initiative.github.io/adrf_onboarding_handbook/images/terms_of_use_tile.png alt="Terms of Use Tile">
</p>

3. Click on **“Sign with DocuSign”**

<p align="left">
  <img src=https://coleridge-initiative.github.io/adrf_onboarding_handbook/images/sign_docuSign.png alt="Sign with DocuSign">
</p>

4. You will then be redirected to the DocuSign signing page. **Click “Continue”** on the upper right corner.

<p align="left">
  <img src=https://coleridge-initiative.github.io/adrf_onboarding_handbook/images/docusign_continue.png alt="Click Continue">
</p>

5. Click **“Start”** to begin.

<p align="left">
  <img src=https://coleridge-initiative.github.io/adrf_onboarding_handbook/images/start.png alt="Click Start to begin">
</p>

6. If you have already configured a signature, click on the **yellow “Sign” button** to apply it. Otherwise, follow the prompts to configure your electronic signature.

<p align="left">
  <img src=https://coleridge-initiative.github.io/adrf_onboarding_handbook/images/sign.png alt="Click the yellow Sign button to apply your signature">
</p>

7. Once the signature is applied, click **“Finish”**.

<p align="left">
  <img src=https://coleridge-initiative.github.io/adrf_onboarding_handbook/images/finish.png alt="Click Finish">
</p>

You will then be redirected back to the management portal. And the “Terms of Use” task will be marked as completed.

### Watching the Security Training Video

The Security Training Video needs to be completed as well. To complete the training, complete the following steps:

1. Click on the **“Security Training Video”** tile to load the player and then click play.
2. Once you have watched the video in its entirety, click on the **“Mark as Complete”** button to complete the task. _Note: the “MARK AS COMPLETE” button will not be enabled until at least 5 minutes have passed since the start of the video._
3. Click on the **back arrow** in the upper right corner to return to the main tasks panel.
4. The training video section will now be **marked as completed**.

### Complete the Security Training Quiz

The Security Training Quiz needs to be completed after the Security Training Video. To complete the training, complete the following steps:

1. Click on the **“Security Quiz”** tile to load the quiz.

<p align="left">
  <img src=https://coleridge-initiative.github.io/adrf_onboarding_handbook/images/st_quiz_tile.png alt="Click on the Security Quiz tile">
</p>

2. Answer the questions and click on the **“SUBMIT RESPONSE”** button. You must answer at least four of the questions correctly to complete this task.

<p align="left">
  <img src=https://coleridge-initiative.github.io/adrf_onboarding_handbook/images/submit_response.png alt="Click on the Submit Response button">
</p>

3. You will be automatically redirected to the main task panel once the questionnaire has been successfully completed. And the **“Security Quiz”** will be marked as completed.
<p align="left">
  <img src=https://coleridge-initiative.github.io/adrf_onboarding_handbook/images/security_quiz_complete.png alt="Security Quiz Complete">
</p>

---

## 4. Do's and Don'ts for Discussing Data Hosted in the ADRF

You **must protect the confidential data** that is hosted inside the ADRF in communicating with your teammates. The general rule is that you should never take any exact number out of the ADRF. This means you should never write down or share any number by text, screenshot, or share an image even with a team-mate. The rules have become more complicated now that everything is online, because even though your teammates are “safe people”, and Zoom conversations are password protected and encrypted, we’d rather err on the side of caution when sharing information over Zoom.

To ensure **safe outputs**, the Coleridge Initiative works with an agency’s Data Steward to develop rigorous export review requirements catered to the specific needs of the partner agency. While you should make sure to acquaint yourself with the specific export rules associated with the confidential data you have been approved to access, **cheat sheet provided below** summarizes some of the rules that apply to discussing data before it has been exported from the ADRF and passed the ADRF team’s disclosure review. 

If you are unsure about a specific situation, please ask reach out to the Coleridge Support Team at [support@coleridgeinitiative.org](mailto:support@coleridgeinitiative.org).

### Exact Numbers
Do not describe a statistic in exact numbers. If you would like to communicate these values while not in person, you can have a private discussion via the projects drive inside the ADRF.

**Example**: If an average within a specific group was 5,000, you would need to convey this average on the projects drive.

### Comparing Values
When comparing values, you are permitted to say that one value is more than, less than, or about the same as another. However, you cannot refer to the exact difference between the two numbers.

In practice, you can use pluses and minuses to convey differences between values for data that has not been exported from the ADRF.

**Example**: “The mean for Group A was roughly the same as the mean for Group B, but these values were both greater than that of Group C.”

### Percentages/Proportions
Percentages and proportions also cannot be directly mentioned. Instead, you can refer to the percentage/proportion within 25%.

**Example**: If a proportion was 30%, you could say “The proportion is about 25%” or “The proportion is between 25% and 50%.”

---

## 5. How to Access and Use Your Project Workspace
A **project workspace** is a secure, isolated virtual environment in the ADRF within which an approved set of users can access a defined number of agency datasets. The project workspace is designed to allow approved researchers to access, analyze, and manipulate specific datasets relevant to their approved projects while maintaining strict data confidentiality and integrity. 

Project workspace in the ADRF are isolated from each other. Even if a person is granted access to two project workspaces, the user can not access or copy files from one into the other. This is important because the two project workspaces might have access to different datasets. 

### Logging into and Logging out of the ADRF
This video linked below runs through the necessary steps for logging into and logging out of the ADRF.

To watch the video, **right-click the image below** and choose **"Open link in new tab"** (by right-cicking, you will avoid leaving this page).

[![Logging into ADRF](https://img.youtube.com/vi/_-AE_iOyF9w/0.jpg)](https://www.youtube.com/watch?v=_-AE_iOyF9w)

### Virtual Desktop Environment
#### What is a VDE?
A **virtual desktop environment (VDE)** allows you to interact with a remote system as if it were your own personal computer. The majority of your standard desktop functions are available, but the programs, data, and permissions are all controlled by the remote administrator (Coleridge Initiative). Thus, you will be working in a familiar environment while accessing protected data, programs, and systems that would otherwise be difficult to distribute. The ADRF uses a standard Windows environment (Windows Server) and provides a variety of software packages to conduct your analysis. For more on Windows capabilities, see the section on Windows Settings.

<p align="left">
  <img src=https://coleridge-initiative.github.io/adrf_onboarding_handbook/images/use1.png alt="Virtual Desktop Environment">
</p>

#### Temporary Nature of the Environment

While the environment is similar to that on your home computer (for Windows users), there are a handful of key differences. The first is that the environment is temporary in nature. This means that if you are not using it for a prolonged period of time (default is four hours but can vary by project), running programs will stop running and the information stored in temporary locations will be deleted. You will receive on on-screen message before any sessions are terminated. For more on safe, non-temporary storage locations in the ADRF, see the section on Storing Analytic Results.

Given the temporary nature of the ADRF, it is crucial to make sure that your work is saved—and saved in an appropriate location. Once this is complete and you are finished working, make sure that you log out of the ADRF instead of closing the window. To do this, click the rightmost icon on the top taskbar to open up the dropdown menu and select End Session. You will be prompted to double-check that your work is saved prior to ending your session and confirm that you want to end your session.

#### Modifying the Environment
##### Establishing Personal Folders
Establishing your own personal folders is one of the simplest, yet most important, steps to take when setting up your environment. As we note in the section on Storing Analytic Results, the two possible places to store your analytic results or files are in either the U: drive or the P: drive.

You will find your personal folder in the U: drive. The folder name will include your Firstname and Lastname, and may additionally include your project workspace number. This is a personal workspace that only you can access in the ADRF.

##### The U: Drive and the P: Drive
The U: drive is your user drive; it’s where you will store any files you are working on. Only the user will have access to the U: drive. For example, if user A wants to share information with user B who is on the same project, user A will need to save files to a P: drive folder and not folders in their U: drive since user B will not be able to access user A’s U: drive.

The P: drive is the project drive, which will be used to house project-specific folders. Thus, you and other collaborators on the same project will be able to save files to project drive folders.

Both the U: drive and P: drive have defined resource limitations of 150GB. When the workspace exceeds these limits, users will not be able to create new files or save data. The ADRF will not alert users when they approach on 150GB used. Users can check their current usage by right clicking on the user folder and clicking on properties.

##### Other Modifications
The top taskbar contains shortcuts to the command prompt, multiple desktop windows, a temporary folder, settings, full-screen view, and toggling multiple monitors.
<p align="left">
  <img src=https://coleridge-initiative.github.io/adrf_onboarding_handbook/images/use2.png alt="Taskbar">
</p>

#### Windows Settings
Your desktop will look familiar if you are a Windows user. You will have icons for quick access to programs or browsers on your desktop. The windows icon on the bottom left side of the screen will open up a menu of programs, folders, and other tools, much as you would see on your own desktop. You will have access to PowerShell and several customization settings (e.g., remove bottom taskbar).
<p align="left">
  <img src=https://coleridge-initiative.github.io/adrf_onboarding_handbook/images/use3.png alt="Desktop">
</p>

### Software in the ADRF
#### JupyterLab
**JupyterLab** provides flexible building blocks for interactive, exploratory computing. While JupyterLab has many features found in traditional integrated development environments (IDEs), it remains focused on interactive, exploratory computing. For more on JupyterLab, see the interface documentation.

The JupyterLab interface on the ADRF consists of a main work area containing tabs of documents and activities, a collapsible left sidebar, and a menu bar. The left sidebar contains a file browser, the list of running terminals and kernels, the table of contents, and the extension manager.
<p align="left">
  <img src=https://coleridge-initiative.github.io/adrf_onboarding_handbook/images/use4.png alt="JupyterLab">
</p>

When using Jupyter Notebooks, make sure that all your work is saved to your U: drive and the correct director within the U: drive. You can “nd the active directory by reading the path displayed in the file browser. By default, JupyterLab opens with your U: drive as the base directory. Below, the folder icon in the white box is my user folder (not displayed, but titled `Firstname.Lastname`; you will have already set up your folder) and subfolder WDQI.

<p align="left">
  <img src=https://coleridge-initiative.github.io/adrf_onboarding_handbook/images/use5.png alt="Make sure your work is saved to your U: drive">
</p>

##### Notebooks
Jupyter Notebooks are documents that combine live runnable code with narrative text (Markdown), equations (LaTeX), images, interactive visualizations, and other rich output. You can create a notebook by clicking the blue + button in the file browser and then selecting a kernel (R, Python3, Stata) in the Launcher tab. For more information on getting started with Jupyter Notebooks, see JupyterLab Notebook documentation.

##### Accessing Stored Data from a Notebook
A common question is how to access stored data while writing to and using a Jupyter Notebook. Data in the ADRF are stored in a database using Microsoft SQL Server. For more information on how to access stored data in the ADRF based on choice of program (Python, R, Stata), see the section on Accessing Your Data.

#### Python 3
Python is a general-purpose programming language. You can access Python in a multitude of ways:

1. **Through JupyterLab**. This is the **recommended way** to access Python since it has packages installed and available, and an execution environment for testing and running code (as well as a place to write and save code). Open JupyterLab and make sure your directory is set appropriately in the “le browser. Once there, in your new Launcher window, click the Python 3 icon.

<p align="left">
  <img src=https://coleridge-initiative.github.io/adrf_onboarding_handbook/images/use8.png alt="JupyterLab">
</p>

2. **Through the start menu (windows icon)**. Type in Python. A desktop app called Python 3.7 (64-bit) will populate a window where you can begin programming.

<p align="left">
  <img src=https://coleridge-initiative.github.io/adrf_onboarding_handbook/images/use6.png alt="Start menu">
</p>

3. **Through the command prompt in the top taskbar**. Once the command prompt window is open, type in python.

<p align="left">
  <img src=https://coleridge-initiative.github.io/adrf_onboarding_handbook/images/use7.png alt="Command Prompt">
</p>

4. **Through Pycharm**

<p align="left">
  <img src=https://coleridge-initiative.github.io/adrf_onboarding_handbook/images/use9.png alt="Pycharm">
</p>

#### R

[stopping here]
