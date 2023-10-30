### How to Implement CI CD on AWS
___________________________________________________________________________________________________

- Using AWS Managed Services that will help CI/CD on AWS
- Amazon Web Services' CI/CD service that automates the build, test, and deployment phases of your release process.

### AWS Code Commit
___________________________________________________________________________________________________

- Usual CI / CD tools are
    - Jenkins
    - Argo CD
    - GitLab CI/CD
    - GitHub Actions
    - AWS codeCommit, codePipeline, codeBuild and codeDeploy using this 4 services you can implement the entire CI/CD provess within AWS and by AWS.



- Example: Take Jenkins: 
    - you have an application that you want to deploy on K8s 
    - use jenkins as a orchestrator
    - A Place where your code is hosted - github
    - when someone commits the code on github it triggers the webhook and it triggers the - jenkins pipeline
    - Build Processs: within the pipeline you have build process, building of application. - docker, maven for java application, sonarQube
    - finally built product it can be a docker image and deploy on k8s or EC2 instance. argocd/ shell script for deploying image on k8s or ec2 instance.

AWS said instead of using 4 different tools, AWS came up with own managened services
- USE AWS CodeCommit instead of github
- USE AWS CodePipeline instead of jenkins pipeline
- USE AWS CodeBuild instead of building the application, example Maven for java applications
- USE AWS CodeDeploy instead of argoCD you can use code deploy service. 



