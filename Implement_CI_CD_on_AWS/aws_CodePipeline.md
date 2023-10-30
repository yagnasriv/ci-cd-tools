### AWS CodePipeline
___________________________________________________________________________________________________

- Compare AWS Code Pipeline with open source platform Jenkins 
- Jenkins is a Orchestrator.
- how does a usual CI/CD work with Jenkins ? 
    - Jenkins is a open source platform
    - How does the workflow begin ? 
    - Source code repo - github, bitbucket, gitlab 
    - target platform - Kubernetes 
    - A Developer - makes a code commit into github
    - then pushes the code change to github, where the webhook integrated with jenkins gets triggered and the jenkins pipeline (declerative pipelines or scripted pipelines in the groovy ) gets run with the new changes.
    - example: developer made changes to a .java file
    - jenkins pipeline get triggers
    - builds an image (docker)
    - CI - you have multiple stages : code checkout, build and unit test cases these depends on one org to other.
    - code scan, sonarQube for implementation.
    - 