### Introduction to CI / CD - Continous Integration and Continous Delivery
___________________________________________________________________________________________________

### What is CI/CD
- CI/CD - continous integration and continous delivery 
    - CI is a process where you integrate a set of tools or set of processes that you follow before delivering your application to your customer.
    - CD is a process where you deliver your application on a specific platform to your customer.

___________________________________________________________________________________________________

### Example:

- A Developer has a code for an application that is developed on their personal device and the customer is some where on the other end of the earth and how will you be able to deliver the application ? in a secure and in a reliable way ? 
- example Mobile Application - the steps for delivering the project might vary from project to project
- CI/CD is the process where you automate all these steps.
- Deliverying you application in less duration will require automation and depends on different steps like
    - Unit test your application
    - static code analysis 
    - Code quality/ vulnerability testing 
    - Automation testing
    - Reports 
    - Deployment of your application 



___________________________________________________________________________________________________
### About Jenkins

- VCS - Version control systems tools like Github, Bitbucket, Gitlab where your code exists
- Legacy Tool : 
    - V1 code - submit to github repo - pushes the changes - Deploy a CI/CD tool example: Jenkins, will tell jenkins to watch for git repo and when ever there is a pull request or new code commit made on this repo on this specific branch, then it will run set of actions.
    - As part of automation, Jenkins will run all the steps which we require.
    - jenkins will act as a orchestrator or a pipe or a tunnel. 
    - if it is a java app, you can integrate you build application in Maven and runs unit tests
    - SonarQube for code quality
    - ALM for reporting the errors
    - After it can be deployed on K8s, Docker or EC2 instance or cloud based VMS
    - This is why jenkins is called as an Orchestrator which facilitates all these above mentioned tools.
    - without CI/CD pipelines the delivering of the application process gets delayed.

___________________________________________________________________________________________________

<NOTE: As an App Developer or DEvops Enginerr you push your code which triggers a automatic pipeline either on Jenkins or Github Actions or Azure Devops Pipeline or AWS Code Pipeline, where the infrastructe can be deployed in different stages as Dev, Test, Stage, Prod>

- Usually org divides their environment like Dev, Stage and Prod
- usually PRod is where the customer can access the End Product. 

___________________________________________________________________________________________________

