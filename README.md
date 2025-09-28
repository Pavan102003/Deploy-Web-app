# Deploy-Web-app

#Simple Cloud File Uploader ☁️

Host Link : https://deploy-web-app-ud17-2ur3pbiy0-pavan-ks-projects-e631c4b6.vercel.app/

Live Demo: 

Cloud Platform: AWS S3 

Backend:Python Flask

Frontend: HTML/Css/JS 

Hosting: Vercel 

#Project Objective
This project is a small, full-stack web application designed to demonstrate the secure and efficient integration of cloud object storage into a web service. It allows users to upload a file (e.g., image, text), securely stores it in a chosen cloud bucket, and returns a public URL for access.

#Key Features
Secure File Upload: Endpoint handles multipart/form-data uploads.
Direct Cloud Integration: Seamlessly streams/uploads files directly to the cloud storage service using the official SDK.
Public Link Generation: Returns a direct URL to the stored file.
Input Validation: [Detail Bonus Feature 1] (e.g., Files are limited to 5MB maximum size.)
Type Checking: [Detail Bonus Feature 2] (e.g., Only image/jpeg, image/png, and text/plain allowed.)

#Challenges Faced and Key Learnings

The Secure Configuration and Deployment 
The most significant challenge involved establishing a secure and compliant workflow for handling sensitive cloud credentials (AWS_ACCESS_KEY_ID, AWS_SECRET_ACCESS_KEY, etc.) across different environments, specifically:

Preventing Exposure: Ensuring these highly sensitive keys were never committed to the GitHub repository, even when using a local .env file for development.

Deployment Parity: Configuring the serverless host (e.g., Vercel/Netlify) to securely read these variables at runtime, as the local .env file is ignored during the build process.

This process taught me the critical difference between local configuration and secure cloud deployment. It emphasized the importance of using the platform's (Vercel/Netlify) secret environment variable management tools over relying on files

