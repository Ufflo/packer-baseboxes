# packer-baseboxes
Packer-built baseboxes

## Software versions
Verified software versions for build components
- Hyper-V (Windows 10, 10.0.18363.693)
- Packer 1.5.4

## Execution
Exmaple: Building Ubuntu Server 18.04.3 artifact with default values
```bash
packer build ubuntu-server-18.04.3.json
```

## Known Bugs
- When running under Hyper-V:
    - Sometimes the generated VM gets the same IP as the host, causing inability to communicate between them. 
      When troubleshooting network related issues, first make sure that the host and guest have unique IP addresses and can reach eachother.