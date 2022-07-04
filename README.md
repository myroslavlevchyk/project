## **Project** ##

&nbsp; &nbsp; &nbsp; In this project The CI/CD process is done by next technologies as GitHub, Jenkins, Docker container, Docker Hub, Ansible. Let’s look at construction CI/CD process with using the above tools.

&nbsp; &nbsp; &nbsp;  As soon as The developer writes and push's the program's code to GitHub - GitHub Webhook will send http-challenge to Jenkins. Whenever Jenkins gets http-challenge from GitHub it launches pipeline. First Ansible ‘s playbook - builds docker-container, puts the modified code into it and sends docker-container to Dockerhub. Then second Ansible’s playbook pulls and runs docker-container on the server. 

&nbsp; &nbsp; &nbsp; After Ansible's playbook executed - we will be able to see changes on Web-page. 

&nbsp; &nbsp; &nbsp;  Monitoring is realized with usage of Lambda AWS. As soon as The Web-page stops or server stops stakeholder will get email with error’s code.

### **Files:** ###
**Presentation**: https://github.com/myroslavlevchyk/project/blob/main/Presentation.pptx 

**Jenkinsfile**: https://github.com/myroslavlevchyk/project/blob/main/Jenkinsfile

**ansible.cfg**: https://github.com/myroslavlevchyk/project/blob/main/ansible.cfg

**hosts.txt**: https://github.com/myroslavlevchyk/project/blob/main/hosts.txt

**group_vars**: https://github.com/myroslavlevchyk/project/blob/main/PROD_SERVERS

**playbook0.yml**: https://github.com/myroslavlevchyk/project/blob/main/playbook0.yml

**playbook1.yml**: https://github.com/myroslavlevchyk/project/blob/main/playbook1.yml

**Dockerfile**: https://github.com/myroslavlevchyk/project/blob/main/Dockerfile

**index.html**: https://github.com/myroslavlevchyk/project/blob/main/index.html