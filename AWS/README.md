# Commands

- terraform init
- terraform fmt
- terraform validate
- terraform plan
- terraform apply
- terraform apply -var-file="secret.tfvars" (read vars from specific file)
- terraform apply -var "environment=prod" (set var, ignore variables.tf file)
- terraform show
- terraform state list
- terraform destroy
- terraform console (init console)
- exit or ctrl + d (close console)
- terraform apply -var='resource_tags={project="my-project",environment="dev"}'
- terraform get (get modules)

- terraform output lb_url | terraform output db_password (that ignore sensitive property)
- curl $(terraform output -raw lb_url)
- grep --after-context=10 outputs terraform.tfstate (read only var sensitive from tfstate file)
- terraform output -json (show vars from outputs.tf file)

chmod 400 ubuntu-kp-test2.pem

sudo ssh -i ./ubuntu-kp-test.pem ubuntu@15.228.50.41
sudo ssh -i ./ubuntu-kp-test2.pem ubuntu@54.218.122.180
sudo ssh -i "ubuntu-kp-test2.pem" ubuntu@ec2-54-218-122-180.us-west-2.compute.amazonaws.com
