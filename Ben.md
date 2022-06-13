---
marp: true
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