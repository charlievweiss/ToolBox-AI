# ToolBox-AI
Al and Algorithms Project Toolbox starter code

Full instructions at https://sites.google.com/site/sd16spring/home/project-toolbox/home-project-toolbox-algorithms-and-ai

## Comments from Charlie on the screenshots
### fcost, gcost, and hcost
Gcost shows the total cost to get to that tile from the starting position. Hcost shows the distance (ignoring obstacles) to get to the goal from a tile (you'll notice that tiles on a northeast diagonal have the same hcost as the other elements on the diagonal). Fcost is the sum of those two numbers for each tile.

### diagonal
The path is forced to make a diagonal movement because there is literally no other way of getting to the goal. Otherwise, it remains efficient by making only vertical or horizontal moves.

### hops
The path takes the only route that allows less than three jumps to get to the goal.

### swamp
The path opts for the route that crosses the swamp twice, though there is a path available to only cross it once. This is because a cleverly placed lava block increases the cost of hopping the lava or going around it above the cost of crossing an extra swamp.
