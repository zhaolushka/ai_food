# FoodBridge / FOOD AI

FoodBridge is a proactive food rescue platform for cafes, canteens, and NGOs in Atyrau.

The core idea is not just listing leftovers, but predicting spoilage risk and triggering early actions:
- warn food providers before quality is lost,
- suggest nearby NGOs that can collect in time,
- track handoff outcomes and impact metrics.

## Project Structure

- `docs/architecture.md` - system architecture and service boundaries
- `docs/mvp-plan.md` - phased MVP delivery plan
- `docs/api-spec.md` - initial API endpoint specification
- `docs/db-schema.md` - core database schema for v1
- `backend/` - Node.js API skeleton
- `frontend/` - web app skeleton
- `ai-service/` - FastAPI risk scoring skeleton
- `docker-compose.yml` - local multi-service orchestration

## Product Positioning

FoodBridge uses AI as an operational decision engine:
- proactive alerts based on spoilage risk,
- recommendation of optimal transfer windows,
- partner matching support for faster rescue flow.

## Initial Partner Targets (Atyrau)

- Corporate canteen networks (oil company contractors)
- City cafes along the embankment
- Foundation partners already connected to food/NGO operations

## Quick Start

1. Install Docker Desktop.
2. Open terminal in `FOOD AI`.
3. Run:
   - `docker compose up --build`
4. Open:
   - Frontend: `http://localhost:3000`
   - Backend health: `http://localhost:4000/health`
   - AI health: `http://localhost:8000/health`
