# AI Student Success System — Requirements Document

## 1. Project Overview
The AI Student Success System is a unified educational platform combining:
1. AI Career Guidance Engine  
2. AI Study Plan Generator  
3. AI Coding Tutor  

Its goal is to give students personalized guidance, structured study planning, and AI-assisted coding support.

---

## 2. Target Users
- School students (8th–12th)
- College students (B.Tech/BCA/etc.)
- Beginners learning coding (Java-first)
- Job seekers reskilling for tech roles

---

## 3. Core Features

### 3.1 AI Career Guidance Engine
**Functional Requirements**
- Conduct psychometric and interest assessment.
- Capture user data: strengths, preferences, academic history.
- Recommend suitable career paths.
- Provide learning roadmaps for selected career.
- Provide salary insights, skill demand, future growth.
- Store user profile and progress.

**Non-Functional Requirements**
- GDPR/Privacy compliant.
- Response time ≤ 3 seconds.

---

### 3.2 AI Study Plan Generator
**Functional Requirements**
- Ask user for exam type, subjects, available hours.
- Automatically generate daily/weekly study plan.
- Adjust plan based on:
  - missed tasks  
  - performance  
  - weak subjects  
- Provide notifications/reminders.
- Generate summaries and flashcards from uploaded PDFs/notes.

**Non-Functional Requirements**
- Offline caching of schedule.
- Mobile/desktop responsive UI.

---

### 3.3 AI Coding Tutor
**Functional Requirements**
- Accept code in Java (initially).
- Provide error explanation and debugging help.
- Suggest improvements without giving full code directly.
- Generate practice challenges.
- Create DSA learning roadmap.
- Conduct mock interviews:
  - coding rounds
  - MCQ rounds
  - HR questions

**Non-Functional Requirements**
- Secure code execution sandbox.
- 100% safe environment (no harmful code).

---

### 3.4 User Accounts & Profile
- Login via email or Google.
- Save progress, plans, career results.
- Sync across devices via cloud.

---

## 4. System Requirements

### 4.1 Functional Requirements Summary
- AI Chat Interface  
- Dashboard & analytics  
- Exam planner  
- Code editor  
- File upload (PDF, images)  
- Notifications service  

### 4.2 Non-Functional Requirements
- 99% uptime.
- Scalability up to 1M users.
- Logging & monitoring (Prometheus/Grafana).
- Security:
  - JWT authentication
  - Rate limiting
  - Encrypted storage of sensitive data

---

## 5. Technology Stack

### 5.1 Frontend
- React / Next.js
- Tailwind CSS
- CodeMirror for coding editor

### 5.2 Backend
- Java Spring Boot (your strength)
- Node.js optional microservices
- Python ML microservices if needed

### 5.3 Database
- MongoDB (user profile, plans, progress)
- PostgreSQL (structured data)
- Redis (caching)

### 5.4 AI Models
- NLP models for:
  - career guidance
  - study planning
  - code analysis
- OCR for scanning questions

### 5.5 Deployment
- Docker + Kubernetes
- AWS/GCP/Azure

---

## 6. Acceptance Criteria
- User can generate a career report in < 1 minute.
- AI can generate a full study plan in < 10 seconds.
- Coding tutor must detect errors in < 2 seconds.
- Plans should adapt automatically when user misses tasks.
- System must work smoothly on mobile and desktop.

---

## 7. Constraints
- Data privacy for minors.
- Should work on low-end devices.
- Limited network reliability in India (offline cache needed).

---

## 8. Future Scope
- Add multi-language support (Hindi, Marathi, Tamil...).
- Add internship recommendation engine.
- Add AI-powered visually interactive lessons.
- Include resume builder, portfolio builder.
