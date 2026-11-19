# pixel-farm

A web-based real-time pixel farm game - plant, grow, and (playfully) steal vegetables with friends. Inspired by classic social farm games and cozy farming games, built as a lightweight web project to run on an idle home server.

## Gameplay
- Plant seeds, water, and wait for crops to mature on a timed growth cycle
- Visit friends' farms in real time and steal ripe crops
- Cozy pixel-art style, played entirely in the browser

## Tech Stack
- Backend: Go - high-concurrency WebSocket server for real-time state sync between farms/players
- Frontend: Vite + Canvas (pixel rendering), TypeScript - simple pixel-art UI, no heavy framework
- Data: SQLite for persistent farm/crop state, Redis optional for online presence / short-lived session and anti-cheat rate limiting
- Crop logic: server-side maturation timers, server-validated harvest/steal actions to prevent cheating

## Devin Workflow
1. Devin Bot works in this repo via pull requests
2. Step 1: Scaffold Go WebSocket server + project layout
3. Step 2: Scaffold Vite + Canvas frontend and pixel farm grid
4. Step 3: Crop planting / growth timer / harvest logic
5. Step 4: Real-time visit + steal mechanic with server validation
6. Step 5: Deployment scripts for a small idle server

## Assets
- Open-source pixel art asset packs (crops, tiles, characters) - to be selected, with license noted in repo

## Deployment
- Phase 1: Private play with a few friends
- Phase 2: Deploy on idle server, consider a dedicated domain for public access, with basic ops / restart scripts

## Status
Project scaffold - README first, code coming via Devin PRs.
