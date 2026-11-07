# File Integrity Monitoring - Test Results

## Test Environment
- Operating System: Ubuntu Linux
- Security Tool: OSSEC HIDS
- Monitored Directory: /opt/ossec-test
- Monitoring Mode: Real-time FIM

## Test Procedure

1. Created a test file named fim-test.txt.
2. Added initial content.
3. Modified the file by appending additional content.
4. Reviewed OSSEC alerts.log.

## Actual Results

### First Modification
- Rule ID: 550
- Severity: 7
- Alert: Integrity checksum changed
- File: /opt/ossec-test/fim-test.txt
- File size: 0 to 25 bytes

### Second Modification
- Rule ID: 551
- Severity: 7
- Alert: Integrity checksum changed again (2nd time)
- File size: 25 to 64 bytes

## Result

PASS - OSSEC successfully detected both file modifications and generated security alerts.

## Security Significance

File Integrity Monitoring helps identify unexpected changes to monitored files and supports investigation of potential unauthorized modifications.

## Evidence

Screenshots of the actual OSSEC alerts should be retained in the screenshots directory.
