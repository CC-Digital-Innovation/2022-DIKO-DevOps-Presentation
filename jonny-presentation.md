---
marp: true
theme: gaia
_class: lead
paginate: true
style: |
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

![w:300px](images/docker-logo.png)

</div>
<div data-marpit-fragment>

![w:150px v-center](images/right-arrow.png)

</div>
<div data-marpit-fragment>

![w:490px](images/k8s-logo.png)

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