# Project0
This Ansible role will install Certbot (apache2), Apache2, Python, and EC2 Instance Connect on an Ubuntu Server Image.
In addition, a generic .html page showing the contributors' team name and members will be generated and the virtual host file will be configured. 
Specifically, the responsibilities of this role are to:
- Obtain the user's GitHub repository name, username, and password through a prompt.
- Enable the Ubuntu Universal repository.
- Add the Certbot repository.
- Update all packages to the latest version.
- Install software-properties-common (allowing for easier management of the Ubuntu distribution and independent software vendor software sources), Certbot, a transitional package for the migration of certbot from Python2 to Python3, 
Ec2-instance-connect, and Apache2.  
- Clone the Project0 repository.
- Copy the Apache configuration files into place.
- Generate an OpenSSH keypair.
- Add a read only deploy key to the Github repository and authenticate using 2FA (the information obtained through the prompt).
- Clone a private GitHub repository through SSH.
- Copy the Certbot configuration files into place which enable HTTPS.
- Enable the Apache2 module rewrite workaround which provides URL manipulation capability for incoming URL requests. 
- Enable the Apache2 module ssl workaround to enable the SSL for the website. 
- Restart Apache. 

## Dependencies

- Ansible >= 2.0.
- An Ubuntu Server image >= 18.04.
- A GitHub account.

## Run

After cloning the Project0 repo and changing directory into Project0/ansible run the playbook on localhost: $ ansible-playbook project0.yml

## Installation

[Running the Ansible file in place (EC2 Server Environment) to stand up the website](https://github.com/alexcoward/Project0/wiki/Ansible-Playbook-Documentation#running-the-ansible-file-in-place-ec2-server-environment-to-stand-up-the-website)

## Contributing

Issues, feature requests, ideas are appreciated and can be posted in the Issues section.

Pull requests are also welcome. To submit a PR, first create a fork of this Github project. Then create a topic branch for the suggested change and push that branch to your own fork.

## Contributors

Alexander Coward (maintainer)

Kindra Richie