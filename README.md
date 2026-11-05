# Puffwood Junction

A cozy 3D model railway game that runs in the browser. Your layout sits on a workshop table as four baseboards, each a different region. Lay track, connect towns and industries, and run your trains automatically or drive them yourself.

## Play

Open `index.html` in a browser. It loads three.js from a CDN, so it needs an internet connection; there is no build step.

## Regions

| Baseboard | Look | Industries | Unlock |
|---|---|---|---|
| Clover Meadows | Green fields, cottages, ponds | Farms, Food Plant | Start |
| Ember Woods | Autumn forest, timber lodges, boulders | Lumber Camps, Sawmill | 9,000 |
| Redrock Canyon | Layered mesas, cacti, adobe homes | Quarries, Coal Mine | 18,000 |
| Frostpine Peaks | Snowy peaks, frozen lake, chalets | Coal Mine, Power Station, Lumber Camp | 30,000 |

Sealed baseboards show as bare plywood with the plan pencilled on. Unlocking one makes it rise into place.

## Features

- Drag-to-build track with automatic curves, junctions with switch lamps, bridges, buffer stops and stations
- Four engines (Puffer, Mogul, Comet, Dash Diesel) and six car types, with visible cargo loads and paint colours
- Automatic routes with "wait for full load", or Drive mode with throttle, brake, reverse and horn
- Supply chains that cross regions, and towns that grow from Hamlet to City
- Day and night lighting, steam and smoke, falling snow and leaves, a tilt-shift "model photo" blur
- Goals, rewards, synthesised sound and an autosave in the browser

## Controls

- Drag to pan, right-drag or Q/E to turn, scroll to zoom (touch: drag, pinch, twist)
- Keys 1 to 6 switch tools, Space pauses
- When driving: W/S throttle, B brake, R reverse, H horn

## Code layout

`index.html` holds the simulation (`G` game state, regions, track graph, trains, economy), a three.js renderer that builds the diorama from that state, and the DOM interface with a 2D overlay for labels.
