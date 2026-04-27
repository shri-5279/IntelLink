# IntelLink — AI-Powered URL Intelligence Platform

> AI-powered URL shortener with malicious link detection, real-time 
> click analytics, and intelligent performance insights — built on AWS

## Why IntelLink Exists

Phishing and malicious links are distributed daily through shortened
URLs — because shorteners hide the destination. IntelLink solves this
by scanning every URL with AI before shortening it, giving users a
safety score and detailed analytics on every link they create.

## Architecture

[Diagram coming in Phase 7]

## Tech Stack

| Layer | Technology |
|-------|------------|
| Backend API | Python, FastAPI |
| Database | PostgreSQL |
| Cache | Redis |
| Message Queue | AWS SQS |
| AI Layer | Claude API (Anthropic) |
| Infrastructure | AWS EC2, Terraform, Ansible |
| Containers | Docker, Docker Compose |
| CI/CD | GitHub Actions |
| Monitoring | Prometheus, Grafana |

## Key Features

- URL shortening with base62 encoding
- AI-powered malicious URL detection before every shorten
- Real-time click analytics: device, browser, country, city, referrer
- AI-generated insights explaining link performance trends
- Intelligent routing by device type and geography
- Redis caching with cached safety scan results
- JWT user authentication and URL ownership
- Rate limiting via sliding window algorithm
- Full observability: Prometheus metrics, Grafana dashboards

## Local Development

```bash
docker compose up --build
```

API available at: http://localhost:8000  
Interactive API docs: http://localhost:8000/docs

## Project Status

- [x] Phase 0: Environment setup
- [ ] Phase 1: Core API
- [ ] Phase 2: Auth & Users
- [ ] Phase 3: Analytics Pipeline
- [ ] Phase 4: AI Safety Layer
- [ ] Phase 5: Redis Caching
- [ ] Phase 6: Smart Insights Engine
- [ ] Phase 7: Terraform Infrastructure
- [ ] Phase 8: CI/CD Pipeline
- [ ] Phase 9: Intelligent Routing
- [ ] Phase 10: Monitoring
- [ ] Phase 11: React Frontend
