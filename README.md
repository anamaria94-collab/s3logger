# s3logger

**s3logger** is a backend cloud project that enables secure file uploads to AWS S3 and automatic metadata logging to DynamoDB. It uses Terraform to provision infrastructure and supports optional automation via Python or AWS CLI.

---

## Project Overview

This project was designed for a small consulting client that needed to:

- Accept document uploads via a centralized cloud location
- Automatically track metadata (filename, size, upload timestamp)
- Avoid maintaining servers or custom applications
- Maintain flexibility for future integrations

---

## Architecture

- **Amazon S3** – for secure, scalable file storage
- **Amazon DynamoDB** – for tracking metadata
- **IAM** – for scoped access control
- **Terraform** – for reproducible infrastructure

