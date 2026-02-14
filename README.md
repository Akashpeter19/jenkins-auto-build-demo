# Jenkins Auto Build Demo 🚀

## 📌 Overview

This project demonstrates a simple Continuous Integration (CI) pipeline using Jenkins and GitHub.

The pipeline automatically:

- Pulls source code from GitHub
- Executes a shell script (`hello.sh`)
- Sends email notification after build success/failure

---

## 🏗️ Infrastructure Setup

- AWS EC2 (Ubuntu 22.04)
- OpenJDK 17 installed
- Jenkins installed as system service
- Port 8080 enabled in EC2 Security Group

---

## 🔄 CI Pipeline Flow

1. Jenkins connects to GitHub repository.
2. It reads the `Jenkinsfile`.
3. Executes `hello.sh`.
4. Sends email notification using Gmail SMTP.
5. Build status marked SUCCESS.

---

## 📂 Project Structure

jenkins-auto-build-demo/
│
├── Jenkinsfile
├── hello.sh
├── screenshots/
└── README.md


---

## 📸 Screenshots

The `screenshots/` folder contains:

- Jenkins Dashboard (Build Success)
- Console Output
- Pipeline Configuration
- Email Configuration

---

## ✅ Result

✔ Git integration successful  
✔ Pipeline executed successfully  
✔ Email notification configured  
✔ CI automation completed  

---

## 🎯 Learning Outcome

This task helped understand:

- Jenkins installation on EC2
- Managing Linux services
- Git & SCM integration
- Writing declarative pipeline
- Troubleshooting GPG & SMTP issues
- Implementing end-to-end CI pipeline

---

**Task Status: COMPLETED ✅**

