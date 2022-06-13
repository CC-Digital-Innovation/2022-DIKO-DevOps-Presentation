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