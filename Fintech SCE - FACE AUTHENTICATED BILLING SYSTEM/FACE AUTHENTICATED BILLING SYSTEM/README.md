# Face Authenticated Billing System

## Project Overview

The Face Authenticated Billing System (FABS) is an advanced e-commerce billing platform that combines facial recognition technology for secure user authentication and efficient invoice and payment management. Designed to enhance security and streamline workflows, FABS allows businesses to handle billing, invoicing, and payments with ease.

### Key Features:
- **Facial Recognition Authentication**: Ensures that only authorized users (admin or operators) can access the system.
- **Invoice Management**: Generate, send, track, and manage invoices in real-time.
- **Payment Processing**: Integrates with Razorpay to allow secure online payments.
- **Real-time Notifications**: Receive immediate alerts for status changes, payment confirmations, and invoice updates.
- **QR Code Generation**: Generate QR codes for quick invoice access.
- **User Profiles**: Store customer profiles securely using facial biometrics for faster future transactions.

This system is highly scalable and can be used across various sectors, including retail, e-commerce, healthcare, and more.

## Technologies Used

- **Frontend**: React.js, Ant Design, Bootstrap, Axios, React Webcam, QRCode.react
- **Backend**: Node.js, Express.js, Mongoose, Bcrypt.js, CORS, Dotenv, Nodemailer, Razorpay
- **Database**: MongoDB
- **Authentication**: Face ID API, Firebase
- **Real-Time Updates**: WebSocket for real-time interactions
- **Payment Gateway**: Razorpay API

## Prerequisites

Before setting up the project, ensure that you have the following installed:

- **Node.js** and **npm** (for backend and frontend dependencies)
- **MongoDB** (for database)
- **Razorpay** account (for payment integration)
- **Firebase** project (for user authentication)

## Installation and Setup

### 1. Clone the Repository
### 2. Backend Setup
Install Dependencies:
```bash
npm install express mongoose bcryptjs cors dotenv jsonwebtoken nodemailer razorpay
```
Set up Environment Variables:
Create a .env file in the root of the backend project and include the following variables:
```bash
MONGO_URL=your_mongo_connection_string
MONGO_DATABASE=your_database_name
JWT_SECRET=your_jwt_secret_key
RAZORPAY_KEY_ID=your_razorpay_key_id
RAZORPAY_SECRET_KEY=your_razorpay_secret_key
EMAIL=your_email_username
EMAIL_PASSWORD=your_email_password
PUBLIC_DOMAIN=http://localhost:3000
```
### 3. Frontend Setup
Install Dependencies:
Navigate to the frontend folder and install the required dependencies:
```bash
cd billing-system
npm install @emotion/react @emotion/styled @faceio/fiojs @mui/icons-material @mui/material @testing-library/jest-dom @testing-library/react @testing-library/user-event antd axios bootstrap firebase html5-qrcode qrcode.react react-router-dom react-spinners react-webcam styled-components web-vitals
```
Set up Environment Variables:
Create a .env file in the frontend project and include the following variables:
```bash
REACT_APP_BASE_URL=http://localhost:5000
REACT_APP_PUBLIC_ID=your_face_id_public_id
REACT_APP_FACE_ID_API=your_face_id_api_key
REACT_APP_FIREBASE_API_KEY=your_firebase_api_key
REACT_APP_FIREBASE_AUTH_DOMAIN=your_firebase_auth_domain
REACT_APP_FIREBASE_PROJECT_ID=your_firebase_project_id
REACT_APP_FIREBASE_STORAGE_BUCKET=your_firebase_storage_bucket
REACT_APP_FIREBASE_MESSAGING_SENDER_ID=your_firebase_messaging_sender_id
REACT_APP_FIREBASE_APP_ID=your_firebase_app_id
REACT_APP_RAZORPAY_KEY_ID=your_razorpay_key_id
```
## Running the Project
1. Backend:
Start the backend server with:
```bash
node index.js
```
Alternatively, use nodemon for auto-restarting the server during development:
```bash
nodemon index.js
```
2. Frontend:
Start the frontend server with:
```bash
cd billing-system
npm start
```
This will run the frontend application, typically at http://localhost:3000.

Usage
Once the backend and frontend servers are running, navigate to http://localhost:3000 in your browser. The system will prompt users to log in via facial recognition.

## Features:
Admin Dashboard: Provides access to user management, system settings, and analytics.

Operator Dashboard: Facilitates the creation, management, and payment processing of invoices.

Notifications: Instant email alerts and real-time updates of payment and invoice status.

QR Code Access: Scan QR codes to quickly view or pay invoices.

## Future Work
Planned Enhancements:
Multi-biometric Authentication: Incorporating fingerprint and iris scanning alongside facial recognition for added security and user preference.

Improved Facial Recognition: Utilizing advanced machine learning models for more accurate facial recognition, especially under various lighting conditions.

Expanded Reporting & Analytics: Provide customizable dashboards for deeper insights into user behavior and payment trends.

Scalability for Enterprises: Improve the system’s scalability for handling large-scale enterprise applications with millions of users and transactions.

Privacy and Compliance: Ensure that biometric data is stored and processed in compliance with global standards (e.g., GDPR, HIPAA).

## Conclusion
The Face Authenticated Billing System offers an advanced, secure, and efficient solution for billing and payment processing, leveraging facial recognition for authentication and real-time updates for seamless operations. This system is ideal for businesses looking to improve security, streamline billing workflows, and enhance the overall customer experience.

## License
This project is licensed under the MIT License - see the LICENSE file for details.
