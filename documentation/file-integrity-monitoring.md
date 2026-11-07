# File Integrity Monitoring (FIM) Using OSSEC

## 1. Overview

File Integrity Monitoring (FIM) is a security mechanism used to detect changes to files and directories.

In this project, OSSEC HIDS was used to monitor a custom Linux test directory and identify changes to monitored files.

## 2. Objectives

- Detect unauthorized file modifications.
- Monitor file creation and deletion.
- Identify changes to important files.
- Generate security alerts for investigation.
- Understand file integrity monitoring in a SOC environment.

## 3. Monitoring Workflow

1. Configure a directory for monitoring in OSSEC.
2. Allow OSSEC to establish an initial file integrity baseline.
3. Create a test file.
4. Modify the test file.
5. Delete the test file.
6. Review the generated security alerts.
7. Investigate the detected changes.

## 4. Example Test Scenarios

| Test | Expected detection |
|---|---|
| Create a file | File added |
| Modify a file | File modified |
| Delete a file | File deleted |

Actual detection depends on the OSSEC configuration and monitoring schedule.

## 5. Security Relevance

FIM helps identify:
- Unauthorized configuration changes.
- Suspicious file modifications.
- Unexpected changes to critical system files.
- Potential indicators of compromise.

## 6. Alert Investigation

OSSEC alerts can be reviewed using:

sudo tail -f /var/ossec/logs/alerts/alerts.log

Relevant alerts should be investigated by checking the affected file, timestamp, user activity and surrounding system events.

## 7. Project Evidence

Add screenshots showing:
- Monitored directory configuration.
- Test file creation.
- File modification.
- OSSEC-generated alerts.

## 8. Learning Outcomes

- Understanding file integrity monitoring.
- Monitoring Linux directories.
- Analysing file change alerts.
- Investigating potential unauthorized modifications.
