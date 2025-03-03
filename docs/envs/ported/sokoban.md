# Sokoban

This family of environments is ported to MiniHack from [NetHack](https://github.com/heiner/nle), levels taken directly from Sokoban minigame inside NetHack, excluding monsters and items. The goal is to push boulder's to goal locations (pits or holes).

Original dat file can be seen [here](https://github.com/heiner/nle/blob/main/dat/sokoban.des).
and corresponding solution from [NetHack Wiki](https://nethackwiki.com/wiki/Sokoban).

An example of Sokoban level ported into MiniHack.

![](../imgs/sokoban3b.png)

## Available Actions
- Movement in 8 directions
- OPEN
- EAT
- PICKUP


## Reward

The agent receives a reward of +1 for reaching the stairs down and +0.1 for filling each pit. Additionally, a small time penalty of -0.001 is applied at each step to encourage efficient solutions.

## Game Mechanics
- The agent must navigate through the level, pushing boulders to fill pits
- Stepping into a pit results in death and the end of the episode
- Episodes are limited to 2000 steps by default
- The game is considered successfully completed when all pits are filled and the agent reaches the stairs


## All Environments

| Name                    | Capability |
| ----------------------- | ---------- |
| `MiniHack-Sokoban1a-v1` | Planning   |
| `MiniHack-Sokoban1b-v1` | Planning   |
| `MiniHack-Sokoban2a-v1` | Planning   |
| `MiniHack-Sokoban2b-v1` | Planning   |
| `MiniHack-Sokoban3a-v1` | Planning   |
| `MiniHack-Sokoban3b-v1` | Planning   |
| `MiniHack-Sokoban4a-v1` | Planning   |
| `MiniHack-Sokoban4b-v1` | Planning   |
