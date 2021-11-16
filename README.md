# upgrade_apache_ubuntu
How to Upgrade Apache to Latest Version on Ubuntu 20.04


# Updating Operating System
- sudo apt update && sudo apt upgrade -y

# Install Latest Apache
- apache2 -v

Server version: Apache/2.4.41 (Ubuntu)

# Adding Apache PPA
sudo add-apt-repository ppa:ondrej/apache2 -y && sudo apt update

# Upgrade Apache from PPA
- sudo apt install apache2
- sudo apt update
- sudo apt upgrade apache2 -y

# Verify version and Apache status
- apache2 -v

Server version: Apache/2.4.51 (Ubuntu)

- sudo systemctl status apache2

# Configure UFW Firewall for Apache
- sudo apt install ufw -y
- sudo ufw enable
- sudo ufw app list
- sudo ufw allow 'Apache'

# How to Keep Apache Updated
- sudo apt update
- sudo apt upgrade
- sudo apt upgrade apache2


link: https://www.linuxcapable.com/how-to-upgrade-apache-to-latest-version-on-ubuntu-20-04/
