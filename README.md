# AWS-IAM-SNS-Config
Configured and tested resource monitoring using AWS Config integrated with Amazon SNS for real-time alerts, validating notifications through EC2 activity and optimizing cost by securely disabling services.

Configured an admin user in Amazon Web Services IAM with Administrator and Billing access, enhancing security by implementing Multi-Factor Authentication (MFA) and restricting root account usage.
<img width="990" height="800" alt="image" src="https://github.com/user-attachments/assets/30018d84-896c-4f53-b47e-f5e4c89cf5a8" />


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

<img width="745" height="897" alt="2" src="https://github.com/user-attachments/assets/d7f15dff-8a90-4fe2-9140-fd64f0f22d46" />
<img width="938" height="742" alt="3" src="https://github.com/user-attachments/assets/a4c832f4-b9ae-4461-ad6b-1bfbbcceb8bc" />


2️⃣ Configure SNS Alerts
Created SNS Topic (config-topic)
Added subscription with Email protocol
Confirmed subscription via email

<img width="1902" height="870" alt="7" src="https://github.com/user-attachments/assets/510d1a33-1e13-4e95-b918-744e2856c727" />
<img width="1895" height="873" alt="8" src="https://github.com/user-attachments/assets/0c525e60-3506-4503-965c-81bdf88518d7" />
<img width="1912" height="920" alt="9" src="https://github.com/user-attachments/assets/30610a5c-a4b7-457d-b95d-ff1a74aa7b52" />


3️⃣ Validate Monitoring
Created an EC2 instance
Observed email notification from SNS
Deleted EC2 instance after testing
Verified alert notifications for changes


<img width="1912" height="965" alt="10" src="https://github.com/user-attachments/assets/0e3b0870-ac47-4f50-aa3a-3fd2e99af14f" />
<img width="1893" height="902" alt="11" src="https://github.com/user-attachments/assets/1577a2e2-e97f-4efb-aee5-ae60206612a1" />
<img width="1496" height="756" alt="16" src="https://github.com/user-attachments/assets/846e7f7e-2d5e-42b4-8b6f-de73ffe96a40" />

📸 Add Screenshot Here (Email Alert Example)

4️⃣ Disable Services (Cost Optimization)
Disabled AWS Config recording
Deleted SNS topic and subscriptions

<img width="1908" height="965" alt="14" src="https://github.com/user-attachments/assets/dc69a7f3-519a-4ba1-8f30-470596ab7e94" />
<img width="1901" height="895" alt="13" src="https://github.com/user-attachments/assets/591c5120-071a-4acd-bf1d-2dc5f7dfb997" />

# ✅Key Outcomes
Successfully implemented real-time infrastructure monitoring
Verified alert system using SNS notifications
Gained hands-on experience with AWS Config rules and tracking
Applied cost optimization by disabling unused services

<img width="1886" height="902" alt="15" src="https://github.com/user-attachments/assets/2ac8aa73-5a10-437a-b570-c03ad3e5eac2" />


# 🚀Conclusion
This project highlights practical knowledge of AWS monitoring and alerting services, ensuring visibility, compliance, and cost-efficient cloud operations.
