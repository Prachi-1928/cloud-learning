\# Day 8 - AWS IAM Fundamentals



\## What is IAM?



IAM stands for \*\*Identity and Access Management\*\*.



AWS IAM is a service that helps control who can access AWS resources and what actions they can perform.



IAM helps manage:



\* Authentication

\* Authorization



\## Authentication vs Authorization



\### Authentication



Authentication means \*\*verifying who a user is\*\*.



\*\*Example:\*\*



Logging into AWS using a username and password.



\### Authorization



Authorization means \*\*determining what actions a user is allowed to perform\*\*.



\*\*Example:\*\*



A user can access Amazon S3 but cannot delete an EC2 instance.



\## IAM Components



\### IAM Users



IAM Users represent individual people or applications that need access to AWS.



Each user can have:



\* Password

\* Access keys

\* Permissions



\### IAM Groups



IAM Groups are collections of IAM users.



Permissions can be assigned to a group instead of assigning them individually.



\*\*Example:\*\*



Developers Group



\* User 1

\* User 2

\* User 3



\### IAM Policies



Policies define permissions.



They specify:



\* What actions are allowed

\* Which AWS resources can be accessed

\* Under what conditions access is allowed



Policies are written in \*\*JSON format\*\*.



\### IAM Roles



IAM Roles provide temporary permissions.



Roles are commonly used by AWS services.



\*\*Example:\*\*



EC2 Instance → Assumes IAM Role → Access Amazon S3



\## Principle of Least Privilege



Users should receive \*\*only the permissions necessary to perform their tasks\*\*.



This improves security.



\*\*Example:\*\*



Instead of giving `AdministratorAccess` to every user, provide only the permissions they actually require.



\## Root User vs IAM User



\### Root User



The root user has complete access to the AWS account.



\*\*Best practice:\*\*



Do not use the root user for daily activities.



\### IAM User



IAM users should be created for regular AWS access with limited permissions.



\## IAM Security Best Practices



\* Enable Multi-Factor Authentication (MFA)

\* Follow the principle of least privilege

\* Avoid using the root account for daily tasks

\* Use IAM roles instead of long-term credentials when possible

\* Regularly review permissions



