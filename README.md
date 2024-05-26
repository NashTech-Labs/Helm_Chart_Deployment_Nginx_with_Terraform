# Helm Chart Deployment: Nginx with Terraform

This repository contains Terraform configuration files to automate the installation of Nginx on a Kubernetes cluster using Helm Chart.

## Prerequisites

Before using this Terraform configuration, make sure you have the following prerequisites:

- Kubernetes cluster up and running
- `kubectl` configured to connect to your Kubernetes cluster
- Helm installed on your local machine
- Terraform installed on your local machine

## Usage

Follow these steps to install Nginx on your Kubernetes cluster:

1. Clone this repository to your local machine.
2. Run `terraform init` to initialize the Terraform configuration.
3. Run `terraform apply` to apply the changes and install Nginx.
4. After the installation completes, access Nginx using the provided NodePort.

## Configuration

- Helm Release Configuration: Modify the main.tf file to customize the Helm release name, repository, chart, and values file.

## Resources

This Terraform configuration deploys the following resources:

- Helm Release: Installs the Nginx Helm chart from the specified repository.


## Cleanup

To remove Nginx installation, run `terraform destroy`. Make sure to take necessary backups before destroying the resources.