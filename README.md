# AWS-IAM-SNS-Config
Configured and tested resource monitoring using AWS Config integrated with Amazon SNS for real-time alerts, validating notifications through EC2 activity and optimizing cost by securely disabling services.

Configured an admin user in Amazon Web Services IAM with Administrator and Billing access, enhancing security by implementing Multi-Factor Authentication (MFA) and restricting root account usage.


# 🔐AWS IAM Admin User & MFA Setup
📌 Project Overview

This project demonstrates how to securely manage access in AWS by creating an admin user using Amazon Web Services IAM and implementing Multi-Factor Authentication (MFA) to enhance account security.

<img width="619" height="900" alt="image" src="https://github.com/user-attachments/assets/deaea834-4ea9-47e5-8723-9235e15a9c4f" />

# 🎯Objectives
Avoid using root account for daily tasks
Create a secure IAM admin user
Assign appropriate permissions (Admin + Billing)
Enable MFA for enhanced security
# 🛠️Services Used
1️⃣Amazon Web Services IAM 
2️⃣Microsoft Authenticator (for MFA)

# ⚙️Implementation Steps
1️⃣ Create IAM Admin User
Logged into AWS Console as root user
Navigated to IAM → Users → Add User
Enabled Console Access and set custom password
Assigned permissions:
AdministratorAccess
Billing
Created user and downloaded credentials (.csv)

📸 Add Screenshot Here (User Creation Step)

2️⃣ Login with IAM User
Used IAM login URL from CSV file
Verified successful login with new admin user

📸 Add Screenshot Here (IAM Login Page)

3️⃣ Enable MFA Security
Navigated to IAM → Users → Security Credentials
Selected Manage MFA Device
Scanned QR code using authenticator app
Entered two consecutive OTP codes
Successfully enabled MFA

📸 Add Screenshot Here (MFA Setup QR Code)

4️⃣ Testing & Validation
Logged out and logged in again
Verified MFA prompt and successful authentication

📸 Add Screenshot Here (MFA Login Verification)

# ✅Key Outcomes
Implemented secure access control using IAM
Enhanced account protection with MFA
Followed AWS best practices by restricting root usage
Gained hands-on experience in identity and security management

# 🚀Conclusion
This project showcases practical knowledge of AWS IAM and security best practices, ensuring controlled access and protection against unauthorized usage in cloud environments.



# 📊 AWS Config Monitoring & SNS Alert Setup
# 📌Project Overview

This project demonstrates how to monitor AWS resources and track configuration changes using AWS Config integrated with Amazon SNS for real-time email notifications.

<img width="619" height="900" alt="image" src="https://github.com/user-attachments/assets/35ab2ded-9ff2-4bed-bcec-f8b5632fdb8a" />


# 🎯Objectives
Enable resource monitoring and configuration tracking
Set up real-time alerts for infrastructure changes
Validate alerts using EC2 activity
Optimize cost by disabling unused services
# 🛠️Services Used
AWS Config
Amazon SNS
Amazon EC2 (for testing alerts)
# ⚙️Implementation Steps
1️⃣ Enable AWS Config
Logged into AWS Console
Selected region (N. Virginia)
Navigated to AWS Config → Get Started
Enabled recording for all resources
Enabled SNS topic for notifications

📸 Add Screenshot Here (AWS Config Setup)

2️⃣ Configure SNS Alerts
Created SNS Topic (config-topic)
Added subscription with Email protocol
Confirmed subscription via email

📸 Add Screenshot Here (SNS Subscription Confirmation)

3️⃣ Validate Monitoring
Created an EC2 instance
Observed email notification from SNS
Deleted EC2 instance after testing
Verified alert notifications for changes

📸 Add Screenshot Here (Email Alert Example)

4️⃣ Disable Services (Cost Optimization)
Disabled AWS Config recording
Deleted SNS topic and subscriptions

📸 Add Screenshot Here (Disable Config & Delete SNS)

# ✅Key Outcomes
Successfully implemented real-time infrastructure monitoring
Verified alert system using SNS notifications
Gained hands-on experience with AWS Config rules and tracking
Applied cost optimization by disabling unused services

# 🚀Conclusion
This project highlights practical knowledge of AWS monitoring and alerting services, ensuring visibility, compliance, and cost-efficient cloud operations.
