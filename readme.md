# Single Dice Roller WebService

A Node.js based web service that implements a simple dice roller application with server-side random number generation.

## Features

- RESTful API for rolling a single 6-sided die
- All random numbers generated on the server
- CORS policy implementation
- Simple and clean user interface

## API Endpoint

### Roll a single 6-sided die
```
GET /api/roll
```
Response:
```json
{
  "value": 4,
  "timestamp": "2025-03-02T12:34:56.789Z"
}
```

Note: All other API endpoints are disabled.

## CORS Configuration

The server implements CORS protection that:
- Allows requests from specified origins (`localhost:3000` and `127.0.0.1:3000`)
- Blocks requests from all other origins
- Supports the GET method only
- Allows credentials to be included in requests

## Setup and Installation

1. Clone this repository
2. Install dependencies:
   ```
   npm install
   ```
3. Start the server:
   ```
   npm start
   ```
4. For development with auto-restart:
   ```
   npm run dev
   ```
5. Open your browser and navigate to http://localhost:3000

## Project Structure

- `server.js` - Main server file that implements the RESTful API and CORS policy
- `public/index.html` - Simple user interface for rolling a single die
- `public/` - Directory for static files
