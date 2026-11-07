# OSSEC HIDS Installation and Configuration

## 1. Installation Overview

OSSEC HIDS was deployed in an Ubuntu Linux environment to provide host-based security monitoring and intrusion detection.

The installation was performed using the official OSSEC open-source project.

Official source:
https://github.com/ossec/ossec-hids

## 2. Installation Process

The general installation workflow:

1. Prepare the Ubuntu environment.
2. Install required build dependencies.
3. Obtain the OSSEC source code.
4. Navigate to the extracted OSSEC directory.
5. Execute the installation script.
6. Select the appropriate installation type.
7. Complete the installation prompts.
8. Verify the installation.

## 3. Important OSSEC Locations

| Location | Purpose |
|---|---|
| /var/ossec/ | Main OSSEC installation directory |
| /var/ossec/bin/ | OSSEC executable files |
| /var/ossec/etc/ | Configuration files |
| /var/ossec/logs/ | OSSEC logs |
| /var/ossec/logs/alerts/alerts.log | Security alerts |

## 4. Configuration Areas

The lab involved working with:

- OSSEC service configuration.
- Authentication and system log monitoring.
- File Integrity Monitoring.
- Rootkit detection.
- Security alert generation and analysis.

## 5. Verification Commands

Check OSSEC processes:

ps aux | grep ossec

Review security alerts:

sudo tail -f /var/ossec/logs/alerts/alerts.log

Inspect OSSEC installation:

sudo ls -la /var/ossec/

## 6. Security Considerations

- Monitor authentication-related events.
- Protect OSSEC configuration files.
- Review security alerts regularly.
- Avoid exposing passwords, private keys or sensitive logs.
- Use controlled testing activities when generating security events.

## 7. Documentation Status

Installation and configuration details should be updated with the actual OSSEC version, installation settings and screenshots from the lab environment.
