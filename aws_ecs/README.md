# Launch a docker project on AWS

1 - create a base docker image for faster builds

2 - create ECR repo for base image and push the image

3 - create app docker image from base image using the ECR link

4 - make sure docker container works locally

5 - create ECR repo for app docker

6 - create security groups for ALB and ECS instances
- port 80 and 443 for ALB
- traffic from ALB security group for ECS instances on port 80 only
- port 22 for ssh

7 - create ALB with ALB security group and Target group with healthchecks

8 - create ECS cluster with the corresponding security group for instances and use the created ALB

9 - create ECS task

10 - create pipeline/build

11 - create ESC service

12 - finish pipeline creation
