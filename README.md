# 🚀 Mission Control — Backend API Engineering Challenge

Welcome! This repository contains a take-home backend API assessment designed to evaluate your API design, data modeling, system architecture, and testing skills.

Your goal is to build a backend service that consumes public data from the NASA Image and Video Library API and exposes your own well-designed REST (or GraphQL) API with meaningful functionality.

The NASA Image and Video Library API provides searchable metadata, images, videos, and audio from NASA’s public archives. No authentication is required.

---

## 🛰️ Base API Information

NASA Image & Video Library API Documentation:  
https://images.nasa.gov/docs/images.nasa.gov_api_docs.pdf

Base URL:
https://images-api.nasa.gov

Example Available Endpoints:

- `GET /search?q={query}` — Search NASA media
- `GET /asset/{nasa_id}` — Retrieve asset manifest
- `GET /metadata/{nasa_id}` — Retrieve metadata
- `GET /captions/{nasa_id}` — Retrieve caption files

You are free to use any endpoints available in the NASA Image and Video Library API.

---

## 📌 Required Features

Implement **at least three (3)** of the following features (or design your own equally complex alternatives), as well as document the work as outlined below in the Documentation section.

### 1️⃣ Integrate with at Least 3 NASA Endpoints

Your implementation must integrate with **at least three different endpoints** from the NASA Image and Video Library API.

Below are example feature ideas:

---

### Example: Enhanced Media Search

GET /media/search

Wrap NASA’s `/search` endpoint and:

- Normalize the response structure  
- Support filters (year, media_type, keywords)  
- Limit and paginate results  
- Sort by date  

---

### Example: Media Detail Aggregator

GET /media/:nasa_id

Combine data from:

- `/asset/{nasa_id}`
- `/metadata/{nasa_id}`

Return a single enriched object including:
- Title  
- Description  
- Media URLs  
- Date created  
- Photographer or NASA center  
- Related keywords  

---

### Example: Yearly Archive Summary

GET /analytics/year/:year

Return:
- Total media items for that year  
- Breakdown by media type (image, video, audio)  
- Top 5 most common keywords  

---

### Example: Topic Insights

GET /analytics/topic/:keyword

Return:
- Total matching media results  
- Oldest and newest items  
- Distribution by media type  

---

### Example: Dashboard Endpoint

GET /dashboard

Expose a combined view including:
- Most recent Mars-related image  
- Total results for “Apollo”  
- Media type distribution for a chosen keyword  

---

You are encouraged to design your own endpoints if they demonstrate similar complexity and thoughtful data modeling.

---

## 📘 Documentation

Create a second `README.md` in your submission repository that should include:

### 📌 Setup Instructions
- How to install dependencies  
- How to run the application  
- How to run tests  

### 📌 API Endpoints
For each endpoint you create:
- URL  
- Method  
- Description  
- Example request  
- Example response  

### 📌 Design Decisions
- Why you chose your framework  
- Project structure  
- Performance or scaling considerations  
- Trade-offs made  
- What you would improve with more time  

---

## 🧪 [BONUS] Testing

Include tests that cover your API integrations:

- Valid responses  
- Edge cases  
- Error handling  
- Invalid inputs  

Tests may be unit tests, integration tests, or both.

---

## 📤 Submission Instructions

1. Fork this repository  
2. Complete your implementation  
3. Push your solution to your fork  
4. Send us the link — do not submit a ZIP file  

---

## ⏱ Time Expectation

We estimate this challenge should take **3–6 hours**, depending on your familiarity with the stack you choose.

Focus on clarity and thoughtful design — it’s not about finishing every possible feature. Show us how you think.

---

Have fun with it, and we look forward to seeing your solution! 🚀
