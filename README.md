# Splunk SOC Lab

I'm building a local SOC lab to learn more about SIEM monitoring,
detection engineering and incident response.

The goal is to collect endpoint logs, investigate suspicious activity,
write and test detection searches, and document what I find.

## Lab environment

- Host: Arch Linux
- Virtualisation: VMware Workstation
- SIEM: Splunk Enterprise (planned)
- Endpoint: Windows VM (planned)
- Endpoint telemetry: Windows Event Logs and Sysmon
- Log collection: Splunk Universal Forwarder
- Detection mapping: MITRE ATT&CK

## Planned detections

1. Repeated failed logins
2. Suspicious PowerShell execution
3. Unusual authentication patterns

Each detection will include its search logic, test procedure, observed results and investigation notes.

## Project structure

- `docs/` - Environment notes, build log and troubleshooting
- `detections/` - Detection searches and test results
- `investigations/` - Investigation notes and timelines
- `reports/` - Incident reports and analyst handovers
- `screenshots/` - Evidence captured from the lab
- `sample-logs/` - Sanitized sample data, where appropriate
- `scripts/` - Lab setup and testing scripts

## Current progress

- [x] Ubuntu VM booted and basic resources checked
- [ ] Splunk installed and accessible
- [ ] Windows VM created
- [ ] Sysmon installed and verified
- [ ] Windows logs arriving in Splunk
- [ ] Three detections tested
- [ ] Incident reports completed
- [ ] Final screenshots and investigation evidence added

## Scope

This is a local learning lab using controlled test activity. Detection results will be documented according to what I can actually reproduce and verify.

No real company logs, credentials or sensitive data will be published.

## Lessons learned

I'll update this section as I work through the setup, troubleshoot issues and test the detections.