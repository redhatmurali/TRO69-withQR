# TR069-withQR — CMS Installation

Installation script for deploying the TR-069 CMS using Docker on Ubuntu 24.04 LTS.

## Requirements

- Ubuntu 24.04 LTS
- Root or sudo access
- Internet connectivity
- A server or virtual machine with sufficient resources

## Installation

### 1. Update the system

```bash
sudo apt update
sudo apt upgrade -y
sudo apt install -y curl wget
```

### 2. Check the Linux kernel

```bash
uname -r
```

### 3. Download and run the installation script

Run the following commands:

```bash
wget -qO install_cms.sh https://raw.githubusercontent.com/redhatmurali/TR069-withQR/main/install_cms.sh

chmod +x install_cms.sh

sudo bash install_cms.sh
```

**One-line installation command:**

```bash
wget -qO install_cms.sh https://raw.githubusercontent.com/redhatmurali/TR069-withQR/main/install_cms.sh && chmod +x install_cms.sh && sudo bash install_cms.sh
```

> **Security note:** Review the installation script before running it with root privileges.

## Notes

- Use Ubuntu 24.04 LTS as the required operating system.
- Ensure that the server has internet connectivity during installation.
- Follow the prompts displayed by the installation script.
- Configure the CMS according to your network, OLT, and VLAN settings after installation.



