
# OSSEC HIDS Lab Architecture

## 1. Overview
This project uses OSSEC HIDS to monitor a Linux endpoint for suspicious activities, authentication events, unauthorized file modifications, and potential security threats.

## 2. Lab Environment
- Operating System: Ubuntu Linux
- Monitoring Solution: OSSEC HIDS
- Deployment: Single-machine home lab
- Monitoring Type: Host-based intrusion detection

## 3. Architecture

The OSSEC installation operates on the Ubuntu endpoint and collects relevant system and security events.

Main components:
- Log Monitoring: Analyses system and authentication logs.
- File Integrity Monitoring (FIM): Detects changes to monitored files and directories.
- Rootkit Detection: Checks for indicators associated with rootkits.
- Alert Analysis: Records and supports investigation of detected security events.

## 4. Monitoring Workflow

1. Linux generates system and authentication events.
2. OSSEC collects events from configured log sources.
3. Detection rules analyse relevant activity.
4. Security alerts are generated when configured conditions match.
5. The analyst reviews alerts and investigates suspicious activity.

## 5. Security Testing

Planned and documented lab exercises include:
- Monitoring SSH authentication events.
- Reviewing sudo activity.
- Testing file creation and modification detection.
- Reviewing OSSEC security alerts.
- Investigating relevant events.

## 6. Learning Outcomes

- Linux security monitoring
- Host-based intrusion detection
- File Integrity Monitoring
- Log analysis
- Security alert investigation
- Basic incident response
