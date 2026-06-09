# Legal Case Tracker

A lightweight, single-page web application built with vanilla JavaScript, styled with clean CSS, and backed by Firebase (v10). This application allows legal professionals to log, track, filter, and manage case records securely in real-time, with built-in support for multiple languages.

---

## Features

* **Google Authentication:** Secure login using Firebase Auth (Google OAuth). Each user's data is safely sandboxed under their unique User ID (UID).
* **Real-Time Synchronisation:** Uses Firestore's `onSnapshot` listener to instantly stream and reflect database changes (adding, updating, or deleting cases) across the user interface without requiring page reloads.
* **Bilingual Interface:** Features a dynamic UI toggle that instantly switches the entire layout between **English** and **Bengali (বাংলা)**.
* **Instant Client-Side Search:** A live search filter that allows users to seamlessly narrow down cases by the lawyer's name as they type.
* **Automatic User Telemetry:** Saves the logged-in user's profile details (Name, Email, and Last Login Timestamp) to a centralized directory upon authorization.

---

## Tech Stack & Architecture

* **Frontend:** Standard HTML5, Custom responsive CSS3 Grid and Flexbox layout.
* **Core Logic:** Functional Vanilla JavaScript (ES6+ Modules).
* **Backend as a Service (BaaS):** Firebase JavaScript SDK v10 (Authentication & Cloud Firestore).

---

## Local Setup Instructions

Because this repository uses placeholder credentials to protect the original developer's database environment, you must link it to your own Firebase project to run it locally.

### 1. Prerequisites
* A web browser.
* A local development server environment (like the **Live Server** extension in VS Code) to support modular JavaScript imports.

### 2. Firebase Database Configuration
1. Go to the [Firebase Console](https://console.firebase.google.com/) and create a new project.
2. In the **Authentication** section, enable the **Google** sign-in provider.
3. In the **Firestore Database** section, create a database and update your rules to allow authenticated reads and writes.
4. Register a new Web App in your project settings to fetch your specific configuration credentials.
