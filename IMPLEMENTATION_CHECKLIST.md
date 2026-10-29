# Implementation Checklist

Build the application yourself using `PROJECT_BRIEF.md`.

## Initial setup

- [ ] Read the project specification.
- [ ] Review the architecture and data model.
- [ ] Create a Python virtual environment.
- [ ] Install and pin the required dependencies.
- [ ] Configure credentials through environment variables.
- [ ] Review the data privacy and security requirements.

## Project acceptance criteria

- [ ] All catalog images processed without error
- [ ] Embedding vectors stored with <0.5 s per image
- [ ] Space overhead <2 × raw image size
- [ ] API responds <1 s for 10 k catalog size
- [ ] Returned items share visual style and match occasion keyword
- [ ] Rationale contains both visual and textual cues
- [ ] Upload works across Chrome/Firefox
- [ ] Recommendations displayed within 2 s of submission
- [ ] No image persisted on server beyond request
- [ ] Initialize repo with Docker Compose (FastAPI, Postgres, Redis)
- [ ] Create product catalog (20‑30 sample images)
- [ ] Implement visual token model loading (pre‑trained checkpoint)
- [ ] Unit tests for tokenization and embedding functions (pytest)
- [ ] Integration tests for /recommend endpoint using FastAPI TestClient
- [ ] Load test with locust (100 concurrent users) to verify latency
- [ ] Security test: ensure uploaded images are deleted after processing
- [ ] Privacy test: confirm no persistent storage of raw uploads
- [ ] Dockerize each component
- [ ] Create docker-compose.yml for local dev
- [ ] GitHub Actions workflow: lint → test → build Docker image → push to Docker Hub
- [ ] Deploy to Render or Fly.io (free tier) with PostgreSQL managed instance and Redis add‑on

## Before completion

- [ ] Implement the planned MVP features.
- [ ] Add unit and integration tests.
- [ ] Run the test suite.
- [ ] Measure the evaluation metrics in the brief.
- [ ] Record actual results and known limitations.
- [ ] Document setup and deployment.
- [ ] Update the README to reflect the implemented features.
- [ ] Add only verified outcomes to your resume.
