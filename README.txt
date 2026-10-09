QALA RP 3D — Android-friendly prototype

WHAT WORKS
- 3D city and third-person follow camera
- Touch movement and camera drag on phone
- Jump, job button and money counter
- Basic multiplayer WebSocket client/server code (other players appear when connected)

IMPORTANT
The game is not a finished Black Russia clone, and multiplayer does NOT work until you host server.js on a public server. The browser page uses Three.js from a CDN, so internet is needed.

RUN MULTIPLAYER SERVER
1. Install Node.js 18 or newer on a computer/server.
2. In this folder run: npm init -y
3. Run: npm install ws
4. Run: node server.js
5. Host index.html over HTTPS using any static web host.
6. Open the hosted game with ?server=wss://YOUR-SERVER-HOST (your hosting must provide secure WebSocket/WSS; plain ws may be blocked on HTTPS pages).

This package includes a simple server for testing. Do not expose it publicly without adding validation/rate limits.
