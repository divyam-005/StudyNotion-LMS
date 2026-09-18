# StudyNotion LMS

StudyNotion is a full-stack Learning Management System where students can explore and enroll in courses and instructors can create and manage course content.

## Features

- Student and instructor authentication
- Email verification and password reset
- Course creation, sections and subsections
- Course catalog and enrollment
- Student dashboard and course progress
- Ratings and reviews
- Shopping cart and payments
- Instructor dashboard
- Profile management
- Cloud-based media uploads

## Tech Stack

**Frontend:** React, Redux Toolkit, React Router, Tailwind CSS, Axios

**Backend:** Node.js, Express.js, MongoDB/Mongoose, JWT, Nodemailer

**Services:** Cloudinary, Razorpay

## Project Structure

```text
StudyNotion-LMS/
├── Frontend/     # React application
└── Server/       # Express API
```

## Setup

Clone the repository:

```bash
git clone https://github.com/divyam-005/StudyNotion-LMS.git
cd StudyNotion-LMS
```

Install frontend dependencies:

```bash
cd Frontend
npm install
cp .env.example .env
npm start
```

Install backend dependencies in another terminal:

```bash
cd Server
npm install
npm run dev
```

The backend requires its own `.env` configuration for database, authentication, email, Cloudinary, Razorpay, and other environment-specific values used by the application.

## Main Architecture

```text
React Frontend
      ↓
Express REST API
      ↓
MongoDB

External services:
Cloudinary → media
Razorpay   → payments
Nodemailer → email
```
