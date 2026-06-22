# 🎫 Prestige Planner — Smart Event Management Ecosystem

<div align="center">
  <p><strong>A comprehensive event management ecosystem integrating Microservices architecture and AI-optimized solutions.</strong></p>
</div>

---

## 📖 About the Project

**Prestige Planner** is not just a traditional event management system, but a **Smart Event Ecosystem**. The project applies a Microservices architecture combined with the latest Generative AI technologies to automate the operational workflows for Organizers and deliver a seamless, intelligent interactive experience for Attendees.

## ✨ Key Features

### 🎯 1. Core Business Features
* **Account Management & Role-based Access:** Secure authentication system (JWT) with clear authorization roles among Admins, Organizers, and Attendees.
* **Comprehensive Event Management:** Supports creating, editing, scheduling, and managing event content (location, time, descriptions, images).
* **Ticketing & Checkout:** Smooth ticket booking process supporting multiple ticket types (VIP, Standard) and integrated with online payment gateways (Momo/VNPay).
* **QR Code Check-in:** Automatically generates QR codes for each ticket, allowing Organizers to scan and check-in attendees quickly at the event.
* **Dashboard & Statistics:** Visual dashboard tracking revenue, ticket sales, and registration charts in real-time.

### 🤖 2. AI Integrations
* **RAG-based Customer Support Agent:** AI automatically comprehends event documents (PDF schedules, rules) vectorized via pgvector to accurately answer attendee questions without hallucinations.
* **Autonomous Agent (Tool Calling):** The chatbot can automatically execute system tasks via chat, such as: looking up ticket information, displaying QR codes, or resending confirmation emails.
* **AI Organizer Co-Pilot:** Generates the entire event (SEO-optimized descriptions, detailed schedules) from a simple prompt.
* **Feedback Analytics:** Performs sentiment analysis on thousands of post-event reviews, automatically sending apology emails and discount vouchers for negative feedback.

## 🛠 Tech Stack

### Frontend
* **React** - Building dynamic user interfaces (SPA)
* **Tailwind CSS / Material-UI** - Modern, responsive UI/UX design

### Backend & AI
* **Java 17 & Spring Boot 3** - Building robust RESTful APIs
* **Spring AI** - Integrating and managing AI Agents, Prompt Engineering
* **LLMs** - Gemini Pro API / OpenAI GPT-4o / Ollama (Local)

### Database & DevOps
* **PostgreSQL** - Primary relational database
* **pgvector** - Extension for storing Vector Embeddings for RAG
* **Docker & Docker Compose** - Containerization and application deployment

## 📂 Project Structure

```text
Event-Management-Website/ (Root)
├── Event-Management-Website/  # ⚛️ Frontend (React SPA)
├── Event-Management-Backend/  # ☕ Backend (Java Spring Boot 3 + Spring AI)
```

## 🚀 Quick Start Guide

### 1. Start Backend & Database
The system uses Docker to quickly initialize PostgreSQL with pgvector.
```bash
cd Event-Management-Backend
# Start Database (PostgreSQL + pgvector)
docker compose up -d

# Run Spring Boot application
./mvnw spring-boot:run
```

### 2. Start Frontend
```bash
cd Event-Management-Website
npm install
npm run dev
```

## 📑 Documentation & Research
* For detailed system designs and architecture diagrams, see the directory: `docs/`
* AI integration research proposal: `ai_integration_thesis_proposal.md`
