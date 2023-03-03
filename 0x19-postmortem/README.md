On March 1, 2023, from 10:00 AM to 12:30 PM (PST), the login service for our web application was unavailable, affecting approximately 60% of our users. Users attempting to log in during this period received error messages and were unable to access the platform.
Timeline:
•	10:00 AM: The issue was detected when a monitoring alert went off, indicating that the login service was experiencing high error rates.
•	10:05 AM: Engineers began investigating the issue, starting with the login service logs and checking the health of the associated servers.
•	10:30 AM: The investigation initially focused on the server infrastructure, as the logs indicated issues with network connectivity and server load.
•	11:00 AM: As the server infrastructure was ruled out as the root cause, the team began looking into the application code, specifically the authentication logic.
•	11:30 AM: A possible bug was found in the code that handles password hashing and storage, and the team began testing a fix.
•	12:00 PM: The fix was deployed to the staging environment, and testing showed that the login service was working again.
•	12:30 PM: The login service was fully restored, and the incident was resolved.
Root Cause and Resolution: The root cause of the issue was a bug in the authentication code that was causing errors during password hashing and storage. This bug was likely introduced during a recent code update and was not caught during testing due to an incomplete test suite.
To resolve the issue, the team rolled back the recent code update and deployed a fix to the authentication code. The fix addressed the bug and included additional tests to catch similar issues in the future.
Corrective and Preventative Measures: To prevent similar issues in the future, the team will take the following actions:
•	Improve the test suite to cover more edge cases and catch potential bugs.
•	Implement more robust monitoring and alerting for the login service and related infrastructure.
•	Review the deployment process and ensure that proper testing and quality assurance procedures are in place.
•	Conduct a post-incident review to identify areas for improvement and update incident response procedures as needed.
Tasks to address the issue include:
•	Conduct a thorough review of the authentication code and ensure that all potential issues are addressed.
•	Improve the test suite to cover more edge cases and ensure that all code changes are thoroughly tested.
•	Update the deployment process to include additional testing and quality assurance steps.
•	Review monitoring and alerting policies and ensure that they are properly configured and cover all critical services.
In conclusion, the outage was caused by a bug in the authentication code that was quickly resolved by the engineering team. The incident highlighted the need for more robust testing and monitoring procedures, which the team will address going forward to prevent similar issues in the future.


