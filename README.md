Ansible docker orchestration

The project provisions two local docker containers and establish ssh connection between the two:

Building the Application Locally

Before building and running the application locally, your system must have the following prerequisites installed:

Vagrant - For setting up your local env
Orcale virtualBox

Environemnt setup
Run vagrant up

role setup-ssh 
1.Creates a user docker_root in container-1
2.generates ssh keys in container-1 
3.Copies the public key of container1 to authorized_keys of container-2

role test-ssh 
1.does a simple ssh connection test from container-1 to container-2



Run
Provision containers - ansible-playbook -i inventory.yml playbook.yml

Destroy containers- ansible-playbook destroy.yml
