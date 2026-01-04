War Card Game.

simple OOP-based card game in python.

🔹 The Suit Class
 	The instances of this class shall have two instance attributes: description and symbol.

 	description can be either: "clubs", "diamonds", "hearts", or "spades".

 	symbol can be either: ♣, ♦, ♥, or ♠.

 	The instance attributes shall be read-only attributes (they should only have getters).

 	The class shall have a class attribute that maps suit descriptions to their corresponding symbols (this should be 	a dictionary).



🔸 The Card Class
 	The instances of this class shall have two instance attributes: suit and value.

 	suit must be an instance of the Suit class.

 	The instance attributes shall be read-only attributes (they should only have getters).

 	The class shall have a class attribute that maps the values of the special cards to their written descriptions (11 	to "Jack", 12 to        "Queen", 13 to "King", and 14 to "Ace"). This should be a dictionary.

 	The class shall have two methods: show and is_special.

 	The show method shall display the value, suit, and symbol of the suit of the card. If the card is special, this 	should be the written description (e.g. "Jack") instead of the value.

 	The is_special method shall return True if the value of the card is greater than or equal to 11 and False 	otherwise.



🔹 The Deck Class
 	The instances of this class shall have one instance attribute: cards. This attribute shall be non-public and it 	shall contain a list of instances of the Card class (these are the cards that belong to the deck).

 	The deck shall have a property called size, which corresponds to the length of the list of cards in the deck.

 	The user of the Deck class shall be able to choose if the deck is initially empty or not when the deck instance is 	created.

 	The class shall have four methods: build, show, shuffle, draw, and add.

 	The build method shall build the deck by creating 52 card instances with numbers from 2 to 14 (inclusive) for each 	one of the four possible suits.
 
 	The show method shall iterate over the list of card instances and call their show method to show the description 	of each card.

 	The shuffle method shall shuffle the deck (the list of cards in the deck) by calling the shuffle function from the 	random module. (please refer to the section on import statements if you are unfamiliar with import statements).

 	The draw method shall return and remove the last card in the list of cards in the deck (this represents removing 	it from the top of the deck).

 	The add method shall insert a new card object to the beginning of the list of cards in the deck (this represents 	removing it from the bottom of the deck).



🔸 The Player Class
 	The instances of this class shall have three instance attributes: name, deck, and is_computer.

 	name shall be a string.

 	deck shall be an instance of the Deck class.

 	is_computer shall be either True or False.

 	name shall be a public attribute and deck and is_computer shall be non-public read-only attributes.

 	The class shall have four methods: has_empty_deck, draw_card, and add_card.

 	The has_empty_deck method shall return True if the size of the player's deck is 0. Else, it shall return False.

 	The draw_card method shall draw a card from the player's deck if the deck is not empty and return it.

 	The add_card method shall add a card to the bottom of the player's deck.
