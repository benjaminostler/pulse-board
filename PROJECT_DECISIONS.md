```md
# Project Decisions (PulseBoard)

## Primary Goal
Build a production-style portfolio project that demonstrates:
- TypeScript end-to-end
- Dockerized local dev
- Automated testing
- CI/CD with GitHub Actions
- AWS deployment

## Stack
- Frontend: React + TypeScript
- Data fetching: React Query
- Backend: Express + TypeScript
- DB: PostgreSQL
- Testing: Jest + React Testing Library (web), Jest + Supertest (api)
- Local Dev: Docker + Docker Compose
- Cloud: AWS (S3/CloudFront, ECS/ECR, RDS)

## Monorepo Structure
- apps/web
- services/api
- packages/shared
- infra/aws