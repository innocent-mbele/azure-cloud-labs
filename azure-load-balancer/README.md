# Project 04 - Azure Standard Load Balancer

## Overview

This project demonstrates the deployment and configuration of an Azure Standard Load Balancer to distribute HTTP traffic across two Ubuntu Linux virtual machines running Nginx. A backend pool, health probe and load balancing rule were configured to provide high availability and automatic traffic distribution.

---

## Configuration Completed

- Deployed Azure Standard Load Balancer
- Configured Frontend Public IP
- Created Backend Pool
- Added two Ubuntu virtual machines
- Configured HTTP Health Probe
- Created HTTP Load Balancing Rule
- Installed and configured Nginx on both virtual machines
- Verified backend health
- Verified load balancing between both servers

---

## Architecture

```
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

- Both virtual machines are healthy.
- Health probe reports 100% healthy instances.
- HTTP requests are successfully distributed across both backend servers.
- Traffic distribution verified using browser refreshes and PowerShell `curl` commands.

---

## Screenshots

- Review and Create
- Deployment Successful
- Load Balancer Overview
- Backend Pool
- Health Probe
- Load Balancing Rule
- Health Probe (100% Healthy)
- Browser showing VM001
- Browser showing VM002
- PowerShell Load Balancing Verification