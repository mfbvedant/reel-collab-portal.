# reel-collab-portal.
# 🎬 Reel Collab Portal

A modern, serverless web portal designed to streamline Instagram Reel collaborations. Creators can submit their details and video drafts, while administrators can review, accept, or reject applications through a secure dashboard.

## ✨ Features

**For Creators:**
* **Seamless Submissions:** Clean, glassmorphism UI to submit contact details, academic info, and Instagram handles.
* **Secure Status Tracking:** Generates a unique, randomized tracking token upon submission.
* **Live Status Updates:** Users can check if their reel is `Pending`, `Selected`, or `Rejected` at any time using their token.

**For Administrators:**
* **Secure Admin Portal:** Password-protected dashboard to manage all incoming applications.
* **Live Evaluation:** Instantly change the status of any application and save it directly to the database.
* **Data Portability:** Export all submissions to a `.json` file for backups, or import data directly into the database.

## 🛠️ Tech Stack
* **Frontend:** HTML5, Vanilla JavaScript
* **Styling:** Tailwind CSS (via CDN)
* **Backend / Database:** Firebase Firestore (Serverless)
* **Hosting:** GitHub Pages

## 🚀 How to Use

**1. Creator Flow**
* Fill out the submission form with your details.
* Agree to the collaboration terms and click submit.
* Copy the generated Tracking Token.
* Enter the token in the "Track Status" sidebar to see real-time updates.

**2. Admin Flow**
* Click the "ADMIN" button in the top right corner.
* Enter the access code (Default: `admin123`).
* Review submissions, update their status, and click "Save".
* Use the Export/Import tools to manage database records.

## 🔒 Security Note
This project uses Firebase Client SDKs. To ensure data is protected, ensure your Firestore Security Rules are set to only allow public creation and token-based reading, while restricting full database reads to authorized structures.
