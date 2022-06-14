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
        color: #CD5C5C;
    }

    img {
        background-color: #FFEFD5;
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
</style>

# 
# The NEW Kingmakers

![bg contain](images/DevOpsTeamPhoto3.png)

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

<!--
_class: lead
-->

<div class="columns-2-33">
<div>

# Fresh Start

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

# Containers

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

# Automate the Workflow

<div class="columns-5">
<div>

![w:100px](images/stick.png)

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

# Live Now

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

# When I started
- Refresher on Python, learned FastAPI
- Worked on Email API interactions
- Consumption of Email API

<!--- When I started the first project I was put on was working on the email API with Alex. I had to do a quick refresh of python, and learn about fast api, which is the restful api platform we were building our api with. I mostly worked on working out a few kinks, and how the api would be consumed. This led me into the second project I have worked on which was refactoring existing reporting scripts to consume the api --->

---
# Email API
- Git to kubernetes pipeline (high level)
- Logging and syslogging
- screenshot of syslog server
---
# Refactor Project
- Email API work led me to health script refactor project
- More universal code base for health reports
- Customer information pulled into single source instead of in each script

<!--- The second project I have worked on so far is a refactorization project for the reporting scripts that exist accross most of our customers. All of these scripts had their own form of emailing and this is what the email api was set up for. Refactoring them to consume the email api led to an effort to make a more universal code base that all customers could pull from instead of a variety of highly custom scripts that all accomplish roughly the same task. This effort is still ongoing --->
---

# Where it's all headed
Refactored health scripts will
- consume email api to have universal theme
- exist in a repo that is pulled each time they run at customer sites
- pull all customer info from external sources (Snow, NocoDB, ini)
<!--- The end goal of these projects will tie together many efforts of the whole team. The reporting scripts code base will consume the email api, and be hosted on github where Jonny's deployment autmoation efforts with jenkins and kubernetes will allow for each customer to pull from the latest code base before running scripts ensuring they have the most up to date code. --->