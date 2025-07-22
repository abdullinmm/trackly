Trackly — это современная микросервисная платформа для отслеживания привычек, продуктивности и прогресса пользователей. Проект позволяет ставить цели, фиксировать выполнения, получать аналитические отчёты и получать уведомления (email, Telegram)

 Repository Structure

├── api-gateway/
│   ├── cmd/
│   └── internal/
├── auth-service/
│   ├── cmd/
│   ├── internal/
│   └── migrations/
├── habits-service/
│   ├── cmd/
│   ├── internal/
│   └── migrations/
├── stats-service/
│   ├── cmd/
│   └── internal/
├── notification-service/
│   ├── cmd/
│   └── internal/
├── bot-service/
│   ├── cmd/
│   └── internal/
├── worker-service/
│   ├── cmd/
│   └── internal/
├── proto/
├── build/
├── deploy/
│   ├── docker-compose.yaml
│   └── k8s/
├── docs/
│   ├── openapi/
│   └── diagrams/
├── .github/
│   └── workflows/
├── Makefile
└── README.md
