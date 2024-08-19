# Annual Project
This project is a part of the annual project of the 3rd year of the bachelor's degree in computer science at the school of Open IT, Montpellier. The goal is to deploy a secure alma linux server following the best practices recommended by the ANSSI.

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
ansible-playbook playbook-init.yaml -k
```
## Authors
- Antonin Royer
- Alisson Creiche
- Victor Mercier