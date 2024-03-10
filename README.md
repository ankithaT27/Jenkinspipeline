wwhat is CICD?

Continuous integration (CI) refers to the practice of automatically and frequently integrating code changes into a shared source code repository. Continuous delivery and/or deployment (CD) is a 2 part process that refers to the integration, testing, and delivery of code changes. Continuous delivery stops short of automatic production deployment, while continuous deployment automatically releases the updates into the production environment.

A continuous integration and continuous deployment (CI/CD) pipeline is a series of steps that must be performed in order to deliver a new version of software

# Jenkinspipeline
Jenkins groovy scripting - Declarative jenkins pipeline
CI:
whenever there is any commit in our gitlab repo, it triggers a jenkins pipeline
so, first the code is checked out, and we build it using maven along with unit test test cases
the code is scanned for any vulnerabilities using ex- sonarqube
we will build a container image and the image is scanned
we will push to image registry (dockerhub/ecr etc)

Update image manifests, update all the Helm charts
using argo cd (argo cd watches git repo continuosuly) and it deployed to kubenetes or use a shell script/helm command we push to the kuberetes platform



