# awx
21/12/2017
------

AWX Automated installation

Target: local machine.

Basic configuration.


HOW TO'S
-------

Change the user for the installation in defaults/main.yml : currently : brichar ( for my local installation ).
		For Installation on our Ansible Server, should change it for: ubuntu

Install ansible : apt-get install ansible

Install git : apt-get install git

Clone installation playbook : git clone https://github.com/BenoitRichard1212/awx-install

then run playbook : ansible-playbook -K awx-install/tasks/main.yml

please after the playbook has completed its tasks wait around 10 minute for the database migration of AWX to complete.

After that the web interface should be available via the server IP.

You can check installation result in : /etc/awx_playbook_complete


TO DO'S
------

Will remove SUDO password prompt.

Ajust for RD environnement, Users, settings, etc.

Lots will change as we change everything to be viable for RD'S.