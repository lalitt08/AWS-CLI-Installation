# AWS CLI Version 2 Installation Guide for Ubuntu

This README provides detailed instructions for installing the AWS Command Line Interface (CLI) Version 2 on Ubuntu. AWS CLI is a powerful toolset that helps you manage and interact with AWS services using the command line.

## Prerequisites

Before you begin, ensure you have `curl` installed on your Ubuntu system. If it is not installed, you can install it by running:

```bash
sudo apt update
sudo apt install curl

Installation Steps
Step 1: Download the AWS CLI v2
Use curl to download the latest version of AWS CLI v2 installation package:

bash
Copy
curl "https://awscli.amazonaws.com/awscli-exe-linux-x86_64.zip" -o "awscliv2.zip"
Step 2: Install Unzip Utility
AWS CLI v2 is packaged as a zip file. You will need unzip to extract it. Install unzip using apt if it is not already installed:

bash
Copy
sudo apt install unzip
Step 3: Unzip the Installation Package
Extract the installation package:

bash
Copy
unzip awscliv2.zip
Step 4: Run the Installer
Navigate to the extracted directory and execute the installation script:

bash
Copy
sudo ./aws/install
Step 5: Verify the Installation
After the installation is complete, verify that AWS CLI v2 is installed correctly:

bash
Copy
aws --version
This command should output the installed version of AWS CLI v2, confirming that the installation was successful.

Post-Installation
After installing, configure AWS CLI with your credentials to start interacting with AWS services:

bash
Copy
aws configure
Enter your AWS Access Key ID, Secret Access Key, region, and output format when prompted.
