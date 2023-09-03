# War Card Game Simulator

## Overview

This Python project simulates the classic card game "War." In this two-player game, you'll face off against a computer opponent, taking turns drawing cards and engaging in "wars" when there are ties. The goal is to win all the cards by the end of the game. This project is designed to demonstrate the use of classes and object-oriented programming in Python.

## How to Play

1. **Starting the Game**: When you run the program, you'll be prompted to enter the number of cards to be drawn at the time of a "war." This number can be customized to make the game more challenging.

2. **Deck Creation**: A standard deck of 52 cards is created, shuffled, and evenly distributed between you (Player One) and the computer (Player Two).

3. **Game Rounds**: The game proceeds in rounds. Each round consists of the following steps:

   - Both players draw one card from their decks.
   - The cards drawn are compared based on their values.
   - The player with the higher-ranked card wins both cards and adds them to the bottom of their deck.
   - If there's a tie (both players draw cards of the same rank), a "war" occurs.

4. **War**: In case of a tie, a "war" is initiated. The following steps occur during a war:

   - A specified number of cards (as determined at the beginning of the game) are drawn face-down for each player.
   - One card is drawn face-up for each player.
   - The player with the higher-ranked face-up card wins all the cards in the war and adds them to the bottom of their deck.

5. **Winning the Game**: The game continues until one player has all the cards or until one player has an insufficient number of cards to initiate a war. In either of these cases, the player with all the cards or the most cards wins the game.

6. **Game Over**: The game concludes, and the winner (Player One or Player Two) is announced.

## Customization

You can customize the game by modifying the following variables in the code:

- `choose`: The number of cards to be drawn at the time of a "war" (default is set via user input).
- `suits`: The four suits used in the deck.
- `rank`: The ranks (values) of the cards in the deck.
- `card_values`: The values associated with each rank for determining card comparisons.
- `MAX_ROUNDS`: The maximum number of rounds to play before ending the game.

## Classes

### `Card`

- Represents an individual playing card with attributes for suit, rank, and value.
- Allows for easy card creation, display, and comparison.

### `Deck`

- Represents a deck of cards.
- Creates a shuffled deck and provides methods for shuffling and dealing cards.

### `Player`

- Represents a player in the game.
- Contains methods for removing, adding, and displaying cards for each player.

## Getting Started

1. Clone this repository to your local machine.

   ```bash
   git clone https://github.com/vijay-vardhan-reddy/war-card-game.git
   ```

2. Navigate to the project directory.

   ```bash
   cd war
   ```

3. Run the game.

   ```bash
   python war.py
   ```

## Contributors

-[Vijay Vardhan Reddy](https://github.com/vijay-vardhan-reddy): Project creator and maintainer.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

Enjoy playing the War Card Game! If you have any feedback, questions, or encounter issues, please feel free to [create an issue](https://github.com/your-username/war-card-game/issues) on the GitHub repository. Have fun!
