# scrum-project
Практика по Scrum и Cloud-Native инфраструктуре

## Архитектурная диаграмма

```mermaid
graph TD
  A[Пользователь] --> B[Frontend]
  B --> C[API]
  C --> D[База данных]
  C --> E[CI/CD Pipeline]
  E --> F[Docker Hub]
  E --> G[AWS EC2 (Terraform)]
  C --> H[Мониторинг (Grafana/Sentry)]
  C --> I[Secrets (Vault/GitHub Secrets)]
  I --> J[VPN/SSH доступ к staging]
