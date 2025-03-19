# ADRF User Guide

_A detailed guide to help users navigate and use the **Coleridge Initiative's** Administrative Data Research Facility (ADRF) effectively._

_Last Modified: `git log -1 --format=%cd --date=short`_

---

## Table of Contents
1. [Introduction](#introduction)  
2. [ADRF Access and Account Set Up](#adrf-access-and-account-set-up)  
3. [Onboarding Modules and Security Training](#onboarding-modules-and-security-training)
4. [Features](#features)  
5. [Usage Examples](#usage-examples)  
6. [Troubleshooting](#troubleshooting)  
7. [FAQ](#faq)

---

## Introduction

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

## ADRF Access and Account Set Up

### Requesting an Account
- **Agency-affiliated researcher**. If you are an agency-affiliated researcher, your agency will set up an ADRF account for you.
- **Individual part of a training program**. If you are part of a [training program](https://coleridgeinitiative.org/applied-data-analytics-training-programs), the Coleridge Initiative team will create an account for you once you have been accepted into the program.

### Account Registration and Onboarding Tasks
- You will receive an email invitation to activate your account. The email will come from [http://okta.com](http://okta.com), so please make sure that it doesn’t get caught in your email spam filter. Follow the steps outlined in the email to set up your password and your multi-factor authentication preferences. Clink on the link below to watch a video walking through the steps.
- After activating your account, you will be logged in to the ADRF Applications page. Proceed to the **Management Portal** by clicking on the icon.
- In the **Management Portal**, you will notice a “Onboarding Tasks” section within “Admin Tasks” with a number of items you will need to complete before you can gain access to the project space. Refer to the next section for details about the onboarding process.

### Obtaining ADRF Access
- **Agency-affiliated researcher**. If you are an agency-affiliated researcher using an agency-sponsored account, you will be granted ADRF access once you complete your onboarding tasks and required data access agreements. If you are a self-paying agency-affiliated researcher, your ADRF access is conditional on receipt of payment. If your institution of Office of Sponsored Programs will be submitting payment on your behalf, please be aware of potential access delays. Whenever possible, the Coleridge Initiative advises paying with a personal credit card or institutional payment card and using the generated invoice to request reimbursement.
- **Individual part of a training program**. If you are part of a training program, you will be granted ADRF access once you complete your onboarding tasks and required data access agreements.

### More Information
If you have any questions, please contact [support@coleridgeinitiative.org](mailto:support@coleridgeinitiative.org).

---

## Onboarding Modules and Security Training

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



