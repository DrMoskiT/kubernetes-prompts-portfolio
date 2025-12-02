# Kubernetes Prompt Engineering Portfolio

This repository showcases a collection of Kubernetes YAML manifests and a portfolio of custom-designed prompts used to generate and analyze these manifests using AI tools such as Google Cloud `kubectl-ai`.  
It serves as a demonstration of practical **Prompt Engineering**, **DevOps automation skills**, and **Kubernetes expertise** for infrastructure-focused projects.

---

### **Technical Expertise**
- **Kubernetes & Containers:** k3s, k3d, Docker, Helm, ArgoCD, GKE  
- **Automation & IaC:** Terraform, Ansible, GitHub Actions, GitLab CI  
- **Monitoring & Observability:** Prometheus, Grafana, Loki, Graylog  
- **Networking:** BGP, Anycast, Ubiquiti UniFi, MikroTik, Dell S-series  
- **Security:** RBAC, IAM, Secrets Management, TLS automation, WAF/SIEM  
- **Languages:** Go, Python, Bash, PowerShell  

---

## 🎯 Purpose of This Repository

This repository fulfills a technical assignment requiring:

1. A set of Kubernetes YAML manifests based on common application deployment patterns.
2. A collection of **prompt engineering scenarios** (prompts) used to generate or improve these manifests using AI tools.
3. A demonstration of clear communication, DevOps thinking, and the ability to use AI effectively in engineering workflows.

---

## 📁 Repository Structure


```text
kubernetes-prompts-portfolio/
│
├── README.md
│
└── yaml/                     # Kubernetes YAML manifests
    ├── app.yaml
    ├── app-livenessProbe.yaml
    ├── app-readinessProbe.yaml
    ├── app-volumeMounts.yaml
    ├── app-cronjob.yaml
    ├── app-job.yaml
    ├── app-multicontainer.yaml
    ├── app-resources.yaml
    └── app-secret-env.yaml
```

---

## 🧠 Prompt Engineering Methodology

All prompts in this repository follow the principles from **Google Prompt Engineering Guide**, including:

- **Clear instructions**  
- **Explicit constraints**  
- **Grounding with relevant context**  
- **Structured output expectations**  
- **Deterministic behavior for YAML generation**  

Each prompt is purpose-built to:

- generate a Kubernetes manifest,
- modify or enhance an existing manifest,
- validate or troubleshoot a configuration,
- or enforce production-grade standards.

---

## 📦 Manifests Overview

The `manifests/` directory contains Kubernetes YAML definitions for:

- Base application Deployment + Service  
- Deployments with liveness and readiness probes  
- ConfigMap-backed volume mounts  
- CronJob and one-off Job  
- Multi-container Pod  
- Resource-constrained Deployment  
- Secret-based environment variables  

These are typical building blocks for cloud-native applications and demonstrate practical Kubernetes usage.

---

## 🧩 Prompt Portfolio

The `prompts/` directory includes fully documented prompt scenarios:

- Deployment generation  
- Probes injection  
- Resource optimization  
- Multi-container design  
- Job scheduling  
- Secret management  
- ConfigMap volume integration  

Each prompt is written to be compatible with **Google Cloud kubectl-ai**, Gemini, or any modern GenAI tool.

---

## 🚀 Usage

You can use any prompt from the `prompts/` directory by running:


—or paste the prompt directly into your preferred AI interface.

The AI will generate Kubernetes YAML based on your requirements.

---

## ⭐ Summary

This repository demonstrates:

- Real-world application of **Prompt Engineering** in DevOps  
- Ability to generate reliable Kubernetes manifests using AI  
- Understanding of Kubernetes architecture and application workflows  
- Clear and structured engineering communication  

It is prepared specifically for review as part of a technical screening request.

# Prompt Engineering Portfolio for Kubernetes

Below is a summary table of all prompts and resulting Kubernetes manifests.

| NAME                 | PROMPT | DESCRIPTION | EXAMPLE |
|---------------------|--------|-------------|----------|
| app.yaml | Generate a basic Deployment and Service for go-demo-app | Base application deployment | [app.yaml](yaml/app.yaml) |
| app-livenessProbe.yaml | Add livenessProbe to Deployment | Ensures pod restarts if unhealthy | [app-livenessProbe.yaml](yaml/app-livenessProbe.yaml) |
| app-readinessProbe.yaml | Add readinessProbe to Deployment | Ensures traffic only routed when app is ready | [app-readinessProbe.yaml](yaml/app-readinessProbe.yaml) |
| app-volumeMounts.yaml | Add ConfigMap-based volumeMount | Mounts configuration into container | [app-volumeMounts.yaml](yaml/app-volumeMounts.yaml) |
| app-cronjob.yaml | Generate a CronJob that runs every 5 minutes | Periodic background job | [app-cronjob.yaml](yaml/app-cronjob.yaml) |
| app-job.yaml | Generate a Job for one-time execution | Simple batch job | [app-job.yaml](yaml/app-job.yaml) |
| app-multicontainer.yaml | Create Pod with 2 containers sharing a volume | Demonstrates multi-container Pod design | [app-multicontainer.yaml](yaml/app-multicontainer.yaml) |
| app-resources.yaml | Add CPU & memory requests/limits | Resource control & scheduling | [app-resources.yaml](yaml/app-resources.yaml) |
| app-secret-env.yaml | Create Secret & Deployment consuming env vars | Secure configuration with secrets | [app-secret-env.yaml](yaml/app-secret-env.yaml) |



