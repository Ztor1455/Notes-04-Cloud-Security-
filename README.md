# Notes-04-Cloud-Security-

Quote: "Security should be the most important conversation regarding any IT implementation. A security vulnerability that is not taken care of can potentially destroy years of efforts in just a matter of minutes.” -Intro Module 4 ACFv2
  
## AWS shared responsibility model

•	Indicates which parts of security will be handled by either AWS or on the customers behalf. 

•	AWS is responsible for 
  
  o	All items related to the physical implementation such as data centers.
 
  o	Global infrastructure and all that relates to it.
 
  o Ensures virtualization infrastructures are provided isolation. 
 
  o	Total control of software virtualization layer.
  
  o	Provides the tools customers need to secure the items controlled by them. 
 
  o	Covers mainly PAAS & SAAS

•	Customers are responsible for 

  o	Security in the cloud such as applications & data set 

  o	Encryption of data at both rest & transit. 

  o Ensure network & firewall configuration 
  
  o	The use of tools to secure apps & data.

  o	Mainly IAAS 

## AWS Identity and Access Management (IAM)

•	Manage access to AWS resources for example Amazon EC2 instance and whom may have control to terminate instances.

•	No cost feature with AWS account.

•	Allows control of all AWS services by using policies & assigning them to users. 

•	Handles authentication and verification 

•	Tool that centrally manages and access launching, configuring, and managing.

•	IAM user is defined by selecting the types of access users are permitted.


•	Types of authentications and access 
  
  o	Programmatic access

  o	AWS Management Console access 

  o	Multi-factor authentication or MFA for increased security

•	Iam policies 

  o	Document that defines permissions 	
  
  o	Either identity based or resource based 

  o	Specify whether an action “may” or “may not” occur

  o	Single policy to multiple entities 

  o	Single entity can have multiple policies 

•	Iam group is collection of I am users

  o	Used to grant same permissions to multiple users at one time

  o	User can be in multiple groups

•	Iamrole is identity with specific permissions
Securing a new AWS account

•	Begin with identity or “AWS root account” with complete access to all services in AWS

•	Do not use this account for day-to-day interactions 

•	Use identity and Access management to create users with certain permissions

•	Step 1: Stop using account root user asap 

•	Step 2: Enable multi-factor authentication 

•	Step 3: Secure a new AWS account using AWS CloudTrail;

  o	Tracks user activity 

  o	Logs API requests 

•	Step 4: Enable a billing report like an AWS Cost and Usage report 

## Securing Accounts 

•	AWS Organizations: allows user to consolidate many AWS accounts through features like grouping AWS accounts into units and the use of service control policies. 

•	Service control policies or “SCP” gives similar permission policies to that of IAM but never grants permission and the need to specify maximum number of permissions, but have similar syntax.

•	AWS Key management system: create & manage encryption keys, control of encryption across AWS, integrates with CloudTrail to log all key usage, and uses hardware security modules. 
