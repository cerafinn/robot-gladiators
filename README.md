# robot-gladiators

## Description
A robot gladiator game created using Javascript that can be played in a browser console.



Table of Contents |
-------------------|
[Usage](#Usage)
[Technologies](#Technologies)
[Game Logic](#Game-Logic)
[Screenshots](#Screenshots)
[Contributing](#Contributing)
[Author](#Author)
[Questions](#Questions)

<br />

## Usage

The project is a JavaScript based game played within a browser console. The user is able to enter information into alert boxes and choose whether to fight or skip. After fighting, the user enters the shop and can choose to refill on health, upgrade attack or leave. After exiting the shop, as long as there are still enemy robots to fight, the user is given the option to fight or skip until all enemies have been defeated. After finishing the game, the user will be informed of their final score and be informed if they have beat the high score for the game or not.

You can find the deployed link and the repository link below:

Deployed Link: [Deployed Link](https://cerafinn.github.io/robot-gladiators)

Repo Link: [Repo Link](https://github.com/cerafinn/robot-gladiators)

<br />

## Technologies

* JavaScript

<br />

## Game Logic

1. Player is assigned money, HP and attack values

2. Function chooses the Opponent robot from the enemy array.
  * If no enemies exist, end of game (**STEP 6**)

3. Fight function runs:
  * Turn order is determined
  * Player's turn: choose to FIGHT or SKIP
    * if FIGHT, Player attacks and Opponent's health is reduced by random number based on Player attack power
    * if SKIP, Player loses money and triggers shop function (**STEP 5**)
  *Opponent's turn: Opponent attacks and Player's health is reduced by random number based on Opponent attack power
  * Repeat turns

4. Fight function continues until either opponent or player have 0 HP.
  * if Player HP = 0, end of game (**STEP 6**)
  * if Opponent HP = 0, triggers shop function (**STEP 5**)

5. Shop function runs:
  * Player can choose if they want to shop or not
    * if yes, can `refill` HP, `upgrade` attack or `exit` shop
    * if `refill` or `upgrade`, if Player can afford option the funds are deducted and the appropriate attribute is increased
  * After completing purchase or exiting shop, next round begins(**STEP 2**)

6. After completing the game, Player is told whether they have reached the high score and if they want to replay the game.
  * if replaying game, return to start of game logic.

<br />

## Screenshots

![IMG](./assets/images/robot-gladiators-screenshot.png)

## Contributing

If interested in contributing to the project, feel free to reach out. Contact information can be found in the Questions section.

<br />

## Author

Andaleeb Farooq: [:octocat:](https://github.com/cerafinn)

<br />

## Questions

If you have any questions or issues, feel free to reach out at: andaleeb.farooq@gmail.com.
You can also find more of my work on Github at [github link](https://github.com/cerafinn).