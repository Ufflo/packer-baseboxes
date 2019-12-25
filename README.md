# packer-baseboxes
Packer-built baseboxes

## Software versions
Verified software versions for build components
- Hyper-V (Windows 10, 10.0.18363.535)
- Packer 1.5.1

## Known Bugs
- When running under Hyper-V:
    - Sometimes the generated VM gets the same IP as the host, causing inability to communicate between them. 
      When troubleshooting network related issues, first make sure that the host and guest have unique IP addresses and can reach eachother.