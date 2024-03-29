---
marp: true
---
<style>
    section {
        background-color: #21618C;
        color: #FFFFFF;
        font-family: Helvetica;
        font-size: 30px;
    }
    h1 {
        font-weight: bold;
        font-size: 60px;
        color: #5DADE2;
        text-align: center;
    }
    h2 {
        font-weight: bold;
        font-size: 40px;
        color: #AED6F1;
    }
    a{
        color: #82E0AA;
    }
    section.mjn{
        background-color: #21618C;
        color: #FFFFFF;
        font-family: Helvetica;
        font-size: 25px;
    }
    h1.mjn {
        font-weight: bold;
        font-size: 35px;
        color: #5DADE2;
        text-align: center;
    }
    
    h2.mjn {
        font-weight: bold;
        font-size: 25px;
        color: #AED6F1;
    }
    section.table {
        background-color: white;
        color: #5DADE2;
        font-family: Helvetica;
        font-size: 25px;
    }
    h1.table {
        font-weight: bold;
        font-size: 35px;
        color: #21618C;
        text-align: center;
    }
    
    h2.table {
        font-weight: bold;
        font-size: 25px;
        color: #21618C;
    }
    img {
        background-color: #21618C;
    }
    .columns-2 {
        display: grid;
        grid-template-columns: repeat(2, minmax(0, 1fr));
    }

    .columns-2-33 {
        display: grid;
        grid-template-columns: 1fr 2fr;
    }

    .columns-3 {
        display: grid;
        grid-template-columns: 1fr 0.5fr 1.5fr
    }

    img[alt~="v-center"] {
        padding: 70px 0;
    }

    .columns-5 {
        display: grid;
        grid-template-columns: repeat(5, minmax(0, 1fr));
        padding: 0 80px;
    }
    .center {
        display: block;
        margin: 0;
        padding: 0;
        text-align: center;
    }
</style>

# 
# The NEW Kids on the Block

![bg contain](images/DevOpsTeamPhoto3.png)

---
# WHAT IS DEVOPS?

The DevOps team, aka the coders. We build the tools that the Digital Innovation team dreams up to make life easier, our work more elegant,reliable, our data more accurate.


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

<div class = "mermaid">
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
</div>

---

<div class = "mermaid">
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
</div>

