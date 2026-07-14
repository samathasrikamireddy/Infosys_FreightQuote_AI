
# 🔐 Intelligent Freight Quote Generation – Authentication Module (Milestone 1)

## 📌 Project Overview

This repository contains the Authentication and User Management Module developed as part of the Infosys Springboard Internship 7.0 – Milestone 1. The application provides secure user authentication using JWT, password recovery through Security Questions and OTP verification, and separate dashboards for users and administrators.

🚀 How to Run the Application (Google Colab)

This application is designed to be executed in a Google Colab environment and exposed to the web using Ngrok.

1. Prerequisites

   You will need to add two secret keys to your Google Colab Secrets tab (the key icon on the left sidebar):

    NGROK_AUTHTOKEN: Your personal authentication token from Ngrok.

   EMAIL_PASSWORD: A 16-character Google App Password used to send OTP emails.

3. Execution Steps
Open the notebook file in Google Colab.

1.Run the Installation Cell to install required dependencies:

2.!pip install streamlit pyngrok bcrypt PyJWT

3.Run the Application Cell (%%writefile app.py) to generate the core script.

4.Run the Server Cell to launch the Streamlit server in the background and establish the Ngrok tunnel.

5.Click the generated *.ngrok-free.dev URL in the output to access the live application.

## ✨ Key Features

Secure User Registration:
Enforces strict password complexity rules (uppercase, lowercase, numbers, symbols, min 8 characters) and prevents duplicate email/username registrations.

Encrypted Authentication: 
Utilizes bcrypt for secure password hashing and PyJWT (JSON Web Tokens) for stable session management.

Dual-Method Password Recovery: 
* Security Questions: Instant reset using user-defined security answers.

OTP Email Verification: 
* Sends a time-sensitive, 6-digit One-Time Password to the user's registered email using smtplib.

Role-Based Dashboards:
* Admin Panel: Exclusive root access (admin@infosys.com) to monitor all registered network operators.

Operator Dashboard: 

* Provides system metrics, document indexing stats, and active task tracking for standard users.

Dynamic Enterprise UI: 

* Custom CSS overrides providing a sleek dark/light mode experience with responsive card containers and hidden default Streamlit branding.

### 🔐 Secure User Registration

The application allows new users to create an account by providing a unique username, email address, password, confirm password, security question, and security answer. Strong password validation and duplicate username checks are performed before registration.

**📷 Signup Page Screenshot**

<img width="622" height="922" alt="Screenshot 2026-07-09 141743" src="https://github.com/user-attachments/assets/bf033548-05fe-4b3e-b65b-148bc6c2837c" />






### 🔑 Secure Login

Registered users can securely log in using their email/username and password. After successful authentication, a JWT session token is generated and users are redirected to their dashboard.

**📷 Login Page Screenshot**

<img width="809" height="1020" alt="Screenshot 2026-07-09 141529" src="https://github.com/user-attachments/assets/7bf10f7f-a3c4-4cb8-a5e3-51711bdfc482" />




### 🔄 Password Recovery

#### ❓ Security Question Recovery

Users can reset their password by answering the security question they selected during registration.

**📷 Security Question Screenshot**

<img width="688" height="1020" alt="Screenshot 2026-07-09 141848" src="https://github.com/user-attachments/assets/c3f63537-3d79-4c43-830d-2046e5742789" />


#### 📧 OTP Email Verification

Users can request a One-Time Password (OTP) to their registered email address for secure password recovery.

**📷 OTP Verification Screenshot**

<img width="896" height="896" alt="Screenshot 2026-07-09 141908" src="https://github.com/user-attachments/assets/ab0a8993-eee3-4d50-962b-fb1d8c3504fe" />

#### ✉️ OTP Email

The OTP is sent to the registered Gmail account using Gmail SMTP.

**📷 OTP Email Screenshot**

<img width="1920" height="633" alt="Screenshot 2026-07-09 144806" src="https://github.com/user-attachments/assets/d507fe1e-3bbd-4ab3-b1e9-1662f4a32ac9" />


### 👤 User Dashboard

After successful login, users are redirected to the dashboard where they can access the application's features.

**📷 User Dashboard Screenshot**

<img width="1885" height="813" alt="Screenshot 2026-07-09 145044" src="https://github.com/user-attachments/assets/9270da40-179f-49c9-a6b2-31901156955d" />


### 👨‍💼 Admin Dashboard

The administrator can log in separately to view all registered users while ensuring passwords remain securely encrypted.

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

.
📁 Repository Structure
├── app.py                  # Main application script
├── README.md               # Project documentation
└── screenshots/            # Directory containing visual proof of work
    ├── login_page.png
    ├── signup_validation.png
    ├── forgot_password_otp.png
    ├── email_inbox_otp.png
    ├── operator_dashboard.png
    └── admin_dashboard.png

