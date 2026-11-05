# Puffwood Junction

A cozy model railway game that runs in the browser. Lay track, connect towns and industries, carry cargo, and run your trains automatically or drive them yourself.

## Play

Open `index.html` in a browser. Everything is in that one file and it needs no build step.

## Features (first playable version)

- A random valley each game: towns, lakes, forests, farms, mines and factories, with a day and night cycle
- Drag-to-build track with automatic curves, junctions with clickable switches, bridges and stations
- Three engines and six car types, with paint colours
- Automatic routes with "wait for full load", or a Drive mode with throttle, brake, reverse and horn
- Supply chains (grain to food, logs to lumber, coal to power) and towns that grow from Hamlet to City
- Goals, rewards, synthesised sound effects and an autosave in the browser

## Controls

- Drag or right-drag to pan, scroll or pinch to zoom
- Keys 1 to 6 switch tools, Space pauses
- When driving: W/S throttle, B brake, R reverse, H horn

## Code layout

`index.html` holds three parts: the simulation (`G` game state, track graph, trains, economy), a top-down 2D renderer, and the DOM interface. The simulation never touches the canvas, so a 3D renderer can be added later using the same data.
