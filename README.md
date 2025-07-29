# s3logger

**s3logger** is a backend-focused, serverless cloud project that enables secure file uploads to AWS S3 and automatic logging of file metadata (filename, size, upload timestamp) to DynamoDB. It is designed for traceable, scalable file handling and is fully provisioned using Terraform.

---

## Project Context

This project simulates a real-world scenario for a client operating in the legal and administrative consulting sector. The client manages documents received from external collaborators and needed a reliable, centralized way to store and monitor submitted files.

### Initial Situation

Before the project, the client used shared folders and email attachments to manage incoming files. As their operations grew, this setup introduced several limitations:

- No centralized or scalable storage
- Lack of metadata tracking (e.g., upload time, file size)
- No automation or validation of received files
- Limited access control and traceability


### Requirements

The client needed a solution that could:

- Securely store uploaded documents in the cloud
- Automatically log metadata about each upload
- Require little to no infrastructure maintenance
- Be extensible for future automation (e.g. tagging, alerts)

---

## Solution Overview

The proposed solution consists of:

- **Amazon S3** for secure, scalable file storage
- **Amazon DynamoDB** for metadata logging
- **AWS IAM** for fine-grained access control
- **Terraform** for Infrastructure as Code (IaC)
- *(Optional)* a Python script for local upload automation via Boto3

This architecture meets the client's requirements while staying low-cost, serverless, and easy to maintain.

---

## Architecture

Check the architecture: https://www.mermaidchart.com/play?utm_source=mermaid_js&utm_medium=editor_selection&utm_campaign=playground#pako:eNpdkMFKAzEQhl9lWCi0YE9724OwtQo9iKVb8bDdQzaZ1mg2KclE7YrgK_iKPolJtqXFUyY_38z8_3xm3AjMimyrzDt_ZpZgPdtogNEIbpRETQjoCK02UeVJGj_ulWEC7RGZbPSxpfQU_pKzXhodOoF5Mlb2_SBEypEbV-uqgNI53-HKKJxE3YZiXC_Ke4hSAacdtx_IPYXuKDcJ3Rsl-WGAl6kO01QIAC4vlp4e2hfkdAXioFlnRBu1BWHXnI2upDPWIZRPVTKV13WVw8zzV6QifJXZ7dD-fv9spULXNBESoq3reZo5n8GatdHmBdohMcGIRfq45k5558z5CiTfLu4I0-l1vEd6Y_5UDOnOOQcq_ycEMxudff0B_3mbEQ
