# Trackly

![CI](https://github.com/abdullinmm/trackly/actions/workflows/go.yml/badge.svg)
![Go version](https://img.shields.io/badge/Go-1.21-blue)
![License](https://img.shields.io/badge/license-MIT-green)

Trackly is a personal habits and productivity microservices platform. Designed as a scalable, event-driven system with modern DevOps practices, supporting multi-channel reminders, progress analytics, and extensible integrations.

---

## Key Features

- User registration and authentication (email/password, JWT)
- CRUD for habits, goals, challenges
- Marking and tracking habit completions (daily, weekly, etc.)
- Multi-channel notifications: Telegram bot, email (easily extensible)
- Progress and analytics reports (streaks, productivity charts)
- REST API for web/mobile clients (OpenAPI coming soon)
- Event-driven communication via Kafka or RabbitMQ
- Modular microservice architecture: api-gateway, habits-service, auth, notifications, stats, worker, bot
- Containerized development and deployment (Docker Compose)
- Automated CI: tests, build, lint for all services

---

## Project structure

- `api-gateway/` - API ingress for frontend/web/mobile clients
- `auth-service/` - JWT authentication, user management
- `habits-service/` - Core domain: habits & goals logic
- `notification-service/` - Email, Telegram notifications, extensible channels
- `stats-service/` - Analytics, streaks, progress charts
- `bot-service/` - Telegram bot integration
- `worker-service/` - Background jobs (reminders, batch imports)
- `.github/go.yml` - GitHub Actions: build, lint, tests for all services

---

## Quick Start

- clone and cd into the repo
- docker compose up --build # (planned — add docker-compose.yml)

- or to build/test all services:
- for svc in api-gateway auth-service habits-service stats-service notification-service bot-service worker-service; do
- cd $svc && go build -v ./... && go test -v -race -cover ./... && cd ..
- done

*Instructions for local orchestration and API examples are coming soon.*

---

## Roadmap

- [ ] Add docker-compose deployment for all services
- [ ] OpenAPI documentation & Postman collection
- [ ] End-to-end integration tests across services
- [ ] Example front-end (React/Vue)
- [ ] Advanced analytics and visualization module
- [ ] Demo deployment (Render/Railway)

---

## License

MIT © Marsel Abdullin

---

## Contacts

- Email: abdullinmm@gmail.com
- Telegram: [@abdullin_marsel](https://t.me/abdullin_marsel)
- LinkedIn: [marsel-abdullin-291238121](https://www.linkedin.com/in/marsel-abdullin-291238121/)
