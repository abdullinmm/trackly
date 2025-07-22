Trackly — Personal Habits & Progress Platform

Technical Specification (TЗ)

Project purpose: A modern microservices platform to track personal habits, goals, and productivity with reminders and analytics.

Core Features

User registration and authentication (email/password, JWT tokens)
CRUD operations for habits, goals, and challenge management
Mark habit completions with flexible timeframes (daily, weekly)
Multi-channel reminders: Telegram bot, email (extensible to push)
Progress reports and analytics including streak tracking
OpenAPI/REST API for web and mobile clients
Event-driven architecture using Kafka or RabbitMQ between services
Containerized deployment with Docker and local orchestration via docker-compose
Comprehensive automated CI/CD pipeline
