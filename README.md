Ansible docker orchestration

playbook.yml starts two ubuntu based containers and destroy.yml, destroys the same containers.

role setup-ssh 
1.Creates a user docker_root in container-1
2.generates ssh keys in container-1 
3.Copies the public key of container1 to authorized_keys of container-2

role test-ssh 
1.does a simple ssh connection test from container-1 to container-2