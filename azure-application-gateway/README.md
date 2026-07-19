# Azure Application Gateway

## Overview

This project demonstrates the deployment and configuration of an Azure Application Gateway to distribute HTTP traffic across two Linux virtual machines running Nginx. The project covers subnet creation, frontend configuration, backend pools, routing rules, validation, deployment and end-to-end load balancing verification.

---

## Architecture

```
                 Internet
                      │
                      ▼
        Azure Application Gateway
                      │
          ┌───────────┴───────────┐
          │                       │
          ▼                       ▼
 Linux Virtual Machine 1   Linux Virtual Machine 2
        (Nginx)                  (Nginx)
```

---

# Screenshots

### Create Application Gateway Subnet

Shows the dedicated subnet created for the Azure Application Gateway.

![](screenshots/azure-application-gateway-01-create-subnet.png)

---

### Subnet Created

Shows the successfully created Application Gateway subnet.

![](screenshots/azure-application-gateway-02-subnet-created.png)

---

### Configure Basic Settings

Shows the basic configuration of the Azure Application Gateway.

![](screenshots/azure-application-gateway-03-basics.png)

---

### Configure Frontend Public IP

Shows the frontend public IP configuration.

![](screenshots/azure-application-gateway-04-frontend-public-ip.png)

---

### Configure Backend Pool

Shows both Linux virtual machines added to the backend pool.

![](screenshots/azure-application-gateway-05-backend-pool.png)

---

### Configure Routing

Shows the routing configuration.

![](screenshots/azure-application-gateway-06-routing-configuration.png)

---

### Configure HTTP Listener

Shows the HTTP listener configuration.

![](screenshots/azure-application-gateway-07-routing-rule-listener.png)

---

### Configure Backend Settings

Shows the backend HTTP settings associated with the routing rule.

![](screenshots/azure-application-gateway-08-routing-rule-backend.png)

---

### Configure Routing Rule

Shows the completed routing rule connecting the listener and backend pool.

![](screenshots/azure-application-gateway-09-routing-rule-created.png)

---

### Validation Passed

Shows Azure successfully validating the deployment configuration before deployment.

![](screenshots/azure-application-gateway-10-validation-passed.png)

---

### Deployment Success

Shows the successful deployment of the Azure Application Gateway.

![](screenshots/azure-application-gateway-11-deployment-success.png)

---

### Backend Pool Associated

Shows the Application Gateway successfully routing traffic to the backend pool containing both Linux virtual machines.

![](screenshots/azure-application-gateway-12-backend-pool-associated.png)

---

## Demonstration Video

This demonstration shows the Azure Application Gateway successfully distributing HTTP traffic between two Linux virtual machines running Nginx. Refreshing the browser confirms end-to-end Layer 7 load balancing by alternating requests between Backend Server 1 (VM1) and Backend Server 2 (VM2).

▶️ **[Watch the demonstration on YouTube](https://youtu.be/zt_IU6-aZz0)**

Or click the image below:

[![Azure Application Gateway Demo](screenshots/azure-application-gateway-12-backend-pool-associated.png)](https://youtu.be/zt_IU6-aZz0)

---

# Project Outcome

- Successfully deployed an Azure Application Gateway.
- Configured a dedicated Application Gateway subnet.
- Configured a frontend public IP.
- Added two Linux virtual machines to the backend pool.
- Configured backend settings and HTTP listener.
- Created routing rules for incoming HTTP traffic.
- Successfully validated and deployed the Application Gateway.
- Verified end-to-end Layer 7 load balancing through live traffic distribution between both backend servers.