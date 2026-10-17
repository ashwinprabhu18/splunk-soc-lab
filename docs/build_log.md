# Build Log

## Initial setup

Created the Ubuntu VM in VMware Workstation to run Splunk for this lab.

Checked the VM's resources and network using `free -h`, `df -h` and `ip -br address`.

- Hostname: flipperserver
- Network interface: ens33
- IP: 172.16.106.134
- RAM: 5.2 GiB total, around 4.6 GiB available
- Disk: around 29 GB free

The VM is running and looks fine for the initial setup.

### Next
- Install Splunk Enterprise
- Get Splunk Web working
- Set up the Windows VM