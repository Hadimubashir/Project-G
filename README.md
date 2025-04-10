# 💸 AWS Cost Optimization – Automated Snapshot Cleanup

Automated the cleanup of unused Amazon EBS snapshots to reduce unnecessary storage costs and improve cloud resource efficiency using AWS Lambda and Python.

## 🛠️ Tools & Technologies
- AWS Lambda
- Python (Boto3)
- AWS CloudWatch
- IAM (Identity and Access Management)

## 🔁 What It Does

- **Automated Cleanup**:  
  Developed a Lambda function in Python to automatically detect and delete **unassociated EBS snapshots**.

- **Boto3 Integration**:  
  Utilized **AWS SDK (Boto3)** to scan and filter snapshots that are no longer attached to any EC2 volumes or instances.

- **Monitoring & Logs**:  
  Connected with **AWS CloudWatch** for real-time logging, monitoring, and alerting of snapshot cleanup operations.

- **IAM Role Configuration**:  
  Assigned a least-privileged **IAM role** to the Lambda function for secure and scoped access to EC2 and snapshot resources.

## 📈 Benefits
- Reduced **EBS storage costs**
- Improved **resource hygiene**
- Fully **automated** and **serverless** operation
- No human intervention required

## 🚀 How to Deploy

1. Create a Lambda function in AWS Console.
2. Assign appropriate IAM permissions (e.g., `ec2:DescribeSnapshots`, `ec2:DeleteSnapshot`).
3. Paste the Python (Boto3) script into the Lambda function.
4. Set a CloudWatch Event Rule (e.g., schedule daily or weekly) to trigger the function.
5. Monitor logs in **CloudWatch Logs** for successful cleanup reports.

---

> This project highlights efficient cost optimization practices and automation using AWS serverless technologies.
