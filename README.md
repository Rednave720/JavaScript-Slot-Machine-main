# JavaScript-Slot-Machine

# 💻  Software Development

Slot Machine Game

This project implements a simple slot machine game in JavaScript. The game lets users deposit money, choose how many lines to bet on, spin the reels, and calculate winnings based on the spin outcome. Gameplay continues until the user runs out of funds or opts to stop playing.

Description of a Play Session:
	1.	Starting Out:
A player begins by entering a deposit amount to fund their game. Next, they choose how many lines (between 1 and 3) they want to bet on and decide on the bet per line based on their available balance.
	2.	Spinning the Reels:
Once the bets are placed, the player spins the slot machine. The game randomly selects symbols for each reel, ensuring that each symbol appears according to its predetermined frequency. These symbols are then rearranged into rows for evaluation.
	3.	Evaluating the Outcome:
The game displays the rows of symbols on screen. It then checks each bet line to see if all symbols match. If they do, the game calculates the winnings based on the bet amount and the value assigned to the matching symbol.
	4.	Updating the Balance and Continuing:
The player’s balance is updated—winning money is added, or the bet is deducted if there’s no match. The game then prompts the player to continue playing or to cash out if they’re satisfied. This cycle repeats until the player runs out of funds or decides to quit.

In essence, each play session is a loop of depositing funds, placing bets, spinning the reels, evaluating the result, and updating the player’s balance.

⸻

Features
	•	User Deposit & Bet Setup:
	•	Prompts the user to deposit a positive amount.
	•	Allows the user to select 1 to 3 bet lines and calculates the maximum allowable bet.
	•	Randomized Spin Mechanics:
	•	Uses predefined symbol counts to simulate reel spins with controlled probabilities.
	•	Ensures no symbol repeats on a single reel.
	•	Reel Transposition:
	•	Rearranges the reels into rows for easier evaluation of winning combinations.
	•	Winning Calculation:
	•	Checks if symbols in a row match and computes winnings based on bet amount and symbol values.
	•	Game Flow Management:
	•	A main loop guides the game through deposits, bets, spins, and balance updates until the game ends.

⸻

How It Works
	1.	Deposit Function:
Prompts the user to enter a deposit, validating that the input is a positive number.
	2.	Bet Setup:
	•	getNumberOfLines: Asks the user to choose how many lines to bet on (1–3).
	•	getBet: Ensures the bet is within the user’s balance and calculates per-line limits.
	3.	Spin Mechanics:
	•	spin: Simulates spinning by randomly selecting symbols from a pool based on SYMBOLS_COUNT.
	•	transpose: Converts reel data into rows for easier evaluation.
	4.	Display & Evaluation:
	•	printRows: Shows the results in a clear, formatted layout.
	•	getWinnings: Determines winnings if all symbols in a row (up to the number of bet lines) match.
	5.	Game Loop:
Orchestrated by the game function, it manages deposits, bets, spins, and updates the user’s balance until the game ends.

⸻

Installation and Running the Game
	1.	Clone the Repository:

git clone <repository-url>
cd slot-machine-game


	2.	Open the Game:
	•	Open index.html directly in your browser, or
	•	Run a local static server (e.g., using npx serve .) and navigate to the provided URL.

⸻

Code Structure
	•	Functions:
Each core functionality is modularized into functions (e.g., deposit, spin, transpose, etc.), ensuring clear separation of concerns.
	•	Objects:
	•	Uses objects for symbol counts (SYMBOLS_COUNT) and symbol values (SYMBOL_VALUES), making the game rules easily configurable.
	•	Control Flow:
	•	Implements loops and conditionals to validate user input and manage game progression effectively.

⸻

Future Improvements
	•	Enhanced Error Handling:
Improve input validation and add error management for unexpected cases.
	•	Code Refactoring:
Reduce repeated logic for better readability and maintainability.
	•	UI Enhancements:
Optionally develop a graphical user interface for a more immersive experience.
	•	Additional Features:
Explore more complex betting options and payout strategies to extend gameplay.

⸻

Conclusion

This slot machine game demonstrates essential JavaScript concepts—using objects, functions, and control structures—to create a fun and interactive user experience. It serves as a solid foundation that can be expanded with more features and refined with better error handling. Enjoy the game, and feel free to customize the code to add your personal touch!

⸻

Feel free to update this README as your project evolves. Happy coding!
