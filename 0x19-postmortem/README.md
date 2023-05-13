Expired SSL Certificate Postmortem

Issue Summary: Duration: May 10, 2023, from 2:00 AM to 4:30 AM WAT Impact: The login and registration service was down, restricting all users attempting to create new accounts or log into existing ones. Root Cause: An expired SSL certificate was not renewed, leading to the service becoming unavailable.

Timeline:

•	2:00 AM: The issue was detected by an automated monitoring system that flagged the login and registration service as unavailable.

•	2:02 AM: The on-call engineer was paged and began investigating the issue.

•	2:05 AM: Initial investigation revealed that the service was inaccessible due to an SSL certificate error.

•	2:10 AM: The team assumed that the SSL certificate had not been installed correctly and began to investigate that as the root cause.

•	2:20 AM: After investigating the SSL certificate installation, the team realized that the certificate had expired and was not renewed.

•	2:30 AM: The team escalated the incident to the senior engineers for additional support.

•	3:00 AM: The senior engineers identified the root cause and began working on a solution.

•	4:00 AM: The new SSL certificate was obtained and installed on the server.

•	4:15 AM: The login and registration service was successfully restored, and all users were able to access the service.

•	4:30 AM: The incident was officially declared resolved.


Root Cause and Resolution: The root cause of the issue was an expired SSL certificate that was not renewed, causing the login and registration service to become unavailable

. The solution was to obtain a new SSL certificate and install it on the server. Once the new certificate was installed, the service was restored, and users were able to access the service again.

Corrective and Preventative Measures: To prevent similar incidents from occurring in the future, the following measures will be taken:

•	Automated monitoring systems will be implemented to track SSL certificate expiration dates and send alerts to the team.

•	The team will implement a policy to renew SSL certificates at least one month before the expiration date.

•	A review of other SSL certificates will be conducted to ensure that all certificates are up to date and renewals are scheduled as needed.

To address the current issue, the following tasks will be completed:

•	Obtain and install a new SSL certificate for the login and registration service.

•	Conduct a review of all SSL certificates to ensure that they are up to date and renewals are scheduled as needed.

•	Conduct a post-incident review with the team to identify areas for improvement and update incident response procedures as needed.
