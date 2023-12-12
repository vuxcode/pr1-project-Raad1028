# Time Report

- 2023-10-30 14:00 Worked for 1 hour and 30 minutes.
  - Implemented the diceroll function
  - Learnt how to edit innerHTML instead of using document.write.
  - Added comments.

- 2023-10-31 14:30 Worked for 2 hours.
  - Started working on the different actions, focusing on the regular attack today.
  - Created a way to determine what the enemy will do for their turn.
  - Made it possible quickly see what each button press does by looking in the console.

- 2023-11-5 16:00 Worked for 2.5 hours.
  - The regular attack action is now at a state where it accounts for all different dice outcomes.
  - Started working on the heavy attack action, was easier since it works almost the same as the regular attack, so I mostly copied code from the regular attack.
  - Made some repeated code into functions instead to make the code fewer lines, although there is more to improve upon here.

- 2023-11-10 14:30 worked for 3 hours
  - Implemented both the parry and the dodge actions.
  - Made all the damage modifiers more flexible.
  - Added a way to display HP and the turn counter on the screen.
  - Continued to improve upon reducing the amount of repeated code.
  - I think all possible turn outcomes is accounted for. Also, the HP variables gets updated now, so damage is actually being dealt.

- 2023-11-12 15:45 worked for 1 hour
  - Dodge advantage is now being added to the dicerolls as intended.
  - If a combatant has a dodge advantage for the upcoming turn it will be shown on the webpage.
  - Other minor changes to the code.

- 2023-11-13 17:00 worked for 2 hours
  - Implemented menues with different buttons. Now when you first load the program you land on the main menu, then you get to the overworld menu and when you click the battle button, you get to the combat screen etc.
  - Worked on the UI, making the combat buttons bigger, and in a locked position.
  - After every turn, a message showing everything that happened that turn is displayed.

- 2023-11-17 16:30 worked for 1 hour
  - Added a text input where the user can pick a name for their character.
  - If the user inputs the name "DEV", elements inside the devBtns divider will be shown. Currently only has the dice test, will probably add more stuff for when i start the work on the shop.
  - Tried to make the main menu UI a bit better. An issue I had is making the "Name your character" text locked in a position no matter what zoom you have on your browser but was unsuccessful. Will revisit in future.

- 2023-11-24 15:30 worked for 1.5 hours
  - Added currency and a way to add currency if devBtns are enabled.
  - Started working on the shop, added buttons for that screen and made them do what they are supposed to.
  - Some UI improvements

- 2023-12-1 14:00 worked for 2 hours
  - Implemented a check for if any combatant is below 1, and if that is the case, the other combatant wins.
  - If the player wins, they are now awarded with gold.
  
- 2023-12-7 17:00 worked for 1 hour
  - Made the enemy health be progressively higher for each battle.
  - The amount of gold rolls is decided by how many battles has been completed.
  - A bunch of fixes to some actions not actually dealing the damage it says it should.

- 2023-12-12 18:00 worked for 2 hours
  - Bugtesting and fixing the issues found.
  - Made sure that you can't continue if a battle ends in a loss or a draw.