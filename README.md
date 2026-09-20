# Cloud & DevOps Internship - Task 2: Infrastructure Setup & Deployment

Welcome to the **Task 2** repository for the Cloud & DevOps Internship. This project demonstrates core AWS infrastructure configuration, networking setup, security parameters, and monitoring implementations.

---

## 🛠️ Infrastructure Architecture

```text
+-------------------------------------------------------------------+
|                        AWS Cloud Platform                         |
|                                                                   |
|   +-----------------------------------------------------------+   |
|   |                       VPC (10.0.0.0/16)                   |   |
|   |                                                           |   |
|   |   +---------------------+       +---------------------+   |   |
|   |   |   Public Subnet     |       |   Private Subnet    |   |   |
|   |   |   (10.0.1.0/24)     |       |   (10.0.2.0/24)     |   |   |
|   |   |                     |       |                     |   |   |
|   |   |  +---------------+  |       |  +---------------+  |   |   |
|   |   |  | EC2 Instance  |  |       |  | S3 Storage    |  |   |   |
|   |   |  | (Nginx Server)|  |       |  | Bucket        |  |   |   |
|   |   |  +---------------+  |       |  +---------------+  |   |   |
|   |   +---------------------+       +---------------------+   |   |
|   |              |                             |              |   |
|   |              +--------------+--------------+              |   |
|   |                             |                             |   |
|   |                +--------------------------+               |   |
|   |                | Security Groups / IAM    |               |   |
|   |                +--------------------------+               |   |
|   +-----------------------------------------------------------+   |
|                                 |                                 |
|                    +-------------------------+                    |
|                    |  CloudWatch & Cost Est. |                    |
|                    +-------------------------+                    |
+-------------------------------------------------------------------+
📁 Repository StructurePlaintextCloud-DevOps-Internship/
├── screenshots/
│   ├── cloudwatch-alarm.png.png
│   ├── cost-estimation.png.png
│   ├── ec2-running.png.png
│   ├── iam-mfa-config.png.png
│   ├── nginx-welcome.png.png
│   ├── s3-bucket.png.png
│   ├── security-groups.png.png
│   └── vpc-subnets.png.png
└── README.md
🖼️ Deliverables & Proof of ImplementationFeature / TaskScreenshotVPC & Subnets ConfigurationEC2 Instance DeploymentNginx Web Server VerificationSecurity Groups SetupIAM & MFA SecurityS3 Storage BucketCloudWatch Alarm ConfigurationCost Estimation & Management🚀 Key Highlights & LearningsNetworking: Designed public and private subnets with custom routing rules within a dedicated VPC.Compute: Provisioned Linux EC2 instances, attached appropriate security groups, and hosted an Nginx HTTP server.Security & Access Control: Enabled Multi-Factor Authentication (MFA) and defined least-privilege IAM policies.Monitoring & Cost Control: Set up CloudWatch alarms for resource metrics and reviewed AWS Cost Explorer estimates.EOFgit add README.mdgit commit -m "Update complete README with screenshots table"git push origin main
