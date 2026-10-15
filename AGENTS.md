# StudyConnect Rwanda — Base44 Dev Environment

## Overview
This is a **static single-page HTML prototype** (`index.html`). All data is stored in the browser via `localStorage`. There is no backend, database, build step, or package manager.

## Running
```bash
docker compose -f docker-compose.base44.yml up -d
```
Serves `index.html` via nginx:alpine on host port 3000.

## Verification
- `curl -s http://localhost:3000/` returns the HTML page with `<title>StudyConnect Rwanda</title>`.
- The app loads an auth screen; create a demo account (Student/Teacher/Admin) to enter the dashboard.

## No secrets required
The app has no external service dependencies.
