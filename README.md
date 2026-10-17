# Autonomous Warehouse Robot Navigation

Dijkstra's-algorithm pathfinding for a warehouse robot on a grid map. A team final project.

## What it does

- Models a warehouse as a grid: `S` start, `D` destination, `X` obstacles, `P` priority pathways, `.` open floor.
- Finds the lowest-cost path with Dijkstra's algorithm. Priority pathways and upward/leftward moves cost less (0.5), so the planner prefers them.
- Visualizes the computed path over the grid.

## Files

- `main.ipynb` - the main project notebook: the pathfinder plus four test cases (no obstacles, obstacles present, priority pathways, and no-path). Visualizes with matplotlib and numpy.
- `mapbuildingsim.py` - interactive warehouse map builder and pathfinder built with pygame. Draw your own map, then press SPACE to run the pathfinder (ESC to quit).
- `main.py` - standalone script version of the pathfinder (matplotlib).
- `warehouseminigameREAL.py` - a terminal minigame on the same pathfinder: reach the destination within a move limit, with an optimal-path comparison at the end.

## Run it

```
pip install numpy matplotlib pygame
jupyter notebook main.ipynb      # main project
python mapbuildingsim.py         # interactive map builder
python warehouseminigameREAL.py  # terminal minigame
```

## Team

Aakash Kumar, Maseo Jagat, Owen Callaway, Akshan Bhelkar, Kaushik Gunasekaren
