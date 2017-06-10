# Greedy-Panicky--Grab-Those-Patty
An AI project for Minecraft[1.8] game. The agent is trained to collect apples, escaping from pursuing enemies, and avoiding lava blocks all at the same time. Based on A-Star algorithm and Malmo framework. [Project Video][video ref]

     
<a href="https://github.com/Leoll1020/Greedy-Panicky--Grab-Those-Patty">Link to Source Code</a>

## Background
Mr.Panicky loves eating apple but he is afraid of bugs. One day, he stole some apples from his boss, Mr.Mean, and unfortunately, got caught. Mr.Mean then put him into a cube full of maneating endermite as a punishment. Luckily, he found he is not only surrounded by endermites, but also his favorite apples! Now starts Mr.Panicky's journey of surviving from endermites while collecting as many apples he can without falling into lava!

## Objective
Designed and implemented an AI agent whose objective is collecting positive rewards (apples) while doging negative rewards (endermites and lava).

## Approach
Applied A-Star searching algorithm to collect positive rewards (apples) and dodge negative rewards (lava) based on current position and expected costs (steps) to goals; Utilized dynamic angle-distance algorithm (provided in mob_fun.py by Malmo) to pursue positive rewards (also apples) and dodge negative rewards (endermites); Then balanced two policies' output by a voting function. This voting function is based on relative distance of different dangers and a hill climbing factor alpha. Alpha is updated frequently and reflects agent's impression of danger weight based on all previous experience.

## Game Screenshot
Game board layout (green: agent, blue: apples, red: endermites):
<br />
<img src="docs/game_board.png" height="360" width="360" alt=""> <br />

Actual game UI:
<br />
<img src="docs/game_layout.png" height="480" width="720" alt=""> <br />


## Links
Video: https://m.youtube.com/watch?feature=youtu.be&v=h-qSJNtnlz0

Github Repo: https://leoll1020.github.io/Greedy-Panicky--Grab-Those-Patty/

Website: https://leoll1020.github.io/Greedy-Panicky--Grab-Those-Patty/index.html


Credits to Yiqiao Zhao, Chen Lu, Xiyue Zhang

[video ref]: https://www.youtube.com/watch?v=h-qSJNtnlz0
