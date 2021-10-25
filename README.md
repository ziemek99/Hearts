# Hearts

A Python implementation of Hearts. This project is a work in progress.

# Objective
Win all the hearts and the queen of spades, or none of these cards. Get as few points as possbile.

# Rules
* Each of the four players is dealt 13 cards.

* Before the round starts, all four players pass three cards left, right, across, or no pass: the game cycles through these four instances with the passing of rounds.

* The player with the two of clubs leads the first trick.

* A player must play a card with the suit of the card that leads the trick if they have one, otherwise any card may be played.

* The player with the high ranked card of the suit that lead wins the trick (aces are high).

* A player may not play hearts or the queen of spades on the first hand (except if they don't have any other option).

* After all 13 tricks have been played, points are tallied for each player.

* A player receives one point per heart and 13 points for the queen of spades.

* If a player has all of the points, they have "shot the moon", get 0 points and all other players get 26 points.

* The game ends when the first player gets to 100. The winner is the player with the fewest points.

# Implementation
The game can be played manually or simulated by the computer. This mode can be toggled at the top of the `Hearts.py` file by changing the variable `auto` between `True` and `False`. The computer will play until one player's score reaches 100 and then the game ends with the final score display. The computer uses a "guess and check" method to play the game. It will attempt to play a card from the current player's hand at random. If the play is valid, the game moves on to the next player. If the play is invalid, the computer is forced to try again, until it makes a valid play. Passing is disabled for the computer simulation.
