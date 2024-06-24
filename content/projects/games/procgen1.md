---
tags:
  - experiment
  - unity
title: Procedurally generated levels
---
My first attempt at generating dungeon-like levels. Most of my work was based on [this video](https://youtu.be/rBY2Dzej03A?si=uYAzqlvs8MnLNCF3) with a few changes.

![[worldgen.gif]]
### Procedure
In the inspector I manually sort each room into separate lists based on the number of exits they each have.
Here are the steps performed each time a new level is generated:
1. Place random points within a certain radius. The number of points determines how many rooms the level will have.
2. Generate a Delaunay triangulation from the points.
3. Use the edges of the triangle to generate a minimum spanning tree.
4. Randomly add in edges to create loops between rooms. For simplicity, the number of edges connected to a single node shouldn't exceed 4.
5. For each node of the MST, determine how many edges are connected to it. This is done so we can find rooms from our pool that have a matching number of exits.
6. Randomly choose and generate a room for each node of the MST. When a room is generated, a bounding box is also created so that subsequent rooms can avoid overlapping with existing ones. If a room would overlap, add a random offset and repeat until the room can be placed.
8. For each exit of each room, use A* pathfinding to find the shortest path to a connected room. Pipes are drawn at each point of the path using rule tiles.