# Infrastructure Repository

This repository contains the infrastructure code written in Terraform and organized using Terragrunt to create and manage infrastructure resources in Azure. The repository is structured into different directories for managing shared resources, development environment, and reusable modules.

## Repository Structure

The repository is organized into the following directories:

- `modules`: Contains reusable Terraform modules that can be used across different infrastructure components.
- `shared`: Contains the Terraform code for shared resources that are used by multiple environments.
- `dev`: Contains the Terraform code for the development environment.

## Prerequisites

Before you begin, make sure you have the following prerequisites set up:

- [Terraform](https://www.terraform.io/downloads.html) installed on your local machine.
- [Terragrunt](https://terragrunt.gruntwork.io/docs/getting-started/install/) installed on your local machine.
- [Azure CLI](https://docs.microsoft.com/en-us/cli/azure/install-azure-cli) installed on your local machine.
- Azure credentials with appropriate permissions to create and manage resources. You can obtain these credentials by logging in to Azure using the Azure CLI (`az login`).

## Running Terragrunt

To deploy the infrastructure using Terragrunt, follow these steps:

1. Clone this repository to your local machine:

```bash
git clone https://github.com/your-username/your-infrastructure-repo.git
cd your-infrastructure-repo
```
2. Change directory to the worksapce you want to deploy (e.g., `dev/.../vnet`).

3. Initialize the Terraform modules and backend configuration.

```bash
terragrunt init
```
4. Generate an execution plan to see the changes that will be applied.
```bash
terragrunt init
```
4. Generate an execution plan to see the changes that will be applied.
```bash
terragrunt apply
```


## Obtaining Azure Credentials

To obtain Azure credentials for authentication, follow these steps:

1. Open a terminal or command prompt.

2. Run the following command to log in to Azure:
```bash
az login
```

Follow the prompts to authenticate with your Azure account. Once authenticated, you will have the necessary credentials to manage Azure resources.

Please ensure that the Azure account used for login has sufficient permissions to create and manage resources in the target Azure subscription.

## Additional Resources

For more information about Terraform, Terragrunt, and Azure, refer to the following documentation:

- [Terraform Documentation](https://www.terraform.io/docs/index.html)
- [Terragrunt Documentation](https://terragrunt.gruntwork.io/docs/)
- [Azure CLI Documentation](https://docs.microsoft.com/en-us/cli/azure/)
- [Azure Documentation](https://docs.microsoft.com/en-us/azure/)