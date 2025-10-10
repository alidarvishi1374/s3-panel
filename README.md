# 🪣 S3 Panel

**S3 Panel** is a lightweight web-based management tool built with **Flask** and **Boto3** that allows you to easily manage S3-compatible object storage systems such as **AWS S3**, **MinIO**, or **Ceph Object Gateway**.

It provides an intuitive interface to handle users, groups, bucket policies, IAM rules, lifecycle management, versioning, and replication — all in one place.

---

## 🚀 Features

- 🧱 **Bucket Management**
  - Create, list, and delete buckets
  - Configure bucket policies
  - Enable/disable versioning and lifecycle rules
  - Manage replication rules

- 📁 **File Operations**
  - Upload and download files directly from the panel
  - View object metadata

- 👥 **User & Group Management**
  - Create IAM users and groups
  - Attach and detach policies
  - Manage user credentials and permissions

- 🔐 **Security**
  - Manage STS tokens for temporary access
  - Control access policies for users, groups, and buckets

- ⚙️ **Other Features**
  - Simple SQLite3 backend for local data persistence
  - Compatible with custom S3 endpoints
  - Lightweight, fast, and Docker-ready

---

## 🧩 Tech Stack

- **Backend:** Python, Flask  
- **Cloud SDK:** Boto3  
- **Database:** SQLite3  
- **Frontend:** Jinja2 (Flask templates)  
- **Containerization:** Docker  

---

## 🐳 Run with Docker

You can quickly run **S3 Panel** using Docker:

```bash
docker run --rm -itd \
  --name s3 \
  -p 5000:5000 \
  -v /root/database:/app/database \
  ghcr.io/alidarvishi1374/s3-panel:latest
