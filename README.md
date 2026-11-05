# Puffwood Junction

A cozy model railway game that runs in the browser. Four model railway tables stand on a workshop floor, one region each. Lay track over hills and valleys, connect towns and industries, and earn the bridges and tunnel that join the tables.

## Play

Open `index.html` in a browser. Everything is in that one file and it needs no build step.

## How it plays

- **Tables and contracts.** You start on Clover Meadows. Each table has contracts. Crossing contracts build the bridge or tunnel to the next table, and the materials often come from another table, so you run trains between them.
- **Terrain.** Each table is built from layered terraces: hills, valleys, rivers, a canyon and snowy peaks. Track climbs one level per tile. Dragging across a deep valley or river builds a bridge; dragging through a hill bores a tunnel. Trains slow down going uphill.
- **Trains.** Automatic routes with "wait for full load", or Drive mode with throttle, brake, reverse and horn.

| Table | Industries | Reached by |
|---|---|---|
| Clover Meadows | Farms, Food Plant, Lumber Camp | Start |
| Ember Woods | Lumber Camps, Sawmill | Ember Bridge (logs) |
| Frostpine Peaks | Coal Mines, Power Station, Lumber Camp | Frostpine Tunnel (lumber + food) |
| Redrock Canyon | Quarries, Farm | Redrock Viaduct (coal + lumber) |

## Controls

- Drag to pan, scroll or pinch to zoom
- Keys 1 to 6 switch tools, Space pauses
- When driving: W/S throttle, B brake, R reverse, H horn

## Code layout

`index.html` holds the simulation (`G` game state, tables, heights, track graph with levels, trains, economy, contracts), a 2D renderer that bakes each table's terrain into row strips and draws everything back to front in an oblique top-down view, and the DOM interface.
