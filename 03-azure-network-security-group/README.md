# Azure Network Security Group

## Overview

This project demonstrates the creation and configuration of an Azure Network Security Group (NSG) to control inbound network traffic. Security rules were configured to allow SSH (port 22) for remote administration and HTTP (port 80) for web traffic. The NSG was then associated with the virtual network subnet to protect the deployed resources.

---

## Screenshots

### NSG Created

Shows the successful deployment of the Azure Network Security Group.

![NSG Created](screenshots/01-nsg-created.png)

---

### NSG Overview

Shows the Network Security Group properties and configuration after deployment.

![NSG Overview](screenshots/02-nsg-overview.png)

---

### Default Security Rules

Shows the default inbound and outbound security rules created with the NSG.

![Default Rules](screenshots/03-nsg-default-rules.png)

---

### Creating HTTP Rule

Shows the configuration of the inbound HTTP rule to allow web traffic on port 80.

![Create HTTP Rule](screenshots/04-add-http-rule.png)

---

### HTTP Rule Added

Shows the completed HTTP inbound rule successfully added to the Network Security Group.

![HTTP Rule Added](screenshots/05-http-rule-added.png)

---

### Associating NSG with Subnet

Shows the Network Security Group being associated with the virtual network subnet.

![Subnet Association](screenshots/06-subnet-association.png)

---

### NSG Association Overview

Shows the Network Security Group successfully associated with the subnet.

![Association Overview](screenshots/07-nsg-associated-overview.png)

---

### Subnet Protected by NSG

Shows the subnet protected by the associated Network Security Group.

![Subnet with NSG](screenshots/08-subnet-with-nsg.png)