# Azure Network Security Group

Created and configured an Azure Network Security Group (NSG) to control inbound traffic.

## Deployment

| Resource | Name |
|----------|------|
| Network Security Group | nsg-cloud-labs-dev-001 |
| Inbound Rule | Allow SSH (22) |
| Inbound Rule | Allow HTTP (80) |

## Screenshots

### 1. NSG created
![NSG Created](screenshots/01-nsg-created.png)

### 2. NSG overview
![NSG Overview](screenshots/02-nsg-overview.png)

### 3. Default security rules
![Default Rules](screenshots/03-nsg-default-rules.png)

### 4. Creating HTTP rule
![Create HTTP Rule](screenshots/04-add-http-rule.png)

### 5. HTTP rule added
![HTTP Rule Added](screenshots/05-http-rule-added.png)

### 6. Associating NSG with subnet
![Subnet Association](screenshots/06-subnet-association.png)

### 7. NSG association overview
![Association Overview](screenshots/07-nsg-associated-overview.png)

### 8. Subnet protected by NSG
![Subnet with NSG](screenshots/08-subnet-with-nsg.png)