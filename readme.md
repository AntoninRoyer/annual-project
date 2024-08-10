## Installation
clone the repository:
```bash
git clone https://github.com/AntoninRoyer/annual-project.git
```

Go to the ansible-peertube directory:
```bash
cd annual-project
```
Put the ip address of the client VM in the inventory file ```hosts.ini.local``` (`host.ini` is template file):
```config
[alma]
alma_host ansible_host=<ip_address>
```

Run the playbook init and enter the password of the ansible user of the client VM when prompted:
```bash
ansible-playbook playbook-init.yml -k
```