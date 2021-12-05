# Install Testrail Using Ansible #

Ansible Playbook for installing [Testrail](https://www.gurock.com/testrail) 

Manual installation at [Testrail Docs Page](https://www.gurock.com/testrail/docs/admin/installation/unix) 

## First Install Ansible ##
```bash
sudo apt-get install software-properties-common
sudo apt-add-repository ppa:ansible/ansible
sudo apt-get update
sudo apt-get install ansible
```

## Then run the Ansible Playbook ##
```bash
ansible-playbook local.yaml -K
```

## Notes #
To use for remote deployment do the following: 
- delete  `connection: local` in `local.yaml`
- edit the `hosts` file to add your remote server
