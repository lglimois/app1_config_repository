# app1_config_repository
Objectif:
  demo pour ansible via Jenkins

# Prerequis
* ssh-keygen
* ssh-copy-id demo@SERVER_IP_ADDRESS
* cat ~/.ssh/id_rsa.pub
* vi .ssh/authorized_keys
* insert

# Site d'exemple

 https://www.infoq.com/fr/presentations/ansible-jean-christophe-sirot-ansible-et-jenkins

## Les exemples du speeker:
https://github.com/jcsirot/ansible-meetup

## Best practise
  http://docs.ansible.com/ansible/latest/playbooks_best_practices.html#content-organization
  montre l'arborescence et alternative, la structure utilisée dans differents projets avec les group_vars

## syntaxe avec les var dans l'inventory
  http://docs.ansible.com/ansible/latest/intro_inventory.html#group-variables
  ansible_host
  
## Tuto ansible
Deploiement d'un war dans un tomcat

  http://aseigneurin.github.io/2014/11/04/ansible-pour-deployer-des-applications.html

  https://github.com/aseigneurin/ansible-sandbox

##Exemple de playbook
  https://github.com/ansible/ansible-examples

##Tester l'existence de variable:
  - assert:
    that:
      - "my_param <= 100"
      - "my_param >= 0"
    msg: "'my_param' must be between 0 and 100"
    
   - fail: msg="Bailing out. this play requires 'bar'"
      when: bar is undefined
  
