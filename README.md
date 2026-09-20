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
