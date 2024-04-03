# DiceGame
   A recreation/updated version of my first coding project in university.

### The Game
   The UI is printed to the terminal.
   
   The first page the user sees is the main menu which looks like:
   
                     Dice Game               
       [p] to play
       [b] to see score board
       [e] to exit

   All the menus have a similar syntax. The charactor within the [ ] is what should be entered to pick that option.

   The scoreboard shows the top 50 scores stored in the text file. 

                      Top 50               
       01.    mee               101
       02.    rfv               097
       03.    ton               091
       04.    ---               ---
       05.    ---               ---
        .      .                 .
        .      .                 .
        .      .                 .
   
   User would need to navigate to the text file manually if they wish to see more then just the top 50 scores.

   The UI for the actual game:

       Round [1]
                      Board                
       01 02 03 04 05 06 07 08 09 10 11 12 
        o  o  o  x  x  o  o  o  o  o  o  o 
       You rolled: 2 & 5
       What would you like to do?
       [c] to combine
       [s] to split
       [g] to give up

   Two dice are rolled and user can choose to 'split' to drop both numbers from the board: o -> x under that number.
                                           or 'combine' to drop the number equal to the sum of the 2 rolled numbers.
                                           or 'give up' which results in the lost screen.
   This implementation does not force a lose screen, it will simply prompt the user to choose another option if the one they picked was invalid.

   The lost screen:

                      You Lost!               
       Score: 20
       [---] type 3 char to record your score!
       [q] to quit without recording your score

   User can give a three character name to be recorded in the score board or quit without recording their score.

   The win screen is basically the same, other then that it only triggers when there are no 'o's on the board.
       *note: I've not been able to 'win' yet so functionality have not been tested...
   
