War Card Game (OOP)
A simple, robust implementation of the classic "War" card game using Object-Oriented Programming principles in Python.

🛠 Project Structure
The project is built using four main classes to handle the game logic and card mechanics.

🔹 The Suit Class
Handles the identity of card suits.

Attributes: description ("clubs", "diamonds", "hearts", "spades") and symbol (♣, ♦, ♥, ♠).

Encapsulation: Read-only attributes using getters.

Class Mapping: Features a class-level dictionary that maps descriptions to their corresponding symbols.

🔸 The Card Class
Represents a single playing card.

Attributes: suit (an instance of the Suit class) and value.

Encapsulation: Read-only attributes using getters.

Special Cards: Uses a class attribute dictionary to map values:

11: Jack

12: Queen

13: King

14: Ace

Methods:

show(): Displays the card's value, suit, and symbol. (e.g., "Jack of Hearts ♥").

is_special(): Returns True if the card value is 11 or higher.

🔹 The Deck Class
Manages a collection of 52 cards.

Attributes: A non-public list _cards.

Properties: size (returns the length of the card list).

Flexibility: Can be initialized as empty or full.

Methods:

build(): Populates the deck with 52 cards (values 2-14 for each suit).

show(): Prints the description of every card in the deck.

shuffle(): Randomizes the card order using the random module.

draw(): Removes and returns the top card (last in list).

add(card): Inserts a card to the bottom (start of list).

🔸 The Player Class
Represents the participants (Human or Computer).

Attributes: name (public), _deck (read-only), and _is_computer (read-only).

Methods:

has_empty_deck(): Returns True if the player has no cards left.

draw_card(): Draws a card from the player's personal deck.

add_card(card): Adds a card to the bottom of the player's deck.
