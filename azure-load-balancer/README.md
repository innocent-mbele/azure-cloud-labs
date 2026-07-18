# Project 04 - Azure Standard Load Balancer

## Overview

This project demonstrates the deployment and configuration of an Azure Standard Load Balancer to distribute HTTP traffic across two Ubuntu Linux virtual machines running Nginx. A backend pool, health probe and load balancing rule were configured to provide high availability and automatic traffic distribution.

---

## Configuration Completed

- Deployed Azure Standard Load Balancer
- Configured a Frontend Public IP
- Created a Backend Pool
- Added two Ubuntu Linux virtual machines
- Configured an HTTP Health Probe
- Created an HTTP Load Balancing Rule
- Installed and configured Nginx on both virtual machines
- Verified backend health
- Confirmed traffic distribution across both servers

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

## Verification

- Both backend virtual machines reported healthy.
- Health probe reached 100% healthy status.
- HTTP requests were successfully distributed across both virtual machines.
- Load balancing was verified using a web browser and PowerShell `curl` commands.

---

## Screenshots

### Review and Create

![Review and Create](screenshots/azure-load-balancer-01-review-and-create.png)

---

### Deployment Successful

![Deployment Successful](screenshots/azure-load-balancer-02-deployment-success.png)

---

### Load Balancer Overview

![Load Balancer Overview](screenshots/azure-load-balancer-03-load-balancer-overview.png)

---

### Backend Pool

![Backend Pool](screenshots/azure-load-balancer-04-backend-pool.png)

---

### Health Probe

![Health Probe](screenshots/azure-load-balancer-05-health-probe.png)

---

### Load Balancing Rule

![Load Balancing Rule](screenshots/azure-load-balancer-06-load-balancing-rule.png)

---

### Health Probe - 100% Healthy

![Health Probe 100% Healthy](screenshots/azure-load-balancer-07-load-balancer-health-probe-100.png)

---

### Load Balancing Rule Verification

![Load Balancing Rule Verification](screenshots/azure-load-balancer-08-load-bal-rule.png)

---

### PowerShell Verification

![PowerShell Verification](screenshots/azure-load-balancer-09-powershell-curl.png)

---

### Browser Verification - VM002

![Browser Verification - VM002](screenshots/azure-load-balancer-10-webpage-vm2-shown.png)

---

### Browser Verification - VM001

![Browser Verification - VM001](screenshots/azure-load-balancer-11-webpage-vm1-shown.png)