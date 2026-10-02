# Pong Game

A two-player Pong game in Python using the built-in `turtle` graphics module.

## How to play
Run `python main.py`. The left player moves their paddle with **W** and **S**, the right player with the **Up** and **Down** arrow keys. Bounce the ball past your opponent's paddle to score. Click the window to exit.

## How it works
- `main.py`: sets up the 800 by 600 black screen, creates two paddles, the ball and the scoreboard, binds the keys, and runs the game loop (move the ball, bounce off the top and bottom walls, bounce off a paddle when the ball is within 50 units of it near the edge, award a point when the ball passes x = 380 or x = -380).
- `ball.py`: a `Turtle` subclass that moves 10 units per step in x and y, flips direction on a bounce, speeds up by 10% on every paddle hit (the sleep delay is multiplied by 0.9), and resets to the centre with reversed direction after a point.
- `paddle.py`: a tall `Turtle` square that moves 20 units up or down per key press.
- `scoreboard.py`: draws both scores and updates them after each point.

## Skills practised
Object-oriented design (classes and inheritance from `Turtle`), event-driven input, a game loop with collision detection, and splitting code across modules.

## Requirements
Python 3 with Tk support (standard on most installs); no extra packages.
