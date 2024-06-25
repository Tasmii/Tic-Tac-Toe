# Tic Tac Toe Game

This is a simple Tic Tac Toe game built with React. The game allows two players to play Tic Tac Toe in a browser. It includes features like sound effects, game over detection, and a reset button.

## Features

- Two-player functionality (Player X and Player O)
- Sound effects for moves and game over events
- Detection of winning combinations and draw situations
- Visual strike-through on the winning combination
- Reset button to start a new game

## Installation

1. **Clone the repository:**

    ```sh
    git clone https://github.com/your-username/tic-tac-toe.git
    ```

2. **Navigate to the project directory:**

    ```sh
    cd tic-tac-toe
    ```

3. **Install dependencies:**

    ```sh
    npm install
    ```

## Usage

1. **Start the development server:**

    ```sh
    npm start
    ```

2. **Open the game in your browser:**

    Navigate to `http://localhost:3000` in your web browser to play the game.

## Project Structure

- `src/`: Contains all the source files
  - `components/`: Contains React components
    - `Board.jsx`: Manages the board state and renders the board
    - `Tile.jsx`: Represents a single tile in the Tic Tac Toe grid
    - `Strike.jsx`: Renders a strike-through line on the winning combination
    - `GameOver.jsx`: Displays the game over message
    - `Reset.jsx`: Provides a reset button to start a new game
    - `TicTacToe.jsx`: The main component that ties everything together
    - `GameState.js`: Defines the various game states
  - `sounds/`: Contains sound assets for the game

## Game Logic

- **Winning Combinations:**
  The game checks for the following winning combinations:
  - Rows: [0, 1, 2], [3, 4, 5], [6, 7, 8]
  - Columns: [0, 3, 6], [1, 4, 7], [2, 5, 8]
  - Diagonals: [0, 4, 8], [2, 4, 6]

- **Game States:**
  - `playerXWins`: Player X wins
  - `playerOWins`: Player O wins
  - `draw`: The game ends in a draw
  - `inProgress`: The game is ongoing

## Sounds

- **Click Sound:** Plays when a tile is clicked
- **Game Over Sound:** Plays when the game ends (either win or draw)

## Customization

- You can customize the sound effects by replacing the files in the `sounds` directory.
- Adjust the volume of the sound effects in `TicTacToe.jsx` by modifying the `volume` property.

## Contributing

Feel free to open issues or submit pull requests for any improvements or bug fixes.

## License

This project is licensed under the MIT License.