---
[![](https://mermaid.ink/img/pako:eNqFksFOwzAMhl_FyoFT9wI5TALGAYEQWkFcegmN20WkcYkdJpj27qS0kwqdhE-W_Pv7f1k-qJosKq0Y3xOGGjfOtNF0VYBcvYniatebIHCV2AVkhm1WuogdBuGlbJgiC9xTuxy-UHw7KZbTa0-MlKbJWb_Var2eOWgo02vn5DfzgQTBYyNAzXmMBuoZBE0HQsAjI07cETJzGUznyTU8RkfRyRcWcMns2lBAWe_QJo_jtifqJ9C_sC1-ONzDBTz31uTkiwsONV9ZIm4FY14d5Rjs2PzdOd1Xw4bqNBzCiKOc_S7Q3qNtEZ6iCdxgrIIqVIexM87m5zgMwErJLp-vUjq3FptkvFSqCscsTT_Rb6wTiko3xjMWyiSh8jPUSktMeBJNDzapjt-b4N3J)](https://mermaid.live/edit#pako:eNqFksFOwzAMhl_FyoFT9wI5TALGAYEQWkFcegmN20WkcYkdJpj27qS0kwqdhE-W_Pv7f1k-qJosKq0Y3xOGGjfOtNF0VYBcvYniatebIHCV2AVkhm1WuogdBuGlbJgiC9xTuxy-UHw7KZbTa0-MlKbJWb_Var2eOWgo02vn5DfzgQTBYyNAzXmMBuoZBE0HQsAjI07cETJzGUznyTU8RkfRyRcWcMns2lBAWe_QJo_jtifqJ9C_sC1-ONzDBTz31uTkiwsONV9ZIm4FY14d5Rjs2PzdOd1Xw4bqNBzCiKOc_S7Q3qNtEZ6iCdxgrIIqVIexM87m5zgMwErJLp-vUjq3FptkvFSqCscsTT_Rb6wTiko3xjMWyiSh8jPUSktMeBJNDzapjt-b4N3J)

---
# WE ARE NOT MIND READERS
<br>

<div class="center">

![](https://media.giphy.com/media/lELRD773cY7Sg/giphy.gif)

</div>

<br>

# _SO PLEASE USE OUR REQUEST LOG!_


---

## REQUEST FORM
[Request Form Link](https://app.smartsheet.com/b/form/5af35d5dc51f42f5975e4570f7f8e268)
![bg left:60% 95%](images/form1.png)
![bg 95%](images/form2.png)

---

# DASHBOARD
- [Dashboard Link](https://app.smartsheet.com/dashboards/w8pRRQfjGW65354rFpCcj4PxC4h6fVJ65F65Cv41)
-- Active Request Log
-- Completed Request Log
-- Request Summaries
![bg right 90%](images/dashboard2.png)

---

# COMPLETED | ACTIVE | BACKLOG

![](images/completed.png)
![](images/active.png)

---


---

<!--
_class: lead
-->

<div class="columns-2-33">
<div>

# FRESH START

* What tools to use?
* How about the workflow?

</div>
<div data-marpit-fragment>

![w:700px](images/devops.jpeg)

</div>
</div>

<!--
- devops team was new and what is it
- emphasize number of tools to choose from
- devops is about efficiency and speed
-->

---

<!--
_class: lead
-->

# CONTAINERS

<div data-marpit-fragment class="columns-3">
<div>

![w:300px v-center](images/docker-logo.png)

</div>
<div data-marpit-fragment>

![w:150px v-center](images/right-arrow.png)

</div>
<div data-marpit-fragment>

![w:490px v-center](images/k8s-logo.png)

</div>
</div>

<!--
- what are containers: illustrate with Moby
- more tools = more complexity, right?
-->

---

<!--
_class: lead
-->

# AUTOMATE THE WORKFLOW

<div class="columns-5">
<div>

</div>
<div>

![w:150px](images/github.png)

</div>
<div>

![w:100px](images/jenkins.png)

</div>
<div>

![w:150px](images/gitlab.png)

</div>
<div>

![w:150px](images/k8s-logo.png)

</div>
</div>

![w:1070px](images/devops-workflow-1.svg)

<!--
- manually, the process is like...
- emphasize single line from dev pov
-->

---

# LIVE NOW

<div class="columns-2">

<div class="columns-2">
<div>

![w:200px](images/vault.png)
![w:300px](images/fastapi.png)


</div>
<div>

![w:240px](images/jenkins.png)
![w:280px](images/gitlab.png)


</div>
</div>

<div>

#### **Docker**

- PRTG Test Drive

#### **Kubernetes**

<div class="columns-2">
<div>

- Vault
- Jenkins
- Gitlab

</div>
<div>

- SNOW to PRTG Automation
- Email API

</div>
</div>
</div>
</div>

<!--
- self-deployed apps
-->

---

---
<!-- _class: mjn -->

## TOOL SYNCHRONIZATION

### WHY
* ServiceNow to become the single source of truth 

### PROJECTS AROUND THIS WHY
* 
* Map Device 42 to SNOW CMDB automatically 
* Automated sync script across PRTG > Meraki > SNOW that detects and corrects naming convention errors

### REV 2
* Improve internal workflow on Device42

![bg left:30%](https://media.giphy.com/media/eJFnnIa1UZEirYB7TU/giphy.gif)

---

# DEVELOPERS WORKFLOW 
## SNOW TO PRTG DEPLOYMENT
### PROBLEM STATMENT
Deployment of PRTG for each customer was very manual and comprehensive process that is completely seperated from SNOW CMDB creation. So we were constantly running into the issue of SNOW and PRTG not matching.

---




---
<!-- _class: mjn -->

## TOOL SYNCHRONIZATION

<div class="columns-2">
<div>

### MVP 
- Automated sync script across PRTG > Meraki > SNOW that detects and corrects naming convention errors
- Workflow
    - Gathers information about a device from PRTG & Meraki 
    - Validates ServiceNow records match customer environments
</div>
<div>

### Rev 2 | Change Control
 - Automate ticket creation before device names are changed
 - Require Customer Approval
 - Execute cross-environmental changes
### Rev 3 | Generalization
- Expand to other customers
- Expand to other vendors
</div>

---

# PRTG SENSOR CLEANUP
- 70,000 sensors
- Automated the deletion of 10s of thousands of sensors to make the PRTG monitoring system more responsive
- Used the PRTG API to detect and delete only specific sensors in the network

 <!-- First exposure to using an API and working with an enterprise network monitoring tool-->

![bg right 90%](https://media.giphy.com/media/26gscNQHswYio5RBu/giphy.gif)


---

![bg right](https://www.forte-systems.com/wp-content/uploads/Banner1024x300-83.jpg)

# SNOW PROJECTS
- Engineer "My Work Page" Redesign
- Homepage Redesign
- Change Overview Board
- Customer Service Board
- SLA Overhaul
- Portal Overhaul

---

SNOW CONTINUED - pending photos from stefan

---

SNOW CONTINUED - pending photos from stefan

---

# THE END


---

ABOUT ME NOTES

<!---
BEN
# When I started
- Refresher on Python, learned FastAPI
- Worked on Email API interactions
- Consumption of Email API

 When I started the first project I was put on was working on the email API with Alex. I had to do a quick refresh of python, and learn about fast api, which is the restful api platform we were building our api with. I mostly worked on working out a few kinks, and how the api would be consumed. This led me into the second project I have worked on which was refactoring existing reporting scripts to consume the api --->

 <!-- 
 ANTHONY
 # When I started / What I do
 - I started at the beginning of February last year
 - I specialize in automation
 - I typically work with the PRTG, Meraki, and pysnow APIs to create scripts that will help customers or the team-->


 <!--
 STEFAN
 - Joined Onboarding in 2020
- Became Snow Admin after Lisa left in 2021
- Moved to Dev Ops in 2022-->