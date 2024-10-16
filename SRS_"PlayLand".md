# Software Requirements Specification
## For "PlayLand"

Version 0.1
Prepared by Lavrinenko Alina, Boiko Polina
# Table of Contents 
* [Revision History](#Revision-History)
* 1 [Introduction](#1-Introduction)
  * 1.1 [Document Purpose](#11-Document-Purpose)
  * 1.2 [Product Scope](#12-Product-Scope)
  * 1.3 [References](#13-References)
  * 1.4 [Document Overview](#14-Document-Overview)
* 2 [Product Overview](#2-Product-Overview)
  * 2.1 [Product Perspective](#21-Product-Perspective)
  * 2.2 [Product Functions](#22-Product-Functions)
  * 2.3 [Product Constraints](#23-Product-Constraints)
  * 2.4 [User Characteristics](#24-User-Charecteristics)
  * 2.5 [Apportioning of Requirements](#25-Apportioning-of-Requirements)
* 3 [Requirements](#3-Requirements)
## Revision History
|   Name   |   Date   | Reason For Changes  |  Version  |
| -------- | -------- | ------------------- | --------- |
| PlayLand | 16.10.24 |                     | Version 1 |
|          |          |                     |           |
|          |          |                     |           |
## 1. Introduction
### 1.1 Document Purpose
The purpose of the SRS is to store all project requirements and other important information. SRS's intended audience is our team.
### 1.2 Product Scope
This game is a collection of different mini-games. Players can choose which game they want to play. The purpose of this game is to be useful while we have a power outage.
### 1.3 References
We used the game “Games Without Internet - Offline” as a reference.
### 1.4 Document Overview
The remaine of the document contains a product overview, requirements, functional and technical specifications.
## 2 Product Overview
### 2.1 Product Perspective
It's a new, self-contained product.
### 2.2 Product Functions
The game must allow the user to:
1. Select a game 
2. Create an account
3. Choose a game mode (easy, medium, hard) where possible.
4. To turn off the music
5. To get some awards
### 2.3 Product Constraints
This game will be made for mobile phones. In this game we'll use cel-shading graphics. 
### 2.4 User Characteristics
Main client of this game is Ukrainian, because it'll be in Ukrainian language and this games will be offline, so Ukrainians can use it during power outage.
### 2.5 Apportioning of Requirements
Requirements that may be delayed until future versions of the system:
1. 10 mini-games (we can make less to start with)
2. Awards (we can gradually add more and more awards)
3. Game currency
## 3 Requirements
Requirements:
1. The game will contain 10 mini-games (ranging from simple games for relaxation to educational games to connect thinking);
2. The game will have its own game currency (for which the player will be able to buy various bonuses, tips or bonus levels);
3. On the main screen, you will be able to select the desired mini-game (while completing one scenario, you can easily move to another through the main screen);
4. The game should automatically save the player's progress in each game (in each mini-game there will be a tab ‘Achievements / results’ where the player can see the success in this game);
5. For achievements, the player receives rewards (bonuses, coins or additional stories, for which the player will also receive some coins that can be spent in other mini-games to improve life (without starting the round again) or even hints;
6. Sound effects and music (while playing the game, you may hear melodies or some sound moments in the games. You can switch off the sound in the settings);
7. The game should be able to add new mini-games without significant changes in the architecture (this will be done by the author of the game, when updating);
8. The game should contain difficulty types for games where possible (you will have the option to choose between ‘easy’, ‘medium’ and ‘hard’ level (progressive growth to attract new players, with the possibility of customising the difficulty level));
9.Graphics style: cel-shading (a picture with clear contours, all possible colours);
10.Menu (understandable for all players, which will contain everything you need to complete all the games. You will see three buttons: ‘games’, ‘settings’, ‘help’ (explanations for any game)).
## 4 Game
### 2048
1. The goal of the game is to create a tile with the number 2048. the player can continue the game after reaching this goal to get higher results.
2. Playing field: the standard is a 4x4 square field, but the player can choose the desired size.
3. End of the game: the game ends when no move can be made, i.e. when all the cells are filled and no tile can connect to another.
4. Rewards: the main task of many players is to beat their previous record or achieve the highest possible result, for which they can receive a reward in the form of coins that can be spent both in this game and in subsequent games.
5. Control: The player must be able to control the tiles by moving them in one of four directions: up, down, left, right.
6.If two tiles with the same value collide in the same direction, they must be combined into one tile whose value is equal to the sum of these two tiles.
7.After each successful move, a new tile with a value of 2 or 4 should appear on the field.
### Tic Tac Toe 
1. The game board: the game is played on a 3x3 grid consisting of 9 cells;
2. Players: the player plays against the computer (one player uses crosses (X), the other uses zeros (O));
3. The goal of the game: the player must fill in three cells with his symbol vertically, horizontally or diagonally;
4. Winning: if one of the players fills three cells in a row (along any line), he wins;
5. Rewards: the game is simple, the main goal and “reward” is the pleasure of winning and improving your own strategy.
6. Rules of the game: The first move is made by the player who plays for the crosses (X). After each turn, the game should automatically switch to the other player.
7. Tie: The game should end in a tie if all the cells of the board are filled and neither player has fulfilled the victory condition. In the event of a tie, a notification should appear and the game should be restarted.
8. Correctness of moves: Players can only place crosses or zeros in empty cells. If a player tries to move to an already occupied square, the game should reject the move and offer to choose another square.
9. AI: The AI should follow standard game strategies and choose free cells depending on the difficulty level:
Easy level - random choice of a move.
Medium level - basic logic, blocking the player's winning moves.
Advanced level - using advanced strategies to achieve victory or a draw.
### Snake
1. Playing field: the field consists of a grid or a simple plane without obstacles (or with them in more complex versions of the game);
2. Player: The player controls a snake that starts as a short chain of segments (usually 1-3 segments);
3. The goal of the game: the player has to control the snake to eat the “apples” that appear on the field.
4. Points: points are awarded for each apple eaten.
(The more apples are eaten, the longer the snake becomes and the more difficult it is to avoid collisions);
5. Snake acceleration: the speed of the snake's movement gradually increases, making the game more challenging;
6. Obstacles on the field: obstacles appear on the field, making it difficult for the snake to move;
7. End of game: the game ends if the snake crashes into a wall or its own body or the field runs out of space.
8. Control: The snake's head should move around the playing field, following the player's commands. The snake should move continuously, and the player can control the direction (up, down, left, right) with the keys or touch controls. The snake must not be able to move in the opposite direction (for example, if the snake moves to the right, the player cannot immediately turn to the left).
9. The player must be able to restart the game after a defeat through the “New Game” button. The game must include the ability to pause and resume at any time.
10. Food should appear in a random free cell that is not occupied by the snake's body.
11.The game can have several levels of difficulty:
Easy - slow speed of snake movement.
Medium - standard speed.
Difficult - high speed and more complicated rules (e.g. obstacles appearing on the field).
### Water sort 
1. The playing field: the field consists of several containers (bottles, tubes) filled with liquids of different colors;
2. The purpose of the game: the player must sort the liquids in such a way that each bottle has one color;
3. Difficulty: the number of colors and containers increases with the level, which makes sorting more difficult;
4. Hints: some versions of the game have a hint system that helps when the player cannot find a solution;
5. Rewards: the game has no rewards, the game structure itself motivates players to reach new levels and improve their logic skills
6. Control: The player should be able to choose one flask and then choose another flask to pour the liquid.
The player can only pour the liquid under the following conditions:
The color of the top layer of the selected flask matches the color of the top layer of the target flask.
There is free space in the target flask.
Only one layer of liquid can be transferred at a time (only the top layer is transferred).
7. If the conditions for pouring are not met (for example, the colors do not match or the flask is full), the game should prohibit the pouring and display a message about the impossibility of the action.
If a player has selected a flask by mistake, he or she should be able to deselect it and choose another flask.
8. Levels of difficulty:The game should include many levels of increasing difficulty:
Initial levels should have fewer flasks and colors.
In more difficult levels, the number of flasks and colors increases and the initial combination of layers becomes more difficult.
9. The game should end when the player successfully sorts all liquids into flasks so that each flask contains only one color. When a level is completed, the player should be shown a victory message and offered a move to the next level.
10. The game should track the player's progress so that the player can pick up where they left off.
It should be possible to start the level again at any time.
11. The game may include a coin system or rewards for completing levels that can be used for hints, extra moves, or other benefits.
### Sudoku 
1. Playing field: the field consists of a 9x9 grid divided into 9 3x3 blocks. At the beginning of the game, some cells on the field should be pre-filled with numbers from 1 to 9. These are the initial clues, which vary depending on the difficulty level. The remaining cells must be empty and ready to be filled by the player.
2. The player must fill in the empty cells with numbers from 1 to 9.
Each number can appear only once in each row, in each column and in each 3x3 block.
3. The game must support multiple levels of difficulty:
Easy - more pre-filled numbers, simplified combinations.
Medium - moderate number of filled numbers, medium difficulty.
Difficult - minimum number of filled numbers, maximum difficulty.
It is possible to add Expert mode with even more complex combinations and minimal hints.
4. The game should check if the selected number can be entered into this cell taking into account the rules (one number per row, column and 3x3 block). If the player enters the wrong number (without breaking the rules), the game should give the opportunity to change it.
5. Hints: The game should provide the ability to use hints to help the player. A hint can show the correct number for the selected cell. The number of hints should be limited at each level (e.g. 3 hints per game).
6.The player must be able to leave notes in empty cells to indicate possible variants of numbers. These notes may be deleted or changed by the player as the game progresses.
7. The game should keep track of the time taken to solve the puzzle.
The timer should start at the beginning of the level and stop when the grid is full or when the game is stopped (e.g., paused).
8. The player should be able to pause the game and return to it later without losing progress. When paused, time must stop.
9. The game should end with a win when the player has correctly filled all grid cells, following the Sudoku rules. Upon completion, the player should see a victory message with the option to advance to the next level or return to the main menu.
### Word Finder 
1. Playing field: The game consists of a rectangular grid filled with letters (for example, 4x4 or 5x5);
2. Game Objective: The player must find certain words that can be arranged horizontally, vertically or diagonally;
3. The essence of the game: There is a list of words to be found in the grid. This list can be available at the beginning of the game;
4. Time: A timer can be set to increase the difficulty;
5. Rewards: Players can get points for words found and the game can have a bonus system for long words or speed;
6. Points: Players get points for each word they find. Longer words can bring more points.
7. User Interface: Main menu with options: start game, settings, view leaderboard, exit.
An intuitive game screen with a grid of letters (from 4x4 to 6x6) in which users find words.
A timer to count down the time for each round of the game (if there is a time limit).
A button for a hint (optional) or the ability to skip a word.
8. Generating a random grid with letters for each round.
Mechanism for finding words by selecting a sequence of letters in the grid (horizontally, vertically, diagonally).
Checking the correctness of words using a dictionary (e.g., pre-built or available via API).
Awarding points for each word found (longer or more complex words may earn more points).
Determining the level of difficulty:
Beginner (short words and more time).
Medium (medium word length, medium time).
High (long or difficult words, limited time).
9. A limited number of hints for each level (shows the first or last letter of the word). Possibility to purchase additional hints.
### 15 Puzzle 
1. The playing field: The game consists of a 4x4 square grid containing 15 numbered tiles and one empty square;
2. Tiles: The numbered tiles must be from 1 to 15;
3. Objective of the game: The player must arrange the tiles in order from 1 to 15, filling the empty cell;
4. Movement: Tiles can only move to adjacent empty cells (up, down, left, right);
5. Trophies: Virtual rewards that can be displayed on the player's profile for completing special tasks
6. User Interface: Main menu with options: start game, view scoreboard, settings, exit.
Game screen with a 4x4 grid (15 tiles and 1 empty space).
Intuitive tile management that allows you to move tiles by clicking or swiping.
A move counter that shows the number of tile moves made by the player.
7. Generation of random starting positions for tiles in the grid with the ability to always get a solvable puzzle.
Mechanism of moving tiles: the player can move tiles to an empty space.
Determining the end of the game: when all the tiles are in the correct order, the game is over.
### Gallows 
1. Players: The game is usually played between two players - one chooses a word and the other tries to guess it (you will play with ii);
2. Attempts: The player has a limited number of attempts (usually 6 or 7) before completing the drawing, after which the game ends;
3. Objective: To guess the word or phrase by choosing letters before the limited number of attempts is exhausted;
4. Rewards:Players receive points for guessing words, with more points for quick guesses;
5. Levels: Progress through different difficulty levels with new words or themes;
6. Time: You can set time limits to increase the difficulty.
7. Game screen: A field for guessing the word that displays the number of letters in the word and the filled spaces after the guess.
An alphabet (letter buttons) from which the player chooses, or a text box for entering a letter.
Gallows visualization: an image that builds up gradually with each incorrect attempt.
Attempt counter: shows how many incorrect attempts are left before the game is over.
Progress bar: The number of correct guesses and errors.
8. Generating a random word from a predefined list (e.g., a game dictionary), according to the difficulty level.
Letter selection: The player can choose letters to guess the word.
Mechanism of guessing processing:
If the letter is in the word, it is displayed on the corresponding places.
If a letter is missing, the gallows is gradually drawn and the player loses one attempt.
Winning: when all letters of the word are guessed.
Loss: when the gallows is completely drawn and all attempts are exhausted.
9. Difficulty levels
Easy level: short or frequently used words, more attempts available.
Medium level: words of medium length and difficulty.
Hard level: long or rarely used words, fewer attempts.
10. Hint system: the player can get a hint about one of the letters of the word.
Hint counter: limited number of hints per game.
### Color Connect 
1. The playing field: The game usually consists of a grid (e.g., 8x8 or 10x10) filled with colored cells;
2. The purpose of the game: The player must connect pairs of the same color by drawing lines between them;
3. The essence of the game: There are pairs of the same color on the grid that need to be connected;
4. Time: In some versions of the game, a time limit may be set to complete a level;
5. Difficulty : The game may have multiple levels of increasing difficulty, with more colors and cells;
6. Restrictions : Lines cannot intersect, and the player can only connect identical colors;
7. Interface: Main menu with options: start game, difficulty levels, settings, exit. A game board with a grid of different sizes (e.g., 5x5, 6x6, 7x7) where players must connect dots of the same color.
8. Easy levels with smaller grids (e.g. 5x5) and fewer colors.
Medium levels (6x6 or 7x7) with more dots.
Hard levels with large grids (8x8 or more) and complex connection patterns.
Win: When all the dots are connected correctly and the entire grid is filled with lines.
Losing (optional): if the player fails to complete the level in a certain time or number of moves (in certain game modes).
9. Hints: the ability to get a hint about the correct connection of a certain pair of colored dots.
Limited number of hints: players can use hints only a few times per level or game.
“Cancel move” option: the ability to cancel the last line built.
### Checkers 
1. Playing field: Standard 8x8 board with 64 squares, alternating colors (usually dark and light);
2. Pieces: Each player has 12 pieces of the same color;
3. Location: The pieces are placed on the first three rows on the dark cells;
4. Objective of the game: Destroy all opponent's pieces or block them so they cannot make moves
5. End of the game: The game ends when one player loses all his pieces or cannot make any legal moves;
6.Main menu with options: start the game, select game mode, settings, leaderboard, help, exit.
7. Interactive checkers: the ability to select checkers and move them around the board.
8.Move indicator: displays whether it is the player's or the computer's/opponent's move.
9.Checker counter: displays the number of checkers of each player on the board.
10. Mechanics: A checker can jump over an opponent's checker diagonally, removing it from the board.
Possibility of combination capture: if after one jump the checker can make another jump, the player can continue the move.
Victory: when all the opponent's checkers are taken or he cannot make a single move.
Loss: when all the player's checkers are taken or it is impossible to make a move.
11.Difficulty levels: Easy level: the computer makes simple moves without complex tactical combinations.
Medium level: the computer uses tactical moves and capture combinations.
High level: the computer analyzes several moves ahead and uses advanced strategies.
