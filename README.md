# JENKINS-> ANSIBLE CHALLENGE

Setup / configure a Jenkins instance on AWS
You already have you Ansible agent running and a EC2 machine that you can configure for Jenkins (Rename from JSHost to JenkinsHost)

You will need to have a GitHub repo with the following files:

- jenkins-config.yml
- inventory.txt
- README.md

Deliverables:

- Playbook for Jenkins
- To configure a Jenkins instance on AWS (Provide IP Address)
- Detailed README.md on how to use your Playbook.
- Screen recording of you playbook running and Jenkins working.

---

## Demo

### Installing Jenkins Using Ansible Playbook

![](jenkins-instance.gif)

---

### Post-installation Jenkins Setup

![](running-playbook.gif)

---

### Notes

#### Inventory.text

Specifies the host(s) for Ansible to manage.

#### jenkins-config.yml

The package cache is updated to ensure the latest packages are available. To secure the installation, a key file is imported from jenkins-ci. The jenkins repository is then added to the remote host. OpenJDK 11 is installed followed by Jenkins. Jenkins service is started to complete the setup process.
