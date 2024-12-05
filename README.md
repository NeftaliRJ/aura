# Fullstack Test: React (Next.js) & NestJS

This project demonstrates my skills in fullstack development, implementing a **frontend** with **Next.js (React + TypeScript)** and a **backend** with **NestJS**. I invested **5 hours** into this test to deliver a functional application closely aligned with the provided requirements.

## Table of Contents

- [Fullstack Test: React (Next.js) \& NestJS](#fullstack-test-react-nextjs--nestjs)
  - [Table of Contents](#table-of-contents)
  - [Overview](#overview)
  - [Project Structure](#project-structure)
  - [Features Implemented](#features-implemented)
    - [Authentication Screen](#authentication-screen)
    - [Home Screen](#home-screen)
  - [How to Run the Project](#how-to-run-the-project)
    - [Prerequisites](#prerequisites)
    - [Steps to Run Locally](#steps-to-run-locally)
    - [Docker Setup](#docker-setup)
  - [Live Demo](#live-demo)
  - [Notes](#notes)

---

## Overview

This application was developed as a test to showcase:
- **TypeScript-based development** in both frontend and backend.
- Usage of **React** for building dynamic and responsive UI.
- Integration of an **external API** for live search functionality.
- Implementation of **form validation** and **conditional rendering**.
- Development of a **chatbot** feature using an external AI service.

The goal was to replicate the given **Figma design** as closely as possible and demonstrate proficiency in:
- Authentication flows.
- Form handling and validations.
- API integration.
- AI service utilization.

---

## Project Structure

- **Frontend**: Located in the `frontend` folder, built with **Next.js (React + TypeScript)**.
- **Backend**: Located in the `backend` folder, built with **NestJS**.

---

## Features Implemented

### Authentication Screen
- Users must log in with valid credentials stored in a JSON file.
- Validation:
  - **Email** input only accepts valid email formats. If invalid, it shows an error: "Invalid user".
  - The "Continue" button remains disabled until both the email and password fields are filled.
- Users cannot access the home screen without successful authentication.

### Home Screen
Includes three primary options:
1. **Search Data**:
   - Implements live search functionality using the Financial Modeling Prep API or an equivalent free API.
   - The search bar dynamically updates results as characters are typed.

2. **Upload Data**:
   - Form with validation rules:
     - Fields marked with a red asterisk are required.
     - Conditional rendering:
       - If "Company Research" is selected, a "Companies" input appears and becomes required.
     - Checklist behavior: Selecting "All" automatically checks all options.

3. **Try AI**:
   - A chatbot interface integrated with a free AI API (e.g., OpenAI, Anthropic, or Google).
   - Users can ask questions and receive AI-generated responses.

---

## How to Run the Project

### Prerequisites
- **Node.js**: Ensure you have Node.js installed.
- **Docker**: Recommended for ease of running the app.
- **API Keys**: Obtain API keys for:
  - Financial Modeling Prep (or equivalent free API).
  - AI service (e.g., OpenAI, Anthropic, or Google).

### Steps to Run Locally
1. **Clone the Repository**:
   ```bash
   git clone https://github.com/your-repo/fullstack-test.git
   cd fullstack-test
   ```

2. **Backend Setup**:
   ```bash
   cd backend
   npm install
   npm run start
   ```

3. **Frontend Setup**:
   ```bash
   cd ../frontend
   npm install
   npm run dev
   ```

4. Access the application at [http://localhost:3000](http://localhost:3000).

### Docker Setup
Alternatively, you can use Docker:
1. Build and start the containers:
   ```bash
   docker-compose up --build
   ```
2. Access the application at [http://localhost:3000](http://localhost:3000).

---

## Live Demo

A live version of the application is hosted on **Vercel**.  
[Check it out here](#).

---

## Notes
- The project adheres to best practices in **code quality**, **security**, and **modularity**.
- Suggestions for improvement or feedback are welcome. Please open an issue in the repository.

---
Thank you for reviewing this project!