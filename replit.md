# NameVerse API Documentation

## Overview
This is a Node.js/Express web application that serves as the documentation and testing interface for the NameVerse API. The API provides access to a comprehensive database of 70,000+ names across Islamic, Hindu, and Christian traditions with detailed information including meanings, origins, lucky days, personality traits, and more.

## Project Structure
```
NameMeaningApiDocumentation/
├── components/          # YAML component definitions
├── docs/               # Documentation HTML pages
├── paths/              # API path definitions
├── src/                # Source HTML files for endpoints
├── index.html          # Main landing page
├── server.js           # Express server
├── package.json        # Node.js dependencies
└── openapi.yaml        # OpenAPI specification
```

## Tech Stack
- **Backend**: Node.js with Express.js
- **Frontend**: HTML, CSS (TailwindCSS CDN), Vanilla JavaScript
- **Port**: 5000 (configured for Replit environment)
- **Host**: 0.0.0.0 (allows proxy access)

## Setup
The project has been configured to run in the Replit environment:
1. Node.js 20 is installed
2. Dependencies installed via npm
3. Server configured to run on 0.0.0.0:5000
4. Workflow created to start the server automatically

## Deployment
Configured for autoscale deployment with the command: `npm start`

## Recent Changes (December 01, 2025)
- Fixed syntax error in server.js (missing comma on line 25)
- Updated server to bind to 0.0.0.0:5000 for Replit environment
- Created workflow for automatic server startup
- Added .gitignore for Node.js projects
- Configured deployment settings for production

## Available Endpoints
- `/` - Main documentation landing page
- `/docs` - API documentation
- `/blog` - Blog page
- `/getnames` - Get names endpoint testing
- `/getnamesbysearch` - Search names by query
- `/getnamesbyletter` - Filter names by starting letter
- `/getnamesbyreligion` - Filter names by religion
- `/getfilteroptions` - Get available filter options
- `/names/:religion/:name` - Get specific name by religion and slug
- `/api/names` - API endpoint for retrieving filtered names
- `/health` - Health check endpoint

## API Features
- 70,000+ names across religions
- 50+ origins (Arabic, Sanskrit, Hebrew, etc.)
- Deep meanings and interpretations
- Lucky days and numbers
- Personality traits
- Filter by religion, alphabet, and more
