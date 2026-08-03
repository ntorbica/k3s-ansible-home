 # create vms
 ANSIBLE_STDOUT_CALLBACK=yaml ansible-playbook -u root ./vm-deployment.yaml --diff -vv --ask-become-pass

 # destroy vms
 ANSIBLE_STDOUT_CALLBACK=yaml ansible-playbook -u root ./vm-destroy.yaml --diff -vv --ask-become-pass
 