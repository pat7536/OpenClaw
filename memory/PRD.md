# MoltBot Installation PRD

## Installation Date
February 2026

## What Was Done
- Retrieved Emergent LLM key via emergent_integrations_manager
- Executed MoltBot installation script from https://moltbot.emergent.to/install.sh
- Script installed dependencies, configured environment, built frontend, and started services
- **Added Brave Search API integration** for web search capabilities

## Services Status
- **Backend**: RUNNING
- **Frontend**: RUNNING  
- **MongoDB**: RUNNING
- **nginx-code-proxy**: RUNNING

## Configuration Applied
- LLM key configured in /app/backend/.env
- Preview URLs configured in /app/frontend/.env
- Frontend production build created
- **BRAVE_API_KEY** configured for web search

## Integrations
### Brave Search API
- **Endpoint**: POST `/api/search`
- **Features**: Web search with customizable result count, pagination, country/language filters
- **Request**: `{"query": "search term", "count": 10, "offset": 0}`
- **Response**: Returns titles, URLs, descriptions, and extra snippets

## Reference
- Tutorial: https://emergent.sh/tutorial/moltbot-on-emergent

## Next Steps
- Explore MoltBot features
- Use Brave Search API for web search queries
- Configure additional settings as needed
- Review tutorial for advanced usage
