# Combat-Simulator

# Robot Gladiators: Lesson 1

In this first lesson, we'll use JavaScript to code a single round of Robot Gladiators. When we're done, the game will follow this sequence:

## Game Sequence

1. **Prompt for Robot Name**: The game will prompt the player to name their robot.

2. **Initialize Player's Robot**: The player's robot will be initialized with the following properties:
   - Health Points: 100
   - Attack Points: 10
   - Money Points: 10

3. **Initialize Opponent Robot**: The player's opponent, Roborto, will be initialized with the following properties:
   - Health Points: 50
   - Attack Points: 12

4. **Game Welcome Message**: The game will display "Welcome to Robot Gladiators!"

5. **Prompt for Action**: The game will prompt the player to either fight the round or skip it.

   - **If the Player Chooses to Skip**:
     - A penalty of 10 money points will be deducted from the player's robot.
     - The game will end.

   - **If the Player Chooses to Fight**:
     - The player's robot will attack Roborto, and the player-robot's attack points will be deducted from Roborto's health points.
     - The game will display Roborto's remaining health points.
     - Roborto will attack the player's robot, and Roborto's attack points will be deducted from the player's robot's health points.
     - The game will display the player-robot's remaining health points.
     - The game will end.

## JavaScript Code Implementation

Below is a sample JavaScript implementation of the game sequence described:

```javascript
// Prompt for the player's robot name
var playerName = prompt("What is your robot's name?");

// Player's robot properties
var playerHealth = 100;
var playerAttack = 10;
var playerMoney = 10;

// Opponent robot properties
var opponentName = "Roborto";
var opponentHealth = 50;
var opponentAttack = 12;

// Display the welcome message
console.log("Welcome to Robot Gladiators!");

// Prompt the player to fight or skip
var promptFight = prompt("Would you like to FIGHT or SKIP this battle? Enter 'FIGHT' or '​⬤