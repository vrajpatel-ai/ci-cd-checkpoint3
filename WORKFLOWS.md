# Workflow Documentation

## CI Pipeline
- **Trigger:** On push (main, develop) & PR to main
- **Jobs:** 
  - Lint → runs ESLint & Prettier check (simulated)
  - Test → runs tests & coverage (simulated)
  - Build → creates build artifact

## Daily Dependency Audit
- **Trigger:** Runs daily at 2 AM UTC
- **Job:** Runs security audit (simulated)

## Deploy to GitHub Pages
- **Trigger:** Push to main
- **Job:** Simulates deployment (echo)

## Secrets
- None required (simulation only)

## Troubleshooting
- Ensure workflows are in `.github/workflows/`
- Check Actions logs if a job fails
- Ensure repo has Actions enabled
