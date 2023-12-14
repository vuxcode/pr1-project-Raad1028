[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-24ddc0f5d75046c5622901739e7c5dd533143b0c8e959d652212380cedb1ea36.svg)](https://classroom.github.com/a/knTkeOvY)
[![Open in Visual Studio Code](https://classroom.github.com/assets/open-in-vscode-718a45dd9cf7e7f842a935f5ebbe5719a5e09af4491e668f4dbf3b35d5cca122.svg)](https://classroom.github.com/online_ide?assignment_repo_id=12603021&assignment_repo_type=AssignmentRepo)
# Project Instructions
Follow the instructions here: https://vuxcode.netlify.app/new/pr1/lessons/major-project-brief/


# Project Summary

This project is a turnbased game where you battle enemies. The original idea was that you as a player would be a gladiator and had to battle your way through the colosseum in order to earn your freedom.

My idea of how the combat would work was to have 4 different actions that the player / enemy can pick and have them all interact with eachother. I also wanted it to all be centered around dicerolls.

I did want to add a shop to the game where the player could spend the gold they earn from their battles, although I feel like that would have taken a bit too much time and also the code was already very long. So I decided to not implement this to the project.

During the making of the project I did run into a couple of issues. One of those were that i had my mind set on how I wanted the UI to look, but I had next to no experience with HTML, so to tackle this I had to google a lot for the HTML part of the program. Another issue I had was when my code got too long to keep track of where everything is located. I tried to sort the code in a way that would be easier to navigate, but it was still pretty hard to keep track. I did find a bit of a solution that made it easier, which was by rightclicking on a function or a variable and then clicking "Go to definition".

Here's a list of stuff I would have improved if I had more time:

- A shop where the player could spend their gold in order to get better gear.
- A win condition, so there is an end to the game other than your character losing a battle.
- Tooltips for each of the combat buttons to explain how each action works.
- Have visual HP bars as well as the current text based system, I think that could make the user experience a bit better.

In terms of the budget I managed to stay below the 30 hour budget atleast for the time I spent actually writing code. I feel like I may have gotten some of my times in the time report wrong as I usually didnt keep track on the exact time I started each session, and would go by what time my first commit happened that day. If I were to include the time spent workshopping how the systems would work in my head, I would guess its a bit closer to the 30 hours

# User Guide

When you first start the program, you will get to a screen where you can decide what name your character will have.

Once you click the "Start the game" button, you will get to another screen where you have two different buttons you can click on. The first one being the "Battle" button which takes you to the combat screen. The other button is a shop button, although in this current state of the project there is nothing in that menu. Below these buttons your current gold amount is displayed.

Once in the combat portion of the program, you will be able to see your characters health in the top left corner or the screen, and the enemy's health in the top right.

Further down you will have 4 different buttons, these say "Regular attack", "Heavy Attack", "Parry" and "Dodge".

The regular attack button makes your character attempt a regular attack. The attack will hit if you roll a number higher than 10, then another dice roll will happen to decide how much damage the attack will deal. The damage roll is then multiplied with the regular attack modifier, which currently is .

The heavy attack works about the same, but will instead only hit the attack if a number above 12 is rolled. The damage roll will instead be multiplied with the heavy attack modifier, which currently is 0.8 so it will deal a bit more damage than a regular attack would have, most of the time.

The parry works a bit different. If you use the parry and you roll a number higher than whatever the enemy rolled, you cancel their attack and you get to attack them instead, with a parry attack modifier, which currently is 0.5. If you instead roll the same or below the enemy, the enemy attack will go through and you do nothing that turn.

The dodge also works a bit different. If dodge is used, you roll a dice that decides how successful the dodge was. Below is a list showing what all dice outcomes do:

    - 18-20: Take no damage from enemy this turn, you get a +2 next dice roll.
    - 13-17: Take 70% less damage from the enemy this turn, you get +2 next dice roll.
    -  8-12: Take 50% less damage from the enemy this turn, you get +2 next dice roll.
    -   4-7: Take 30% less damage from the enemy this turn, you get +1 next dice roll.
    -   1-3: Take full damage from the enemy this turn, you get +1 next dice roll.

Once you use a combat action, text will be written on the screen which says what happened during that turn. The health of each combatant also updates. 

What the enemy does for their turn is random, and has a 25% chance for each option.

If the enemy health goes below 1, the player wins the battle and gets a randomized goldreward and can try to do another battle where the enemy will have a bit more health.

If the player health goes below 1, the game is over and the player will have to reload the page to try again.