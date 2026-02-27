# 🚀 Mission Control — Backend API Engineering Challenge

Welcome! This repository contains a take-home backend API assessment designed to evaluate your API design, data modeling, system architecture, and testing skills.

Your goal is to build a backend service that consumes public data from the **SpaceX API** and exposes your own well-designed REST (or GraphQL) API with meaningful functionality. The public SpaceX API provides rich JSON data including launches, rockets, payloads, launchpads, and more — with no authentication required.

---

## 🛰️ Base API Information

**API Documentation:**  
[https://api.spacexdata.com/v4](https://github.com/r-spacex/SpaceX-API/tree/master)

**Example Endpoints**  
- `GET /launches` — List all launches  
- `GET /launches/:id` — Launch detail  
- `GET /rockets` — Rocket list  
- `GET /capsules` — Capsule list  
- `GET /launchpads` — Launchpad info  

---

## 🧠 Your Mission

Build a backend API that:

✅ Fetches and uses SpaceX public data  
✅ Exposes your own clean API with meaningful endpoints  
✅ Includes data transformation, filtering, and aggregation  
✅ Has documentation and tests  
✅ Handles errors and invalid input gracefully

You may choose **any language or backend framework** (e.g., Node.js, Python, Go, Java/Kotlin, Rust, etc.).

---

## 📌 Required Features

Implement **at least three (3)** of the following features (or design your own *equally complex* ones) as well
as document the work as outlined below in the documentation section:

### 1️⃣ Integrate with 3 endpoints
**Example:**  
GET /launches/upcoming
Return a sorted list of upcoming launches with:
- mission name  
- launch date/time  
- rocket name  
- launch site

Include optional filters (e.g., by year, rocket type, or launch site).

**Example:**  
GET /stats/launches
Return a summary including:
- total launches
- total successful launches
- success rate (%)
- number of upcoming missions

**Example:**  
GET /rockets/usage
Compute rocket-level aggregates:
- number of launches per rocket
- success/failure counts
- earliest and latest launch dates per rocket

**Example:**  
GET /launchpads/:id/activity
For a given launchpad:
- list of launches
- total launches
- success rate

**Example:**  
GET /dashboard
Expose a combined view of:
- next upcoming launch
- most used rocket
- launch success trends (yearly)

---

## 📘 Documentation

Create a second `README.md` that should include:

📌 Setup Instructions  
- how to install dependencies  
- how to run the app  
- how to run tests  

📌 API Endpoints  
- url
- method
- description  
- example request/response

📌 Design Decisions  
- why you chose your framework  
- project structure
- performance or scaling considerations  
- what you would improve with more time

---

## [BONUS] 🧪 Testing

Include tests that cover your API integrations:

✔ Valid responses  
✔ Edge cases  
✔ Error handling  
✔ Invalid inputs

*Tests may be unit tests, integration tests, or both.*

---

## 📤 Submission Instructions

1. **Fork** this repository  
2. Complete your implementation  
3. Push your solution to your fork  
4. Send us the link — **do not submit a ZIP file**

---

## ⏱ Time Expectation

We estimate this challenge should take **3–6 hours**, depending on your familiarity with the stack you choose. Focus on clarity and thoughtful design — it’s *not* about finishing every feature perfectly. Show us reasoning.

---

Have fun with it, and we look forward to seeing your solution! 🚀

---
