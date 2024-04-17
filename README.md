# Capstone Project : E-Commerce Platform Deployment using Git, Linux and AWS

## Implementing Version control

* Created a project directory named MarketPeak_Peak and initialize the repository.
* Downloaded the free template and extracted the template onto the local repository.
* Staged the files in the repository
* Set Git Global configuration with username and email
* Made the first commit with the message "Initial commit with basic e-commerce site structure"
* Created a remote repository on github with the same name as my local directory 
* added the remote repository to the local repository configuration
* Pushed all the files from the local repository to the githug repository.

## Creating EC2 Instance and installing Apache Webserver

* Created an EC2 Instance on AWS and updated OS to the latest version
* Assinged elastic IP for public acces
* Cloned github repository on EC2 instance using the SSH method. (Created key pair and uploaded public key to github)
* Installed Apache Server (apache2) on Ubuntu. Although instructions carried the yum package manager had to use apt-get as EC2 instance had ubuntu installed
* Configured apache webserver for website by deleting contents of /var/www/html and copying contents of the cloned repository to the folder.
* Restarted apache2 service and accessed website from browser using public IP.

## CI/CD workflow

* Created and switched new branch (development) on local repository
* Made some changes to the index.html file.
* Commited changes and pushed changes to development branch on origin (github)
* Swithced back to main branch and and merged development branch with main.
* Push merged changes to github
* Requested pull from origin to webserver and restarted the apache2 service.
* Was able to view changes on the public site.

## README.md

This readme document was done as the deployment was carried out step by step.

