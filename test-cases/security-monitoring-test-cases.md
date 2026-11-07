# Security Monitoring Test Cases

## Test Case 1: SSH Authentication Monitoring

Objective:
Identify failed SSH authentication attempts.

Test procedure:
1. Generate a controlled failed SSH login attempt.
2. Review Linux authentication logs.
3. Check whether OSSEC generates a corresponding alert.
4. Record the alert details.

Expected result:
The authentication failure should be recorded in the relevant system logs. OSSEC alert generation depends on configured rules and log collection.

## Test Case 2: Sudo Activity Monitoring

Objective:
Review privileged command execution.

Test procedure:
1. Execute a permitted sudo command.
2. Review authentication logs.
3. Identify the user and executed command.
4. Check OSSEC alerts for relevant events.

Expected result:
Sudo activity should be recorded in the system authentication logs.

## Test Case 3: File Integrity Monitoring

Objective:
Detect changes to monitored files.

Test procedure:
1. Create a test file in the configured monitoring directory.
2. Modify its contents.
3. Review OSSEC alerts.
4. Record detected changes.

Expected result:
OSSEC should detect applicable file changes according to its FIM configuration and scanning schedule.

## Test Evidence

Record actual test results, timestamps, screenshots and alert details after executing each scenario.

## Conclusion

These scenarios provide a controlled method for evaluating Linux security monitoring, authentication event analysis and file integrity detection.
