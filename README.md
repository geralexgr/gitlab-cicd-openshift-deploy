# gitlab-cicd-openshift-deploy
This repository holds an example **.yml** file that can be used to deploy recourses on Openshift through Gitlab CI/CD.

The pipeline consists of three steps:

1. Houseekeping (deletes any leftovers from previous run attempts)
2. Deployment (deployment of pod microservice)
3. Cleanup (destroys the build pods)

The pipeline should trigger only for develop branch and it should be placed accordingly on the root structure of this branch.

The build strategy is set to be docker as a result a Dockerfile should exist along with the .yml file on the root directory with the instructions for the building. An example Dockerfle is placed on the repository for reference.
