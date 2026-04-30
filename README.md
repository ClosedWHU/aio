# ClosedWHU AIO (All-In-One) Stack

This repository manages the deployment and infrastructure for the ClosedWHU ecosystem.

## Services
- **Infrastructure**: PostgreSQL (pgvector), Redis.
- **Backends**: SSO, Dugout, Ham Gateway, WHU.sb API, WHU.sb Queue.

## Quick Start
1. Copy `.env.example` to `.env` and configure your passwords.
2. Run `docker compose up -d`.

## CI/CD
Images are built automatically on release or can be triggered manually via GitHub Actions.
Images are pushed to Docker Hub under the `closedwhu/` organization.

### Workflow Inputs
- `service`: Choose to build all services or a specific one (`sso`, `dugout`, `ham-gateway`, `whu-sb`).
