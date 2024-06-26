# ChessMS

By Ruihang Liu, Alex Miller, Jared Pincus

More detail of the project is on [DevPost](https://devpost.com/software/chessms-8ta6j9).

Winner of "Best Use of CockroachDB" at [BostonHacks 2022](https://bostonhacks-2022.devpost.com/)

# Project

SMS-based game AI

Uses Twilio to communicate between player and AI.

Uses CockroachDB to store persistent game state for all players.

# Dependencies

Python: `stockfish`, `parse`, `chess`, `flask`, `twilio`, `psycopg` [binary]


# Immediate goals

Read FEN-format user move input

Get it running locally

`help` text gives possible user commands

Choose at start of game to be white or black

User commands:
 - `start`: begin a game. If a game is currently running, confirm whether to end current game
 - `forfeit`: user ends current game.

## Starting a game

 - Ask if user wants to be `white`, `black`, or `random`
 - Ask for difficulty. Either `easy`/`medium`/`hard`, or accept specific ELO

# Optional goals

Display possible moves to user

More natural-ish language user commands

Prettier unicode/ascii boards
 - chess piece unicode symbols
 - display ranks/files
 - box around board

Get it running server-side

Change visuals based on if user is white or black

User chooses certain game settings
 - ELO rating

Deliberately add a delay to text response

Track lifetime wins/losses/draws

User can ask for W/L/D any time

Promotion
