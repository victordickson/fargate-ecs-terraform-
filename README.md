# Fargate-ecs-terraform

This is a script that will allow you to successfully spin up Fargate using Terraform.
The Load balancer URL is configured to listen on port 3000.
When Terraform spins up your load balancer URL, please use port:3000, e.g example.com:3000

## Steps to Use
1. create and update a terraform.tfvars with the appropriate values.
```
aws_access_key = "AWS_ACCESS_KEY"
aws_secret_key = "AWS_SECRET_KEY"
aws_region = "us-east-1"
```
2. Run terraform init && terraform plan
3. Run terraform apply -auto-approve
4. To destroy resources, run terraform destroy -auto-approve
