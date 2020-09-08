# AWS-cloud :

- go to aws console
- select Iam
- add User
- put the username
- select programatic access
- select attach existing policy directlly
- search ec2 container registry powerUser

## cluster create :
- go to aws console
- Select ECS(Elastic container service)
- create the clustrer

## Create ECR for Docker Image:
- go to aws console

## Install the AWS CLI version 2 on Linux:
- curl "https://awscli.amazonaws.com/awscli-exe-linux-x86_64.zip" -o "awscliv2.zip"
- unzip awscliv2.zip
- sudo ./aws/install
- link : https://docs.aws.amazon.com/cli/latest/userguide/install-cliv2-linux.html
- check the aws into your terminal (write aws help to check)
- aws configure
- AWS Access Key ID [None]:
- AWS Secret Access Key [None]:
- Default region name [None]: us-east-1
- Default output format [None]: json
## Push commands for seenusdockerrig :
- aws ecr get-login-password --region us-west-2 | docker login --username AWS --password-stdin 996111791879.dkr.ecr.us-west-2.amazonaws.com
- docker tag musa101/flask_app:latest   996111791879.dkr.ecr.us-west-2.amazonaws.com/seenusdockerrig:latest
-  docker push 996111791879.dkr.ecr.us-west-2.amazonaws.com/seenusdockerrig:latest The push refers to repository [996111791879.dkr.ecr.us-west-2.amazonaws.com/seenusdockerrig]

## Create a task defination :
- Go to ECR
- Go to Task definations
- Create a new task definations
- Use EC2
- Name the Task defination
- Set the task memory(512 MB or 256)
- set the Task CPU (512 or 256)
- Add container
- add the container name
- Add image to the ECR
- Add image to the URL
- port mapping
- container port (depends on your docker images 5000)
- add Host Port( 5000)
- Create the task

## Create the service



## How to change Port Number:

- Go to Ec2 Instance
- Click security Group
- Inbound Rules
- Edit Inbound Rules
- Change Port 80 to 5000 




