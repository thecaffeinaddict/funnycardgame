# Balatro - Love.js Game

## Overview
This is a web-based game built with LÖVE 2D game framework, compiled to WebAssembly using love.js. The game runs entirely in the browser.

## Project Structure
- `index.html` - Main HTML page that loads the game
- `love.js` - Love.js runtime (LÖVE 2D to WebAssembly)
- `love.wasm` - WebAssembly binary for LÖVE engine
- `love.worker.js` - Web Worker for game processing
- `game.js` - Game data loader
- `server.js` - Static file server for development
- `theme/` - CSS and assets for the page

## Running the Project
The project uses a Node.js static file server on port 5000.

Run command: `node server.js`

## Technical Notes
- The server includes COOP/COEP headers for SharedArrayBuffer support
- Cache-Control headers are disabled for development
- Game data (~89MB) is downloaded and cached in IndexedDB on first load

## Recent Changes
- 2026-01-05: Initial setup for Replit environment with static file server
