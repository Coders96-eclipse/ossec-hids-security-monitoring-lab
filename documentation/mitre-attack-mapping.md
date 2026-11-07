# MITRE ATT&CK Mapping

## Overview

This document maps selected Linux security monitoring scenarios to the MITRE ATT&CK framework.

Reference: https://attack.mitre.org/

## Technique Mapping

| Security Activity | MITRE Technique | ID |
|---|---|---|
| Brute Force attempts against SSH | Brute Force | T1110 |
| Abuse of sudo privileges | Abuse Elevation Control Mechanism | T1548.003 |
| Suspicious file modification | File and Directory Permissions Modification | T1222 |
| Rootkit-related activity | Rootkit | T1014 |
| SSH remote access | SSH | T1021.004 |

## Detection Opportunities

### 1. SSH Authentication Attacks
Monitor repeated failed authentication attempts and investigate unusual login patterns.

### 2. Sudo Privilege Abuse
Review privileged command execution and investigate unexpected privilege escalation activity.

### 3. File Integrity Changes
Monitor sensitive files and investigate unexpected modifications.

### 4. Rootkit Indicators
Review rootkit detection results and investigate suspicious system modifications.

## Important Notes

These mappings represent potential relationships between monitoring scenarios and ATT&CK techniques.

A technique should only be reported as detected when actual telemetry and investigation evidence support that conclusion.

## Reference

MITRE ATT&CK Enterprise:
https://attack.mitre.org/
