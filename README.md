# Automate EigenLayer Program Installation
This repository contains Ansible scripts for setting up the EigenLayer program on Linux systems. It automates the installation of necessary components including Docker, Docker Compose, and Go, as well as cloning and building the EigenLayer CLI. 

## Prerequisites
A Linux system (Ubuntu 20.04 LTS or later recommended) with root access.
Git and Ansible installed on your machine.

## Getting Started
### Step 1: Installing Dependencies
Before beginning, ensure your system's packages are up to date:


```
sudo apt update && sudo apt upgrade -y
```

Install Git (if not already installed):

```
sudo apt install git -y
```

### Step 2: Cloning the Project
Clone this repository to access the Ansible playbook and necessary files:

```
git clone https://github.com/your-repository/eigenlayer-setup.git
cd eigenlayer-setup
```

### Step 3: Executing the Playbook
With the playbook downloaded, run it using the following command:

```
ansible-playbook setup_eigenlayer.yml
```

Ensure you're executing the playbook with root privileges or via a user with sudo access. This script will handle everything from installing Docker and Docker Compose to building the EigenLayer CLI.

### Step 4: Verifying Installation
To confirm the installation of the EigenLayer program, you can check the version:

```
eigenlayer --version
```