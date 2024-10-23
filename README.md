# automation
This project automates the security hardening of a newly provisioned Virtual 
Machine (VM) using Ansible. The playbook ensures that the VM is configured 
securely by performing several security tasks, such as creating a new admin user,
securing SSH access with public key authentication, disabling password authentication,
enabling the UFW firewall with necessary rules, and installing and configuring 
Fail2Ban to prevent brute-force attacks. These steps ensure that the VM is ready 
for secure use in production or development environments.

### Requirements:

## Versions:
- Python3: 3.10.12
- Nginx: nginx/1.18.0 (Ubuntu)
- Flask: 3.0.3
- Werkzeug 3.0.4
- Ubuntu: 22.04
- Docker: 27.3.1, build ce12230
- Docker-compose: 2.28.1
- Ansible: core 2.16.11
- jinja: 3.1.4

# How to run it

1. Install update
2. Git clone repo "Automation" to /home directory
```bash
git clone https://github.com/matusik-ops/automation.git
```
3. Rewrite all vars and inventory in automation/Ansible
```bash
cd automation/Ansible
vim inventory 
vim ... # vars
```
4. Run playbook in automation/Ansible folder "playbook.yml"
```bash
ansible-playbook -i inventory start.yml
```
