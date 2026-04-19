# 📊 Monitoring and Alerts with AWS CloudWatch
Implemented real-time monitoring and alerting for an EC2-based application using AWS CloudWatch and SNS.

## 🚀 Features
* Implemented threshold-based CPU utilization monitoring using CloudWatch
* Configured EC2 instance health checks using StatusCheckFailed metric
* Integrated Amazon SNS for automated real-time alert delivery
* Simulated production-like load to validate monitoring and alerting pipeline

### Architecture Flow
Client → EC2 Instance → CloudWatch Metrics → CloudWatch Alarm → SNS → Email Notification
<img width="1536" height="1024" alt="cloudwatch_alarms" src="https://github.com/user-attachments/assets/e3e11687-3800-49e2-b030-b8f1abf737cb" />

## 📸 Screenshots

### 🔴 Alarm Triggered
<img width="1920" height="1008" alt="alarm ec2" src="https://github.com/user-attachments/assets/de546c22-e1e9-4070-a55d-7795f5229b00" />

### 📩 SNS Email Notification
<img width="1920" height="1008" alt="sns email" src="https://github.com/user-attachments/assets/86a18c33-8cc0-46ff-9db8-c01629c32749" />

### ⚙️ Alarm Configuration
<img width="1920" height="1008" alt="alarm config" src="https://github.com/user-attachments/assets/388cba75-2d90-462d-8924-67a8490adde8" />

### 📡 SNS Topic
<img width="1920" height="1008" alt="sns subscription" src="https://github.com/user-attachments/assets/453f5110-8472-49ca-8495-be90e1cd1499" />

### 📈 EC2 CPU Spike
<img width="1920" height="1008" alt="cpu spike" src="https://github.com/user-attachments/assets/2c97fc36-8720-4070-b87c-ed347b5e2647" />

## 🛠️ Tools Used
* AWS CloudWatch
* Amazon SNS
* Amazon EC2

## 🧪 Testing & Validation
* Generated high CPU load using stress tool to simulate real-world scenarios
* Verified alarm state transitions (OK → ALARM)
* Confirmed end-to-end notification delivery via SNS email alerts

## 🧠 Key Learnings
* CloudWatch alarms depend on sufficient datapoints for accurate evaluation
* Monitoring resolution (1-minute vs 5-minute) directly impacts alert responsiveness
* SNS enables decoupled, event-driven notification systems
* Sustained load is required to reliably trigger monitoring thresholds

## ✅ Outcome
Built a complete monitoring and alerting system capable of detecting performance issues and notifying users in real-time.
