# Chapter: The AAA of Security

The AAA, also known as Triple A, refers to the three key elements of security: Authentication, Authorization, and Accounting/Auditing. AAA is a security framework that controls access to computer resources, enforces policies, and audits usage.

## 1 Authentication

Authentication involves a user providing information about who they are. Users present login credentials that affirm they are who they claim. AAA compares a user’s credentials with its database of stored credentials by checking if the username, password, and other authentication tools align with that specific user.

Three types of authentication include something you know (like a password), something you have (like a Universal Serial Bus (USB) key), and something you are (such as your fingerprint or other biometrics).

## 2 Authorization

Authorization follows authentication. During authorization, a user can be granted privileges to access certain areas of a network or system. Authorization differs from authentication in that authentication only verifies a user’s identity, whereas authorization dictates what the user is allowed to do.

For example, a member of the IT team may not have the necessary privileges to change the access passwords for a company-wide virtual private network (VPN). However, the network administrator may choose to give the member access privileges, enabling them to alter the VPN passwords of individual users.

## 3 Accounting/Auditing

Accounting/Auditing keeps track of user activity while users are logged into a network. It may be used to analyze user trends, audit user activity, and provide more accurate billing.

## 4 Why is AAA Important in Network Security?

AAA is a crucial part of network security because it limits who has access to a system and keeps track of their activity. There are two main types of AAA for networking: network access and device administration.

### 4.1 Network Access

Network access involves blocking, granting, or limiting access based on the credentials of a user. AAA verifies the identity of a device or user by comparing the information presented or entered against a database of approved credentials. If the information matches, access to the network is granted.

### 4.2 Device Administration

Device administration involves the control of access to sessions, network device consoles, secure shell (SSH), and more. This type of access differs from network access as it does not limit who is allowed into the network but rather which devices they can have access to.