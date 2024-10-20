# Ansible Configuration for S3 Upload and CloudFront Invalidation

Welcome to the **Ansible Configuration for S3 Upload and CloudFront Invalidation** project! This repository houses Ansible playbooks to streamline the process of deploying files to AWS S3 and invalidating CloudFront caches.

## Table of Contents

- [Introduction](#introduction)
- [Features](#features)
- [Prerequisites](#prerequisites)
- [Setup](#setup)
- [Usage](#usage)
- [Contributing](#contributing)
- [License](#license)

## Introduction

This project is part of the Purple Cohort in the Level Up In Tech DevOps Bootcamp. It demonstrates automating AWS operations using Ansible.

## Features

- **Code Checkout**: Clones the latest code from the repository.
- **AWS Credentials Setup**: Configures AWS credentials for secure access.
- **File Upload**: Automates the upload of files to an S3 bucket.
- **CloudFront Invalidation**: Automates invalidation of CloudFront cache to reflect changes instantly.

## Prerequisites

- Python 3.x
- Ansible
- AWS CLI
- Git

## Setup

1. **Clone the repository**:
    ```sh
    git clone https://github.com/your-username/your-repo-name.git
    cd your-repo-name
    ```

2. **Create a virtual environment**:
    ```sh
    python -m venv venv
    ```

3. **Activate the virtual environment**:
    ```sh
    # On macOS/Linux
    source venv/bin/activate
    
    # On Windows
    .\venv\Scripts\activate
    ```

4. **Install dependencies**:
    ```sh
    pip install -r requirements.txt
    ```

5. **Set up AWS credentials**:
    Ensure your AWS credentials are set as environment variables:
    ```sh
    export AWS_ACCESS_KEY_ID=your-access-key-id
    export AWS_SECRET_ACCESS_KEY=your-secret-access-key
    export AWS_DEFAULT_REGION=us-east-1
    ```

## Usage

To execute the playbook, run:
```sh
ansible-playbook -i inventory playbook.yml