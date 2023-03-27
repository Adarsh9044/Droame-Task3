# Droame-Task3
Here is implementation:


One possible algorithm to solve this problem is as follows:

Sort the list of drones based on their starting time in ascending order.

For each drone in the list, find the shortest path from its starting position to its destination using a pathfinding algorithm such as A*.

Before moving the drone along its path, check if there are any collisions with other drones. If there are, adjust the path by selecting an alternative path or waiting for the other drone to pass.

Move the drone along its path at a speed of one unit per second until it reaches its destination.

Repeat steps 2-4 for all drones in the list.

Some additional assumptions and details:

To check for collisions, we can keep track of the positions of all drones at each time step and compare them to the positions of other drones.
If a collision is detected, we can either wait for the other drone to pass before continuing along the original path, or we can calculate a new path that avoids the collision.
We can assume that the drones move instantaneously from one position to the next, without any acceleration or deceleration time.
To optimize for minimum time, we can use a heuristic function in the pathfinding algorithm that estimates the remaining distance to the destination, as well as the time required to reach it. This will prioritize paths that are both short and fast.
