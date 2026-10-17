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

## Splunk Web is up

Got Splunk Enterprise installed again and started it under the
`splunk` service account.

Opened Splunk Web from my host and reached the login page.

### Next
- Verify the login works
- Create the `win_security` index
- Set up the Windows VM and Sysmon

## Created the Windows security index

Created the `win_security` index in Splunk to keep the Windows
security events and Sysmon telemetry for this lab in one place.

Ran a basic search to check the index. It has no events yet because
the Windows endpoint and log forwarding aren't configured.

### Next
- Create the Windows VM in VMware
- Install Sysmon
- Install the Splunk Universal Forwarder
- Forward Windows events to Splunk