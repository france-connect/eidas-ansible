# Ansible scripts for the deployment of eiDAS-node v1.1

As used for deploying test eiDAS instances at FranceConnect.

We publish it in the hope it can help get you get eiDAS-node running faster.

This is intended for use with Centos 7.2

License : EUPL

## How to use :

In roles/deploy-eidas-node/tasks/main.yml, change the tasks that download eidas-node.war, idp.war and sp.war from our local Jenkins instance to get these WARs from a place of your choice.

Deploy a Centos 7.2 machine, and add an ansible user with sudoer rights.
 
In the 'inventory' file, set ansible_host to the IP of your Centos machine.

run `ansible-playbook -i inventory install-deploy-eidas.yml -u ansible -M roles/`


