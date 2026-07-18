# Azure Standard Load Balancer

## Overview

This project demonstrates the deployment and configuration of an Azure Standard Load Balancer to distribute HTTP traffic across two Ubuntu Linux virtual machines running Nginx. A frontend public IP, backend pool, HTTP health probe and load balancing rule were configured to provide high availability and automatic traffic distribution. Nginx was installed on both virtual machines, and traffic distribution was verified using a web browser and PowerShell `curl` commands.

---

## Architecture

```text
                Internet
                    │
                    ▼
      Azure Standard Load Balancer
                    │
        ┌───────────┴───────────┐
        │                       │
        ▼                       ▼
vm-cloud-labs-linux-001   vm-cloud-labs-linux-002
       Nginx                    Nginx
```

---

## Screenshots

### Review and Create

Shows the Azure configuration before deploying the Standard Load Balancer.

![Review and Create](screenshots/azure-load-balancer-01-review-and-create.png)

---

### Deployment Successful

Shows the successful deployment of the Azure Standard Load Balancer.

![Deployment Successful](screenshots/azure-load-balancer-02-deployment-success.png)

---

### Load Balancer Overview

Shows the deployed load balancer and its frontend configuration.

![Load Balancer Overview](screenshots/azure-load-balancer-03-load-balancer-overview.png)

---

### Backend Pool

Shows both Ubuntu Linux virtual machines added to the backend pool.

![Backend Pool](screenshots/azure-load-balancer-04-backend-pool.png)

---

### Health Probe

Shows the HTTP health probe configured to monitor the availability of the backend virtual machines.

![Health Probe](screenshots/azure-load-balancer-05-health-probe-created.png)

---

### Load Balancing Rule

Shows the HTTP load balancing rule linking the frontend IP, backend pool and health probe.

![Load Balancing Rule](screenshots/azure-load-balancer-06-load-balancing-rule.png)

---

### Health Probe Status

Shows both backend virtual machines reporting a healthy status.

![Health Probe Status](screenshots/azure-load-balancer-07-load-bala-health-probe-status.png)

---

### Load Balancing Rule Verification

Shows the completed load balancing rule configuration.

![Load Balancing Rule Verification](screenshots/azure-load-balancer-08-load-bal-rule.png)

---

### PowerShell Verification

Shows HTTP requests distributed between both backend virtual machines using PowerShell `curl`.

![PowerShell Verification](screenshots/azure-load-balancer-09-powershell-curl.png)

---

### Browser Verification – VM002

Shows the load balancer routing traffic to **vm-cloud-labs-linux-002**.

![Browser Verification - VM002](screenshots/azure-load-balancer-10-webpage-vm2-shown.png)

---

### Browser Verification – VM001

Shows the load balancer routing traffic to **vm-cloud-labs-linux-001**.

![Browser Verification - VM001](screenshots/azure-load-balancer-11-webpage-vm1-shown.png)