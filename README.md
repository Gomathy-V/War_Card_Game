# War_Card_Game

### Project Overview
- Develop a text-based version of the classic card game "War" using Python. The game aims to simulate the competition between two players as they draw and compare cards from their respective decks.

### Tools and Technologies
- **Programming Language:** Python
- **IDE/Code Editor:** Jupyter Notebook
- **Libraries:**
  - `random` for shuffling the deck.

### Features
- **Deck Initialization:** The deck is created using list comprehensions and the `ranks` and `suits` lists.
- **Shuffling:** Random shuffling of the deck to ensure fair gameplay.
- **Dealing Cards:** The deck is split into two halves, one for each player.
- **Game Play:** The function handles the core game logic, including the war scenario.
- **User Interface:** Displays the current round number and shows "WAR" if a tie occurs during that round.
- **Game End:** The game loop continues until one player runs out of cards.

### Explanation
**1. Deck Initialization:**
   - A standard deck of 52 cards is created, comprising four suits (hearts, diamonds, clubs, spades) and 13 ranks (2 through 10, Jack, Queen, King, Ace).

**2. Card Shuffling:**
   - The deck is shuffled to ensure random distribution of cards to the players.

**3. Player Setup:**
   - Two players (Player 1 and Player 2) are created, each receiving 26 cards dealt from the shuffled deck.

**4. Game Play:**
   - Players draw the top card from their respective decks and compare them.
   - The player with the higher-ranked card wins the round and takes both cards, placing them at the bottom of their deck.
   - In case of a tie (War), a tie-breaking mechanism is triggered:
      - Each player draws five face-down cards and one face-up card.
      - The face-up cards are compared to determine the winner of all the cards involved in that round.
      - If the face-up cards are also tied, the process repeats until a winner is determined or a player cannot continue the war due to insufficient cards.

**5. User Interface:**
   - At the beginning of each round, the interface will display the current round number.
   - During a round, if a tie happens between the cards played by both players, the interface will display "WAR" to signify the occurrence of a special tie-breaking sequence.
     
**6. Game End:**
   - The game continues until one player runs out of cards.
   - The player with all the cards is declared the winner.

