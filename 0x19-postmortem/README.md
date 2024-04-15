
Issue Summary:

Duration: April 14, 2024, 15:00 - April 15, 2024, 09:00 (UTC)
Impact: The web application experienced intermittent downtime and significant performance degradation, affecting approximately 60% of users. Users reported slow page loads, timeouts, and inability to access certain features.
Root Cause: A misconfiguration in the load balancer resulted in uneven distribution of traffic across backend servers, causing some servers to be overloaded while others remained underutilized.
Timeline:

Detection: April 14, 2024, 15:00 (UTC)
The issue was initially detected through monitoring alerts indicating high server response times and increased error rates.
Actions:
Engineers investigated backend servers, suspecting database issues due to increased query times.
Network team inspected network infrastructure for potential issues with connectivity.
Assumption was made that increased traffic due to a recent marketing campaign might have overwhelmed the system.
Misleading Paths:
Initially focused on database performance without considering load balancing issues.
Investigated network infrastructure extensively before realizing the issue was internal to the application.
Escalation:
Incident was escalated to the DevOps team after initial investigations failed to identify the root cause.
Resolution: April 15, 2024, 09:00 (UTC)
The misconfiguration in the load balancer was identified and corrected, ensuring even distribution of traffic across backend servers.
System performance was monitored closely to ensure stability post-resolution.
Root Cause and Resolution:

Root Cause: Misconfiguration in the load balancer settings resulted in uneven distribution of incoming traffic, causing some backend servers to become overloaded while others remained underutilized.
Resolution: The load balancer configuration was adjusted to evenly distribute incoming traffic across all backend servers. Additionally, monitoring alerts were set up to notify of any future load balancing issues.
Corrective and Preventative Measures:

Improvements/Fixes:
Regular audits of load balancer configurations to prevent similar misconfigurations in the future.
Implement automated testing of load balancer settings to ensure proper functionality.
Improve communication channels between teams to facilitate quicker escalation and resolution of issues.
Tasks:
Patch load balancer configuration to evenly distribute traffic.
Implement automated testing scripts for load balancer configurations.
Conduct training sessions for engineers on load balancer management best practices.
Review incident response procedures to streamline escalation processes.
