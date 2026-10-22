# EECE430 Assignment 5 — Docker AI Inventory Agent

This project is a Django AI Inventory Agent packaged using Docker.

## Requirements
- Docker Desktop
- Gemini API key

## Build the image
```powershell
docker build -t inventory-agent .
```

## Configure the API key
Create a local `.env` file containing:

```text
GEMINI_API_KEY=your_api_key_here
```

Never upload your real API key to GitHub.

## Run the container
```powershell
docker run --rm -p 8000:8000 --env-file .env inventory-agent
```

## Open the application
http://localhost:8000/

The database tables are created automatically at startup. A fresh database starts with no inventory items.
