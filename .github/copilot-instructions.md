# Copilot Instructions

## Project

- This is a small FastAPI application for Mergington High School extracurricular activities.
- The backend entry point is `src/app.py`; the frontend is in `src/static/`.
- Activity and participant data is intentionally stored in memory and resets on restart.
- `.vscode/mcp.json` configures the GitHub MCP server for this exercise; preserve it unless the task explicitly changes MCP setup.

## Run and Validate

- Install dependencies with `pip install -r requirements.txt`.
- Start the app with `uvicorn src.app:app --reload` from the repository root, or use the VS Code launch configuration.
- The web UI is served at `/`; API documentation is at `/docs`.
- For backend changes, validate with a focused HTTP request or Python check when possible. Keep frontend changes compatible with the existing plain HTML, CSS, and JavaScript structure.

## Change Guidelines

- Keep changes focused and preserve the existing public API unless the task requires a contract change.
- Use FastAPI's existing route and error-handling patterns.
- Encode activity names and email addresses in frontend URLs.
- Do not add persistence or new dependencies without a clear requirement.
