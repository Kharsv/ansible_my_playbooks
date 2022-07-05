# ansible_my_playbooks
This is a simple Ansible torial with some playbook.yml example. 

1. Install ansible. Fedora.
sudo dnf update
sudo dnf install ansible
sudo dnf upgrade ansible
1.1 Check.
sudo dnf update
dnf search ansible
dnf info ansible
 
2. Install Jenkins
sudo wget -O /etc/yum.repos.d/jenkins.repo https://pkg.jenkins.io/redhat/jenkins.repo
sudo rpm --import https://pkg.jenkins.io/redhat/jenkins.io.key
sudo dnf upgrade
# Add required dependencies for the jenkins package
sudo dnf install java-11-openjdk
sudo dnf install jenkins
jenskin
3. Start Jenkins
sudo systemctl enable jenkins
sudo systemctl start jenkins
sudo systemctl status jenkins
4. Go to localhost:8080
