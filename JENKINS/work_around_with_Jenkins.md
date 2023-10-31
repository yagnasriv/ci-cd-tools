### Introduction to Jenkins 
___________________________________________________________________________________________________

### Installation of Jenkins
- Jenkins is a Java based product
- install java - jdk lastest 17 or above for beforing installing Jenkins 
- login into the Jenkins once installed using
    - http://ip_address_of_the_machine:8080
    - make sure to have the 8080 port added to the securtiy group for the ec2 instance
    - Before logging into the Jenkins server, to get the admin password make sure to run the
        - sudo cat /var/lib/jenkins/secrets/initialAdminPassword
    - Click on Install suggested plugins and later while working around you can add/ install which ever plugins you require.

___________________________________________________________________________________________________

### How Jenkins work in Real Time 

- How Jenkins architecture work ?
    - Jenkins master node is where you install Jenkins and it is usually used for scheduling and there are worker nodes ( 1, 2, 3 ... etc)
    - where these worker nodes are used to updating applications based on group vise or for certain groups
    - If few workers nodes are not being used frequently then those resources are being wasted 
    - To avoid this scenario, we will use the latest aproach where we use Docker Agent for running Jenkins' pipelines.

___________________________________________________________________________________________________

#### How to use Docker agent for running Jenkins pipelines

- MAke sure to check if docker is installed on the Ec2 instance 
- If not, use the sudo apt install docker.io command to install docker on the machine and with the help of sudo command change the perimission for the docker group for running the docker commands.
- Once Docker installation is completed, login into the jenkins server and install docker pipeline plugin, this plugin is required to run the jenkins pipelines using docker agent.
- and restart the jenkins server so that the installed docker plugin will be available.

___________________________________________________________________________________________________

### Writing our first Jenkins pipeline

- Click on create a Job for creating your first jenkins pipeline,
- You can create a pipeline in different ways, like
    - FreeStyle Project
    - Pipeline
    - Multi Configuration project
    - folder
    - Multibranch pipeline
    - organization folder

- In this example, you will use pipeline approach 
    - By using pipeline approach you can use a Declerative or scripted pipeline approach. 
- 
