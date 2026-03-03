# AWS IAM Cloud Security Project   
--- 
## 📌 Project Overview

This project demonstrates the implementation of cloud security controls in Amazon Web Services (AWS), with a primary focus on Identity and Access Management (IAM) and the principle of least privilege.

The objective was to:

- Create IAM users and groups
- Attach managed and custom policies
- Monitor activity using CloudTrail
- Launch and manage EC2 resources
- Create and manage an S3 bucket
- Validate access restrictions and audit activity

---   

## 🏗️ Services Used

- Amazon Web Services
- AWS Identity and Access Management (IAM)
- Amazon EC2
- Amazon S3
- AWS CloudTrail

---   

## 🔐 IAM Configuration
### 1. IAM Group Created
- Group Name: Abatech-processing-documentation
- Policy Attached: AdministratorAccess (AWS managed policy)
This group was created to manage permissions centrally.

### 2. IAM User Created
- User Name: Abatech-processing-documentation-jude
- User added to the IAM group.
A separate custom policy was also created and attached directly to the user.

### 3. Policy Implementation
A policy was created and attached to:
- The IAM user (Abatech-processing-documentation-jude)
The goal was to test permission boundaries and validate least-privilege access.

---   

## 🖥️ EC2 Deployment

- Instance Name: Documentation server
- AMI Used: Windows AMI
Instance lifecycle actions performed:
  - Launch
  - Stop
  - Terminate

This validated:   
  - User permissions for compute management
  - Logging of actions in CloudTrail

---   

## 📦 S3 Bucket Configuration

- Bucket Name: Documentation bucket

Actions performed:   
  - Bucket creation
  - File upload
  - File deletion

This tested:
  - Object-level access
  - Permission enforcement
  - Audit visibility

---   

## 📊 Cloud Monitoring & Logging

- CloudTrail Name: management event

CloudTrail was configured to log:

- IAM activity
- EC2 actions
- S3 operations

This ensures:
  - Accountability
  - Traceability
  - Audit readiness

---

## 🔎 Security Concepts Demonstrated

- Principle of Least Privilege
- Role-based access control (RBAC)
- IAM policy attachment (group vs user)
- Activity monitoring and auditing
- Resource lifecycle management
- Cloud security governance
