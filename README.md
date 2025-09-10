# Terraform_learn
Learning terraform by doing hands-on

This project demonstrates how to use [Terraform](https://www.terraform.io/) to provision AWS infrastructure. It sets up a basic EC2 instance using an Ubuntu AMI.

## 📁 Project Structure
learn-terraform-get-started-aws/
├── main.tf # Main Terraform configuration
├── terraform.tf # AWS provider and resource declarations
├── terraform.tfstate # Terraform state file (generated after apply)


## 🔧 Prerequisites
Make sure you have the following installed on your Ubuntu system:
- [Terraform](https://developer.hashicorp.com/terraform/downloads)
- [AWS CLI v2](https://docs.aws.amazon.com/cli/latest/userguide/install-cliv2.html)

### Install AWS CLI v2 (if needed)
sudo apt update
sudo apt install curl unzip -y
curl "https://awscli.amazonaws.com/awscli-exe-linux-x86_64.zip" -o "awscliv2.zip"
unzip awscliv2.zip
sudo ./aws/install

🔐 Configure AWS Credentials
Before using Terraform, export your AWS credentials or use aws configure.
export AWS_ACCESS_KEY_ID=your-access-key-id
export AWS_SECRET_ACCESS_KEY=your-secret-access-key
Or run:
aws configure

🚀 How to Use
Initialize Terraform
terraform init

Validate the Configuration
terraform validate

Format Terraform Files
terraform fmt

Apply the Configuration
terraform apply

Check the Terraform State
terraform state list
terraform show

🧹 Cleanup
To destroy all created resources:
terraform destroy

📌 Notes
Do not commit terraform.tfstate or AWS credentials to GitHub.
