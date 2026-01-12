# AWS EC2 Auto Start and Stop Using Lambda

This project automates the starting and stopping of EC2 instances using AWS Lambda and CloudWatch Events (EventBridge). It helps reduce AWS costs by shutting down unused servers during non-working hours.

## 🔧 Technologies Used
- AWS Lambda
- Amazon EC2
- CloudWatch Events (EventBridge)
- IAM
- Python (Boto3)

## 📌 Project Overview
Two Lambda functions are created:
- One to start EC2 instances
- One to stop EC2 instances

These functions are triggered automatically using CloudWatch Event rules based on time schedules.

## 🛠️ How It Works
1. CloudWatch Event triggers Lambda at scheduled time
2. Lambda executes Python script
3. Lambda uses Boto3 to call EC2 API
4. EC2 instances are started or stopped automatically

## 📂 Files
- start_ec2.py → Starts EC2 instance
- stop_ec2.py → Stops EC2 instance

## 🎯 Use Case
This project is useful for:
- Development servers
- Testing environments
- Cost optimization

## 👨‍💻 Author
Ayush Dungarwal
