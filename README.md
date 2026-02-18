# Jenkins Auto Build Demo 🚀

## 📌 Overview

This project demonstrates a fully automated Continuous Integration (CI) pipeline using Jenkins, GitHub, and AWS EC2.

The pipeline automatically:

- Pulls source code from GitHub
- Triggers build automatically on every commit (via GitHub Webhook)
- Executes a shell script (`hello.sh`)
- Sends email notification after build success/failure

---

## 🏗️ Infrastructure Setup

- AWS EC2 (Ubuntu 22.04)
- OpenJDK 17 installed
- Jenkins installed as system service
- Port 8080 enabled in EC2 Security Group
- GitHub Webhook configured for automatic triggering

---

## 🔄 CI Pipeline Flow (Fully Automated)

1. Developer pushes code to GitHub.
2. GitHub Webhook sends event to Jenkins.
3. Jenkins automatically triggers the pipeline.
4. Jenkins pulls the latest commit.
5. Executes `hello.sh`.
6. Sends email notification using Gmail SMTP.
7. Build status marked SUCCESS/FAILURE.

---

## ⚙️ Webhook Configuration

- Payload URL:
  http://13.233.107.226:8080/github-webhook/

- Content Type: `application/json`
- Trigger Event: Push Event
- Jenkins Build Trigger: GitHub hook trigger for GITScm polling

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

- Jenkins Dashboard (Auto Triggered Build)
- Console Output
- Pipeline Configuration
- GitHub Webhook Configuration
- Email Notification Received

---

## ✅ Final Result

✔ GitHub Repository Connected  
✔ Webhook Configured Successfully  
✔ Automatic Build Trigger on Commit  
✔ Email Notification Configured  
✔ End-to-End CI Pipeline Implemented

---

## 🎯 Learning Outcome

This task helped understand:

- Jenkins installation on AWS EC2
- Linux service management
- Git & SCM integration
- GitHub Webhook configuration
- Writing declarative pipelines
- Email notification setup via SMTP
- Implementing real Continuous Integration (CI)

---

**Task Status: COMPLETED – Fully Automated CI Implemented ✅**
Trigger after URL fix
Shared lib retest
