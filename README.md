# automation
for project: Project_myweb/automation

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
