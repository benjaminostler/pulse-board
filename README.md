# PulseBoard

PulseBoard is a production-style full-stack analytics dashboard for tracking metrics over time (projects, metrics, daily check-ins, and trends).  
This repo is intentionally built to demonstrate modern software engineering practices: TypeScript end-to-end, containerized local development, automated testing, CI/CD, and AWS deployment.

## Tech Stack

**Frontend**
- React + TypeScript
- React Query (server-state management)
- Recharts (data visualization)

**Backend**
- Node.js + Express + TypeScript
- REST API

**Database**
- PostgreSQL

**Engineering / DevOps**
- Docker + Docker Compose (local dev)
- GitHub Actions (CI/CD)
- AWS (deployment target: S3/CloudFront for web, ECS/ECR for API, RDS for Postgres)

## Project Status

This project is under active development. Current goals:
- [ ] Monorepo scaffold (web + api + shared types)
- [ ] Dockerized local development (web + api + db)
- [ ] Basic end-to-end flow (web ↔ api ↔ db)
- [ ] Testing (Jest + RTL for web, Jest + Supertest for API)
- [ ] CI/CD via GitHub Actions
- [ ] Deployment to AWS

## Repo Structure (Planned)

pulse-board/
apps/
web/ # React + TypeScript frontend
services/
api/ # Express + TypeScript backend
packages/
shared/ # Shared TypeScript types (DTOs)
infra/
aws/ # Deployment notes / IaC (later)
.github/
workflows/ # CI/CD pipelines (later)


## Setup (Coming Soon)

Once scaffolding is complete, local development will be a single command:

```bash
docker compose up --build
