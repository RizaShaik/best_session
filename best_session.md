# Best Session — Building MyBlog

## Context

I wanted to move beyond writing standalone programs and understand how different parts of a software system work together.

To explore this, I built MyBlog, a full-stack blogging platform that helped me learn how frontend applications, backend APIs, databases, containers, and local orchestration interact in practice.

Rather than focusing only on features, I treated it as an opportunity to understand end-to-end software development.

## Problem

The goal was to build a platform that could:

- create and manage blog posts
- store and retrieve content persistently
- connect frontend and backend components through APIs
- remain modular and easier to maintain
- run consistently across environments

I also wanted to understand how a system evolves from local development to something closer to a deployment workflow.

## System Design

### Tech Stack

- Frontend: React
- Backend: Node.js
- Database: MongoDB
- Containerization: Docker
- Local orchestration experimentation: Kubernetes (Minikube)

### High-Level Flow

Client Request → React UI → Backend API → MongoDB → Response

The frontend communicates with backend endpoints, which process requests and interact with MongoDB for persistent storage.

## Engineering Decisions

### Why separate frontend and backend?

I kept the frontend and backend independent so I could better understand API interactions and data flow.

This also made debugging easier because I could isolate issues between UI logic, server-side handling, and database operations.

### Why Docker?

Managing dependencies across environments can become inconsistent.

I experimented with Docker to package the application in a reproducible way and better understand how containerized applications run consistently.

### Why Minikube?

I wanted to explore orchestration concepts instead of treating deployment systems as a black box.

Using Minikube locally helped me learn about service configuration, containers, and how multiple application components can be managed together.

## Challenges I Faced

### 1. Frontend–Backend communication

One of the biggest challenges was understanding request/response flow between React and backend APIs.

Debugging data flow issues helped me improve how I approached problem-solving and tracing bugs systematically.

### 2. Data persistence

Working with MongoDB helped me understand the difference between temporary application state and persistent storage.

I learned how data moves across layers and how backend systems manage information reliably.

### 3. Environment consistency

Running projects across environments introduced dependency and configuration challenges.

Experimenting with Docker helped me better understand reproducibility and setup consistency.

## What I Learned

This project helped me think about software as a connected system instead of isolated code.

Key takeaways:

- understanding API-based communication between systems
- thinking in terms of modular software components
- debugging across multiple layers of an application
- learning how containers improve reproducibility
- gaining exposure to orchestration concepts through Minikube

## Why this matters to me

I enjoy understanding how systems work end-to-end rather than treating tools as abstractions.

Building MyBlog strengthened my interest in backend systems, debugging, and software architecture, and made me more curious about how production systems are designed and maintained.

## Repository

GitHub: https://github.com/RizaShaik/my-blog