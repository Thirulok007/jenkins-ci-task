# Jenkins CI/CD Pipeline Project

## 📌 Project Overview
This project demonstrates a simple Continuous Integration (CI) pipeline using Jenkins, GitHub, and AWS EC2.  
Whenever code is pushed to GitHub, Jenkins automatically pulls the code and executes the build process on an EC2 instance.

---

## ⚙️ Technologies Used
- AWS EC2 (Amazon Linux)
- Jenkins (CI Tool)
- Git & GitHub (Version Control System)
- Linux Commands
- Shell Scripting (Bash)

---

## 🚀 Project Setup Steps

### 1. AWS EC2 Setup
- Created an EC2 instance in AWS Cloud
- Connected to the instance using SSH

---

### 2. Jenkins Installation
- Installed Jenkins on EC2 instance
- Installed Java (Amazon Corretto 17)
- Started Jenkins service using systemctl
- Accessed Jenkins using browser:


http://<EC2-PUBLIC-IP>:8080


---

### 3. Git Installation
Installed Git on EC2:

```bash
sudo dnf install git -y

Verified Git installation:

git --version
4. GitHub Repository Setup
Created a GitHub repository named: jenkins-ci-task
Added a shell script file: hello.sh
hello.sh content:
#!/bin/bash

echo "Jenkins CI Test"
echo "Build Successful"
date
5. Jenkins Job Configuration
Created a Freestyle project in Jenkins: jenkins-task2
Configured GitHub repository:
https://github.com/Thirulok007/jenkins-ci-task.git
Selected branch:
main
6. Build Configuration

Added build step in Jenkins:

chmod +x hello.sh
./hello.sh
7. Build Execution
Triggered build manually using “Build Now”
Jenkins fetched code from GitHub repository
Executed the shell script successfully
📤 Output
Jenkins CI Test
Build Successful
<Current Date Output>
🎯 Result
Jenkins successfully integrated with GitHub
Code is automatically fetched from repository
Build executed successfully on AWS EC2 instance
CI pipeline is working properly
📸 Screenshots Included
AWS EC2 instance running
Jenkins dashboard
Job configuration page
GitHub repository
Successful build output
Console output log
🏁 Conclusion

This project successfully demonstrates a basic CI/CD pipeline using Jenkins, GitHub, and AWS EC2. It helps automate the build process whenever code is pushed to the repository.
