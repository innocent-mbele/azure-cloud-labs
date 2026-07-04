# Azure Network Security Group (NSG)

Configure an NSG and associate it with a subnet.

## Quick Notes

- NSGs filter inbound and outbound traffic.
- Lower priority number = higher priority.
- First matching rule is applied.
- Can be attached to a subnet or NIC.
- Default rules remain unless overridden.

## Screenshots

### NSG Created
![NSG Created](screenshots/01-nsg-created.png)

### NSG Overview
![NSG Overview](screenshots/02-nsg-overview.png)

### Default Rules
![Default Rules](screenshots/03-nsg-default-rules.png)

### HTTP Rule
![HTTP Rule](screenshots/05-http-rule-added.png)

### NSG Association
![Association](screenshots/08-subnet-with-nsg.png)