# Tic-Tac-Toe-Game

## Basic 3x3
A 3x3 tic-tac-toe game with a basic interface, including a button to switch between **dark mode** and **light mode**

The **simplest method** to check for a win is to use a variable `winningPossibilities` in the `js` file to store all **winning positions** and sequentially check if there are three cells in a row (or column, or diagonal) with the same character

Since this is a 3x3 grid, the checking process doesn’t take much time

**Note**: The HTML, CSS, and JS code for **Basic 3x3**, as well as all subsequent variations, were originally inspired by Jothin Kumar’s repository ([tic-tac-toe](https://github.com/Jothin-kumar/tic-tac-toe)). I then developed and modified them according to my own preferences

## Grid 15x15 + Some Optimization
Increasing the game board size from 3x3 to 15x15 (or more if desired)

Using a function `addButtons()` to add 15x15 button elements to the `html` file instead of doing it manually like the 3x3 board

Since this is a 15x15 board, **change** the win condition from 3 consecutive characters in a row (or column, or diagonal) to 5 characters and **optimize** the win-checking method `checkWin()` by checking the row, column, and diagonal containing the newly added character each time a character is added. If 5 consecutive characters are found, **immediately** return a win result

Adding a `next round` button and `score board` to allow **playing multiple consecutive rounds**

**Known issue:** The interface may still be misaligned or not look good depending on the computer or phone screen

## Hexagonal Grids + Some Effects
Changing the shape of the cells from squares to **hexagons** to create a more visually appealing look

Adjusting the win-checking method `checkWin()` slightly to accommodate the new positions of the hexagonal cells

Adding **sound effects** for each cell click and an effect to **highlight** the hexagon cell when the mouse hovers over it

In the `css` file, change from `px` to `vw` to make the interface look better **regardless** of the screen size of the computer being used

## 3D Tictactoe
3D version of tic-tac-toe game, also known by the trade name Qubic 

Adding **z-coordinate** in the `XOSquare` class

The **win condition** is adjusted to 3 characters in a row or diagonal line **through** the 3 boards, the `checkWin()` function is **optimized** 

Modifying the `next round` button so it cannot be continued unless the current game is **finished**

**Note:** you can increase the size to 4x4x4 or larger if you like (the functions in the `js` file can be **applied** to larger boards), I keep it 3x3x3 simply because it fits neatly on my computer screen and is easy to see
