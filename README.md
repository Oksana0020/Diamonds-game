# Diamonds Game

A turn-based strategy game inspired by Robinson Crusoe and Friday, played with two piles of stones on a desert island.

The game was developed step by step, starting with simple rules and later adding special events.

Diamonds Game is a Python strategy game where human player competes against an AI using the **Minimax algorithm**.

## Rules

The game starts with two piles of stones.

Players take turns making one move:

- Remove **1–10** stones from pile A
- Remove **1–10** stones from pile B
- Remove **1–5** stones from both piles equally

Player who reaches **(0,0)** wins the game.

## AI Opponent

AI uses:

- Minimax search
- Depth-limited search
- Heuristic board evaluation

Evaluation function considers:

- Total stones remaining
- Pile balance
- Closeness to multiples of 11
- Lucky 13 danger
- Whose turn it is at cutoff depth

## Special Feature: Lucky 13

If any pile becomes **13** then **5 stones are added to both piles**.

This adds randomness and strategy changes.

## Features

- Human vs AI gameplay
- Character selection (Robinson / Friday)
- Move validation
- Visual pile bars
- Character dialogue
- Configurable AI depth

## Run Game

```python
play_game_basic(110, 55, max_depth=4)
