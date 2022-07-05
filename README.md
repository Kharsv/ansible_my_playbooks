# ansible_my_playbooks <br/>
This is a simple Ansible torial with some playbook.yml example. <br/>
<br/>
There is 4 playbooks withs simle tasks<br/>
run with:<br/>
#ansible-playbook playbook.yml --extra_vars ansible_sudo_pass="mypass"   <br/>
1 Ping<br/>
2 Install apache<br/>
3 Install packeges and restart<br/>
file first_playbook  - install jenkins<br/>
<br/>
Set up.<br/>
Install Fedora...<br/>
1. Install ansible. <br/>
sudo dnf update <br/>
sudo dnf install ansible <br/>
sudo dnf upgrade ansible <br/>
 <br/>
1.1 Check. <br/>
sudo dnf update <br/>
dnf search ansible <br/>
dnf info ansible <br/>
  <br/>
2. Install Jenkins <br/> <br/>
sudo wget -O /etc/yum.repos.d/jenkins.repo https://pkg.jenkins.io/redhat/jenkins.repo <br/>
sudo rpm --import https://pkg.jenkins.io/redhat/jenkins.io.key <br/>
sudo dnf upgrade <br/> <br/>
# Add required dependencies for the jenkins package <br/>
sudo dnf install java-11-openjdk <br/>
sudo dnf install jenkins <br/>
jenskin <br/>
3. Start Jenkins <br/> <br/>
sudo systemctl enable jenkins <br/>
sudo systemctl start jenkins <br/>
sudo systemctl status jenkins <br/>
4. Go to localhost:8080 <br/>
