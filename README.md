### ViZDoom (Speedrunning) RL Maps

This repository holds different maps used for a project, teaching RL agents to speedrun in ViZDoom. This makes up 4 maps:

* Basic Scenario
* Maze
* Maze Difficult
* Deadly Corridor

Deadly Corridor is an existing ViZDoom scenario, but was modified for the project. 

### Details

Each map has a green or red vest that appears at the end, with the main goal of reaching it as fast as possible, as a negative living reward is applied. The reward system is designed for each scenario such that it encourages the agent to explore better and reach the end goal safely. Specific reward details are mentioned for each map.

Every scenario would have this basic reward system:

* Living Reward : $-0.001$
* Goal Reward: $+100$

Below is a description of each map.

### Scenarios

#### Basic Scenario

U-shaped map where the agent must navigate down a corridor with a bend to reach the armour vest.

#### Maze

As the name implies, a simple labyrinth with the same goal of the agent reaching the vest at the end of the maze.

#### Maze Difficult

The same map as Maze, however with added enemies and obstacles, different reward values given depending on the enemy killed. Another quicker path to the goal is added, but an added room separated by 2 doors and a Chaingunner inside.

#### Deadly Corridor

The same Deadly Corridor scenario used by ViZDoom, except the agent is not reward for getting closer to the goal, but reaching it instead like all other scenarios. Doors separating each corridor so the agent can't just sprint to the end in lower difficulties.
