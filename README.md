# CI/CD Pipeline for Kubernetes Deployment and Testing of 5G Core

## 📌 Overview  
This project demonstrates an automated CI/CD pipeline for deploying and testing a 5G Core network. It integrates Open5GS for the core network, UERANSIM for UE simulation, Docker for containerization, Kubernetes for orchestration, and GitHub Actions for automation.

---

## 🛠️ Technologies Used  
- Open5GS (5G Core Network)  
- UERANSIM (UE and gNB Simulation)  
- Docker  
- Kubernetes (Minikube)  
- GitHub Actions (CI/CD Pipeline)  

---

## ⚙️ Installation Summary  
The setup involves installing Docker, Kubernetes (Minikube), Open5GS, and UERANSIM. After installation, the system is configured so that Docker images can be used inside Kubernetes.

---

## 📁 Project Structure  
- Dockerfile for building the Open5GS image  
- Kubernetes configuration files for deployment and service  
- Scripts for deployment, testing, and cleanup  
- GitHub workflow file for CI/CD automation  

---

## 📁 Project Structure

project/
├── Dockerfile  
├── k8s/  
│   ├── deployment.yaml  
│   └── service.yaml  
├── scripts/  
│   ├── deploy.sh  
│   ├── test.sh  
│   └── cleanup.sh  
└── .github/workflows/  
    └── cicd.yml  

---

## 🚀 Deployment Process  
1. Build the Docker image for Open5GS  
2. Deploy the application to Kubernetes  
3. Verify deployment status  
4. Expose services for communication  

---

## 🧪 Testing Process  
- A UE (User Equipment) connects to the 5G Core  
- Registration and session establishment logs are checked  
- Based on logs, the system outputs PASS or FAIL  

---

## 🔁 CI/CD Pipeline  
The CI/CD pipeline is triggered automatically on every push to the repository. It performs:  
- Code checkout  
- Docker image build  
- Kubernetes deployment  
- Execution of test scripts  
- Validation of results  

---

## 🔥 Multiple UE Testing  
- Multiple UEs are launched simultaneously  
- Each UE attempts to connect to the 5G Core  
- Logs are analyzed to verify successful connections  
- The system reports PASS if all UEs connect successfully  

---

## 🎯 Workflow Summary  
1. Build Docker image  
2. Deploy to Kubernetes  
3. Run UE simulation  
4. Analyze logs  
5. Return PASS or FAIL  

---

## ⚠️ Common Issues  
- Pod not running → Check Kubernetes deployment status  
- UE not connecting → Verify UERANSIM configuration and subscriber data  
- Image not found → Ensure Docker is correctly configured with Kubernetes  

---

## ✅ Final Outcome  
- Automated deployment of 5G Core  
- Kubernetes-based orchestration  
- Real-time UE testing  
- CI/CD pipeline automation  
- Support for multiple user simulation  

---

## 👨‍💻 Author  
**Nandan M S**
