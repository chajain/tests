---
title: Create a new VM with Network Data from YAML	
---
1. Add Network Data to the VM via YAML
    - Here is an example of Network Data config to add DHCP to the physical interface eth0
        ```
        network:
        version: 1
        config:
        - type: physical
            name: eth0
            subnets:
            - type: dhcp
        ```
1. Save/Create the VM

## Expected Results
1. Machine starts succesfully
1. Network Data should show in YAML
1. Network Datashould show in Form
1. Machine should have DHCP for network on eth0