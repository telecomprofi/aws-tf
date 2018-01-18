# Terraform modules to work with AWS

How to use:
0. Checkout required .tf file from repo
1. download and install terraform, unzip and add its directory to the PATH env variable. run from console
terraform init (that will download  required providers from hashicorp terraform.io)
2. export ACCESS ID and ACCCESS KEY env variables 
export AWS_ACCESS_KEY_ID=
export AWS_SECRET_ACCESS_KEY=
3. edit .tf file to add your specific parameters (like ec2 instance type, ami id, region, elb, vpc, etc)
4. run dry-run with $ terraform plan -out <your planned actions file>
5. check on-screen changes and if they are ok run
terraform apply (answer "yes" when prompted).


if you would like to see graph of your deployment issue command like this  terraform graph | dot -Tpng > graph.png (graphviz is required)
