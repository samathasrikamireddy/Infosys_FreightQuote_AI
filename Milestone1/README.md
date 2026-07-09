
# 🔐 Intelligent Freight Quote Generation – Authentication Module (Milestone 1)

## 📌 Project Overview

This repository contains the Authentication and User Management Module developed as part of the Infosys Springboard Internship 7.0 – Milestone 1. The application provides secure user authentication using JWT, password recovery through Security Questions and OTP verification, and separate dashboards for users and administrators.

---

## ✨ Key Features

### 🔐 Secure User Registration

The application allows new users to create an account by providing a unique username, email address, password, confirm password, security question, and security answer. Strong password validation and duplicate username checks are performed before registration.

**📷 Signup Page Screenshot**

![Uploading image.png…]()


--

### 🔑 Secure Login

Registered users can securely log in using their email/username and password. After successful authentication, a JWT session token is generated and users are redirected to their dashboard.

**📷 Login Page Screenshot**

*(Paste your Login screenshot here.)*

---

### 🔄 Password Recovery

#### ❓ Security Question Recovery

Users can reset their password by answering the security question they selected during registration.

**📷 Security Question Screenshot**

*(Paste your Security Question screenshot here.)*

#### 📧 OTP Email Verification

Users can request a One-Time Password (OTP) to their registered email address for secure password recovery.

**📷 OTP Request Screenshot**

*(Paste your "Secure Password Reset" screenshot here.)*

#### 🔢 OTP Verification

Users enter the received 6-digit OTP to verify their identity before creating a new password.

**📷 OTP Verification Screenshot**

*(Paste your OTP verification screenshot here.)*

#### ✉️ OTP Email

The OTP is sent to the registered Gmail account using Gmail SMTP.

**📷 OTP Email Screenshot**

*(Paste your Gmail inbox screenshot here.)*

---

### 👤 User Dashboard

After successful login, users are redirected to the dashboard where they can access the application's features.

**📷 User Dashboard Screenshot**

*(Paste your User Dashboard screenshot here.)*

---

### 👨‍💼 Admin Dashboard

The administrator can log in separately to view all registered users while ensuring passwords remain securely encrypted.

**📷 Admin Dashboard Screenshot**

*(Paste your Admin Dashboard screenshot here.)*

---

## 🔒 Security Features

- JWT Authentication
- bcrypt Password Hashing
- Gmail SMTP OTP Verification
- Security Question Authentication
- SQLite Database
- Strong Password Validation
- Email Validation
- Secure Session Management

---

## 🛠️ Technology Stack

- Python
- Streamlit
- SQLite3
- JWT
- bcrypt
- Gmail SMTP
- Google Colab
- ngrok


