# ansible-playbooks
Ansible Cloudforms Demo for Ansible Meetup

 Pull Ansible playbook in Galaxy
   ansible-galaxy install -p roles/ bennojoy.ntp

 Add to play.yml role

 - hosts: all
  vars:
    motd_message: "Welcome to {{ ansible_hostname }}"
  roles:
    - kbrebanov.motd
    - bennojoy.ntp

 Push to Github
 git add *
 git commit -a -m "added ntp from galaxy"
 git push origin master

 Refresh CF Cloudforms Repository

 Order from Service catalog
	
