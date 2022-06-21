---
marp: true
---
<style>
    section {
        background-color: #FFEFD5;
        color: #E9967A;
        font-family: Helvetica;
        font-size: 30px;
}
    h1 {
        font-weight: bold;
        font-size: 60px;
        color: #CD5C5C;
}
    h2 {
        font-weight: bold;
        font-size: 40px;
        color: #CD5C5C;

}
</style>

# TEAM INNOVATION
- Michelle Nazath
- Stefan Axelson
- Anthony Farina
- Jonny Le
- Ben Verley
- Alex Barraza

![bg left fit](images/devops.png)

---
# What is DevOps

The DevOps team, aka the coders. We build the tools that the Digital Innovation team dreams up to make life easier, our work more reliable, our data more accurate.


---

![bg fit](images/chaos5.png)

---

# PATH TO ORDER
1. Gather Requirements Uniformly
2. Properly Sequence Tasks & Projects
3. Individual Task Management
4. Understand & Articulate Value 
5. Sales Messaging
![bg cover opacity:20%](images/chaos6.jpeg)

---

# WORKFLOW
```mermaid
sequenceDiagram
    participant Business Requirements
    participant Request Log
    participant Work Request
    participant Closeout
    Business Requirements-->>Request Log: Submit Request
    Note left of Business Requirements: ops team to submit request 
    Request Log-->>Work Request: Prioritze, Assign, Schedule
    loop 
        Request Log-->>Work Request: Review & Update Request Log
        Work Request-->>Work Request: Iterate
    end
    Work Request-->>Closeout: Documentation, Knowledge Transfer
```
---
```mermaid
graph LR
    A[eng1] --> |submit request| E(Request Log)
    B[eng2] --> |submit request| E(Request Log)
    C[eng3] --> |submit request| E(Request Log)
    D[eng4] --> |submit request| E(Request Log)
    E --> F{Review Request}
    F --> G{fa:fa-spinner Work Request}
    G --> H{fa:fa-glasses Review}
    H -->|iterate|G
    H --> I{fa:fa-folder Documentation}
    I --> J(fa:fa-light Knowledge Transfer)
    J --> K(fa:fa-flag Completed)
```
---
[![](https://mermaid.ink/img/pako:eNqFksFOwzAMhl_FyoFT9wI5TALGAYEQWkFcegmN20WkcYkdJpj27qS0kwqdhE-W_Pv7f1k-qJosKq0Y3xOGGjfOtNF0VYBcvYniatebIHCV2AVkhm1WuogdBuGlbJgiC9xTuxy-UHw7KZbTa0-MlKbJWb_Var2eOWgo02vn5DfzgQTBYyNAzXmMBuoZBE0HQsAjI07cETJzGUznyTU8RkfRyRcWcMns2lBAWe_QJo_jtifqJ9C_sC1-ONzDBTz31uTkiwsONV9ZIm4FY14d5Rjs2PzdOd1Xw4bqNBzCiKOc_S7Q3qNtEZ6iCdxgrIIqVIexM87m5zgMwErJLp-vUjq3FptkvFSqCscsTT_Rb6wTiko3xjMWyiSh8jPUSktMeBJNDzapjt-b4N3J)](https://mermaid.live/edit#pako:eNqFksFOwzAMhl_FyoFT9wI5TALGAYEQWkFcegmN20WkcYkdJpj27qS0kwqdhE-W_Pv7f1k-qJosKq0Y3xOGGjfOtNF0VYBcvYniatebIHCV2AVkhm1WuogdBuGlbJgiC9xTuxy-UHw7KZbTa0-MlKbJWb_Var2eOWgo02vn5DfzgQTBYyNAzXmMBuoZBE0HQsAjI07cETJzGUznyTU8RkfRyRcWcMns2lBAWe_QJo_jtifqJ9C_sC1-ONzDBTz31uTkiwsONV9ZIm4FY14d5Rjs2PzdOd1Xw4bqNBzCiKOc_S7Q3qNtEZ6iCdxgrIIqVIexM87m5zgMwErJLp-vUjq3FptkvFSqCscsTT_Rb6wTiko3xjMWyiSh8jPUSktMeBJNDzapjt-b4N3J)

---

# REQUEST LOG
## REQUEST FORM
- [Request Form Link](https://app.smartsheet.com/b/form/5af35d5dc51f42f5975e4570f7f8e268)

## DASHBOARD
- [Dashboard Link](https://app.smartsheet.com/dashboards/w8pRRQfjGW65354rFpCcj4PxC4h6fVJ65F65Cv41)
-- Active Request Log
-- Completed Request Log
-- Request Summaries
![bg right 90%](images/dashboard.png)

--- 


<div class="center">

![](images/emailapimermaid.svg)

</div>

---

# EMAIL API

## Problem Statement
As part of our services we provide daily reports via email with the current status of all devices we manage. This provides huge value to the customer in that is gives them a summary of the environments health each morning they can review quickly without having to login and check each system manually or sort through individual emails from each device. However maintaining this has been complex, there had to be a better way. Issues with the original deployment were:
- Inconsistency of format, structure and deployment of all email updates
- Dependent on the customer to run said email report
- In ability to manage updates to script across all customers at once

---

# EMAIL API | CREATE REPORT

<div class="columns-2">
<div>

* Sends an HTML Tabular Report
* Attachments allowed
* Body/descriptions allowed
* All attachments are saved in NocoDB
* All events are logged in a syslog

</div>
<div>

![w:1200px](images/emailAPI.PNG)

</div>

---
# EMAIL API | CREATE DATABASE (NocoDB)

<div class="columns-2">
<div>

![w:1000](images/NocoDB.png)

</div>
<div>

* Open Source
* Converts a database to spreadsheets
* Saves all attachments
* Located by timestamp

</div>

---

<!-- _class: mjn -->

## EMAIL API | SYSLOG

- Leverages loguru for local logging and sysloging
- Various options for logging
    - console
    - file
    - syslog

![bg vertical right:50% 100%](images/syslogemailapi.png)
![bg 100%](images/syslogfile.png)

<!-- Follows the automated workflow, Git to kubernetes pipeline (high level)screenshot of syslog server-->

---

# REFACTOR HEALTH SCRIPT PROJECT
- Email API work led us to health script refactor project
- More universal code base for health reports
- Eliminated the depenecy of hard coded Customer information in individual scripts 
    - Created NocoDB for configuration setting

<!--- The second project I have worked on so far is a refactorization project for the reporting scripts that exist accross most of our customers. All of these scripts had their own form of emailing and this is what the email api was set up for. Refactoring them to consume the email api led to an effort to make a more universal code base that all customers could pull from instead of a variety of highly custom scripts that all accomplish roughly the same task. This effort is still ongoing --->

---

# WHERE WE ARE HEADED
Refactored health scripts will
- consume email api to have universal theme
- exist in a repo that is pulled each time they run at customer sites
- pull all customer info from external sources (Snow, NocoDB, ini)
<!--- The end goal of these projects will tie together many efforts of the whole team. The reporting scripts code base will consume the email api, and be hosted on github where Jonny's deployment autmoation efforts with jenkins and kubernetes will allow for each customer to pull from the latest code base before running scripts ensuring they have the most up to date code. --->