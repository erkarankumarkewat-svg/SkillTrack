# SkillTrack India 🇮🇳

### Smart India Hackathon Prototype
**Problem Statement:** PS26135 — Skilling Outcomes Tracking System

SkillTrack India is a prototype platform designed to track the **real-world outcomes of skilling and vocational training programs** beyond enrolment, attendance, assessment, and certification.

It connects training records with post-training outcomes such as **employment, self-employment, apprenticeships, employer verification, wage progression, retention, and follow-up status**.

> **Prototype Notice:** This repository uses configured/demo data to demonstrate the proposed product workflow, architecture, UX, and outcome-tracking approach. It is not a production government system.

---

## 🎯 Problem

Training systems can record enrolment, attendance, assessment, and certification, but post-training outcomes are often incomplete or fragmented.

Important questions include:

- Did the trainee get a job?
- Is the trainee still employed?
- Did the trainee become self-employed?
- How did wages change?
- Was employment verified?
- Was the training relevant to the job?
- Which courses and providers are producing sustainable outcomes?
- Where are skill and outcome gaps concentrated?

SkillTrack India proposes a unified outcome-tracking layer to help answer these questions.

---

## 💡 Solution

The platform connects:

```text
Training
   ↓
Assessment & Certification
   ↓
Outcome Follow-up
   ↓
Employment / Self-Employment / Apprenticeship
   ↓
Verification
   ↓
Retention & Wage Tracking
   ↓
Outcome Analytics
```

---

## ✨ Key Features

### Trainee Outcome Passport
- Training history
- Certification
- Employment status
- Self-employment outcomes
- Follow-ups
- Employer verification
- Wage records
- Retention information
- Outcome status

### Employment & Self-Employment Tracking
Track post-training livelihood outcomes, employment information, job role, employer details, and configured self-employment/income outcomes.

### Employer Verification
Employers can participate in the outcome-verification workflow to improve confidence in reported employment outcomes.

### Follow-up Management
Structured follow-ups help capture outcome information after training and certification.

### Wage & Retention Tracking
Track configured wage records and employment retention over time.

### Analytics
Explore outcome information by:
- Cohort
- Course
- Training provider
- District
- Employment status
- Outcome status
- Retention

### Geographic Insights
The prototype includes state/district-oriented views for training and outcome insights.

### Role-Based Access Control
Authentication and protected API routes separate access according to stakeholder roles.

---

## 👥 Demo Personas

| Persona | Purpose |
|---|---|
| **Admin** | System-level visibility and administration |
| **District User** | District-level analytics and monitoring |
| **Training Provider** | Training and trainee workflows |
| **Employer** | Employment/outcome verification |
| **Trainee** | Personal outcome information and journey |

> Demo accounts are for local/prototype testing only. Never publish real credentials or secrets.

---

## 🖥️ Main Modules

1. Authentication
2. Dashboard
3. Trainee Management
4. Outcome Tracking
5. Trainee Outcome Passport
6. Follow-up Management
7. Employer Verification
8. Wage & Retention Tracking
9. Training Provider Insights
10. State/District Analytics
11. Skill Gap / Outcome Insights
12. Role-Based Access Control

---

## 🏗️ Technology Stack

**Frontend**
- HTML5
- Tailwind CSS
- JavaScript
- Lucide Icons
- Chart.js
- Leaflet

**Backend**
- Node.js
- Express
- TypeScript
- REST APIs

**Database**
- PostgreSQL-compatible Prisma data model
- Prisma ORM

**Security**
- JWT authentication
- Role-Based Access Control
- Protected API routes
- Consent-oriented outcome records

---

## 📁 Project Structure

```text
skill-track-india/
├── backend/
│   ├── prisma/
│   │   ├── schema.prisma
│   │   └── seed.ts
│   ├── src/
│   │   ├── routes/
│   │   ├── controllers/
│   │   ├── services/
│   │   └── ...
│   ├── public/
│   ├── package.json
│   └── tsconfig.json
├── docs/
├── README.md
└── ...
```

> The exact structure can vary between prototype versions.

---

## 🚀 Run Locally

### Prerequisites

- Node.js 18+
- npm
- PostgreSQL for production-style deployment

### Clone

```bash
git clone https://github.com/erkarankumarkewat-svg/skill-gap-SIH-Ps.git
cd skill-gap-SIH-Ps
```

### Install

```bash
cd backend
npm install
```

If the repository contains a separate frontend package:

```bash
cd ../frontend
npm install
```

### Environment

Create the required backend `.env` file.

Example:

```env
PORT=5000
DATABASE_URL="your-database-url"
JWT_SECRET="replace-with-a-secure-secret"
```

**Never commit real secrets, database credentials, API keys, or production `.env` files.**

### Prisma

```bash
npx prisma generate
```

### Seed demo data

```bash
npm run seed
```

### Start backend

```bash
npm run dev
```

Backend:

```text
http://localhost:5000
```

Health check:

```text
http://localhost:5000/api/v1/health
```

### Start frontend

From the frontend directory:

```bash
npm run dev
```

The prototype uses the port configured in the project, typically:

```text
http://localhost:3000
```

---

## 🧪 Testing

Useful validation commands:

```bash
npm run build
npx prisma validate
npm run seed
```

The prototype has been tested across important workflows including:

- Authentication
- Role-based access
- Outcome workflows
- Analytics
- Follow-ups
- Employer/outcome verification
- Database interactions

---

## 🔐 Security & Data Principles

### Role isolation
Users should only access information permitted by their role.

### Consent-oriented collection
Outcome information should be collected and used through appropriate consent and governance mechanisms.

### Minimal exposure
Analytics should avoid unnecessary exposure of personally identifiable trainee information.

### Auditability
Important workflow actions should be traceable.

### No fabricated outcomes
Configured demonstration data is distinguished from real-world outcome data.

---

## 📈 Future Scope

Possible future extensions include:

- Verified employment-data integrations
- Secure government identifier integrations
- Automated follow-up channels
- Employer API integrations
- Advanced outcome verification
- Longitudinal wage analytics
- Predictive skill-gap analysis
- District-level benchmarking
- Production-grade evidence/document storage
- Notification integrations
- Stronger consent and privacy controls
- Production monitoring and audit infrastructure

These are future possibilities and are **not claimed as implemented production capabilities**.

---

## 🎬 Prototype Journey

```text
Training
   ↓
Certification
   ↓
Follow-up
   ↓
Employment / Self-Employment
   ↓
Verification
   ↓
Retention
   ↓
Wage Progression
   ↓
Outcome Analytics
```

The demonstration uses configured data to show how different stakeholders can interact with the platform and how outcome information can be consolidated for monitoring and decision support.

---

## 🏆 Smart India Hackathon

**Project:** SkillTrack India  
**Problem Statement:** PS26135 — Skilling Outcomes Tracking System  
**Event:** Smart India Hackathon  
**Type:** Software Prototype

The project focuses on moving beyond simply measuring **how many people were trained** toward understanding **what happened after training**.

---

## ⚠️ Disclaimer

This repository contains a **hackathon prototype**.

It uses configured/demo data and simplified workflows to demonstrate the proposed solution. It should not be interpreted as a production implementation, official government service, legal determination, or authoritative source of employment, certification, or beneficiary information.

Any government, identity, employment, or regulatory integration would require appropriate authorization, security review, privacy controls, data governance, and official APIs/sources before production deployment.

---

## 👥 Team

Developed as a **Smart India Hackathon prototype** for the Skilling Outcomes Tracking System problem statement.

---

## 📄 License

Add the license applicable to your team/project before publishing this repository publicly.
