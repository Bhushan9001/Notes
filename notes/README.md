
## To Build Your Application using AWS CodeBuild and Deploy on S3 / SEBS using AWS CodePipeline, deploy Sample Application on EC2 instance using AWS CodeDeploy.


Bucket instructions
```bash
  Create an s3 bucket
  give proper name to bucket
  click on create bucket
  go to properties and enable versioning property
  add zip present in repo (must contain .yml file).
  
```
Codebuild instructions
```bash
open codebuild in aws services
click on build project
add s3 bucket as source
choose os amazon linux
use buildspec file
click on create build project
```
Pipeline Instructions
```bash
click on create pipeline
give proper name 
add source as aws s3
add build stage aws codeBuild
deploy provider aws s3
click on create pipeline

```

# To understand the Kubernetes cluster architecture, install and spin up a Kubernetes cluster on Linux Machines/Cloud platform.

Set up Docker 
Step 1 : Install Docker
Kubernetes requires an existing Docker installation. If you already have Docker installed, skip ahead to Step 2. If you do not have Kubernetes, install it by following these steps: Update the package list with the command: 
       
$ `sudo apt-get update`

Next, install Docker with the command: 

$ `sudo apt-get install docker.io`

Repeat the process on each server that will act as a node. 

Check the installation (and version) by entering the following: 

$ `docker ––version`

Step 2 : Start and Enable Docker

 Set Docker to launch at boot by entering the following:

 $ `sudo systemctl enable docker `

$ `sudo systemctl status docker`

$ `sudo systemctl start docker `
Set up Docker 
Step 1 : Install Docker
Kubernetes requires an existing Docker installation. If you already have Docker installed, skip ahead to Step 2. If you do not have Kubernetes, install it by following these steps: Update the package list with the command: 
       
$ `sudo apt-get update`

Next, install Docker with the command: 

$ `sudo apt-get install docker.io`

Repeat the process on each server that will act as a node. 

Check the installation (and version) by entering the following: 

$ `docker ––version`

Step 2 : Start and Enable Docker

 Set Docker to launch at boot by entering the following:

 $ `sudo systemctl enable docker `

$ `sudo systemctl status docker`

$ `sudo systemctl start docker `
Set up Docker 
Step 1 : Install Docker
Kubernetes requires an existing Docker installation. If you already have Docker installed, skip ahead to Step 2. If you do not have Kubernetes, install it by following these steps: Update the package list with the command: 
       
$ `sudo apt-get update`

Next, install Docker with the command: 

$ `sudo apt-get install docker.io`

Repeat the process on each server that will act as a node. 

Check the installation (and version) by entering the following: 

$ `docker ––version`

Step 2 : Start and Enable Docker

 Set Docker to launch at boot by entering the following:

 $ `sudo systemctl enable docker `

$ `sudo systemctl status docker`

$ `sudo systemctl start docker `


# Installing Kubectl
`curl -LO https://storage.googleapis.com/kubernetes-release/release/`curl -s https://storage.googleapis.com/kubernetes-release/release/stable.txt`/bin/linux/amd64/kubectl`
`chmod +x ./kubectl`
`sudo mv ./kubectl /usr/local/bin/kubectl`
`kubectl version --client`
# Installing Minikube
`curl -Lo minikube https://storage.googleapis.com/minikube/releases/latest/minikube-linux-amd64 \
  && chmod +x minikube`
`sudo mkdir -p /usr/local/bin/`
`sudo install minikube /usr/local/bin/`
`minikube start --driver=none `
# If this fails with a message "requires conntrack to be installed in root's path"
`sudo apt install conntrack`
# then try again
`sudo minikube start --driver=none`
#check the status
`sudo minikube status`
# Output:
#host: Running
#kubelet: Running
#apiserver: Running
#kubeconfig: Configured

#It is suggested (by minikube) to change the ownership and
#permissions of ~/.kube and ~/.minikube after the installation.

`sudo chown -R $USER $HOME/.kube`
`sudo chown -R $USER $HOME/.minikube`

    