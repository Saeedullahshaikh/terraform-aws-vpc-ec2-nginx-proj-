# Terraform AWS VPC, EC2, and Nginx Project

This project demonstrates the deployment of a **Virtual Private Cloud (VPC)**, an **EC2 instance**, and the installation of the **Nginx web server** on AWS using **Terraform**.

---

## 🚀 Project Overview

The goal of this project is to automate the creation of a secure AWS infrastructure that includes:

* A **VPC** with public and private subnets.
* An **EC2 instance** running Ubuntu.
* Installation of the **Nginx web server** on the EC2 instance.
* Configuration of **security groups** to allow HTTP and SSH access.

---

## 🛠️ Project Structure

```
terraform-aws-vpc-ec2-nginx-proj/
├── main.tf            # Main Terraform configuration
├── providers.tf       # Provider configurations
├── vpc.tf             # VPC and subnet configurations
├── ec2.tf             # EC2 instance configuration
├── security_groups.tf # Security group configurations
├── outputs.tf         # Output variables
└── variables.tf       # Input variables
```

---

## 👞 Prerequisites

Before you begin, ensure you have the following:

* [Terraform](https://www.terraform.io/downloads.html) installed.

* An active [AWS account](https://aws.amazon.com/).

* AWS credentials configured on your machine. You can set them up using the AWS CLI:

  ```bash
  aws configure
  ```

* Basic knowledge of AWS services and Terraform.

---

## ⚙️ Usage

1. **Clone the repository**:

```bash
git clone https://github.com/Saeedullahshaikh/terraform-aws-vpc-ec2-nginx-proj-.git
cd terraform-aws-vpc-ec2-nginx-proj-
```

2. **Initialize Terraform**:

```bash
terraform init
```

3. **Review the execution plan**:

```bash
terraform plan
```

4. **Apply the configuration to create the resources**:

```bash
terraform apply
```

Type `yes` when prompted to confirm the creation of resources.

5. **Access the Nginx Web Server**:

* After deployment, Terraform will output the **Public IP** of the EC2 instance. Open this IP in your browser to see the default Nginx welcome page.

6. **Destroy the infrastructure** (when no longer needed):

```bash
terraform destroy
```

Type `yes` when prompted to confirm the destruction of resources.

---

## 🛠️ Features

* **VPC Creation**: Automates the setup of a Virtual Private Cloud with public and private subnets.
* **EC2 Deployment**: Launches an Ubuntu EC2 instance within the VPC.
* **Nginx Installation**: Installs and starts the Nginx web server on the EC2 instance.
* **Security Groups**: Configures security groups to allow HTTP and SSH access.
* **Outputs**: Provides the public IP of the EC2 instance upon successful deployment.

---

## Author

**Saeedullah Shaikh**
- GitHub: [@Saeedullahshaikh](https://github.com/Saeedullahshaikh)

## 📜 License

This project is licensed under the MIT License.
