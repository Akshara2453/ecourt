⚖️ Vakil Varta — E-Portal for Court Case Management

A modern web application for lawyers, clients, and courts to digitally manage case workflows, book consultations, and verify identities using OTP-based email verification.

This Node.js-based portal offers lawyer-client profile management, secure email OTP verification, and dashboard access for streamlined court case operations.

🚀 Features

👨‍⚖️ Lawyer Profile Creation & Management (/lawyer)

👨‍💼 Client Registration & Interaction (/client)

📊 Dashboard Interface (/dashboard)

📩 OTP-based Email Verification System

📁 EJS Templating for Dynamic Pages

🌐 CORS-enabled backend for API use

🏗️ Tech Stack

Layer	Technology

Backend	Node.js, Express.js

Database	MongoDB with Mongoose ORM

Frontend	EJS Templates

Mailer	Nodemailer with Gmail SMTP

Middleware	CORS, Body Parser, Method Override

📨 OTP Verification Workflow

Used for email verification when signing up:

POST /sendotp

Generates a 4-digit OTP

Sends it to the user's email via Gmail SMTP

Stores it temporarily in memory for 60 seconds

POST /verify

Accepts the OTP and email from user

Verifies if OTP matches the stored one

🔧 How to Run Locally

Clone the Repository

git clone https://github.com/Akshara2453/ecourt.git

cd ecourt

Install Dependencies

npm install

Setup Environment Variables

Create a .env file:

touch .env

Add your mongo atlas connection string in .env file

Run the App

node app.js

Open: http://localhost:8080
