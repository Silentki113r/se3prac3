2048 Test Plan
========

Background
========

The objective of this game is to merge numbered tiles until you have one tile equal to 2048. The user manipulates the game by ‘tilting’ the board up, right, down, left in direction. If two tiles are the same number and are in line with each other are moved to a direction, which will allow a ‘merge’, a new tile is formed with the value of the total of the two tiles that merged. As the game progresses and as ‘tilts’ are performed, new tiles are created and positioned at random on the board. The user will merge as many tiles and as many times as needed to make a tile with the value 2048 WITHOUT filling the board with tiles and running out of possible merges as this will end the game short.


Specifications for running
========

For General use:
For anyone wanting to play the game, with no other obligations.

•	Web browser that allows JavaScript.

You can also of course play this game via the command line with the appropriate files.

For use of testing/changing program:
For anyone wanting to look at how the program runs, test it, make or suggest improvements.

•	GitHub Account

•	IDE – Not Netbeans save yourself a headache

•	C compiler and library – Mac OSX Mavericks…… What a joke.

Testing
========

There are many aspects of this game that can be tested, such as:

•	Movement of tiles

•	Merging of tiles

•	Game initialization

•	Game end point (no more moves AND 2048 tile)

•	Random placement of new valued tiles after each tilt

•	Tiles merge with appropriate tiles (eg. same value)

•	Scoring

Other aspects, which effect the games functionality:

•	Event handling (user input)

•	Event recognition (user input)

•	Action Listeners (user input)

TEST: Movement of tiles
========
[UNIT TEST]
Testing if program can handle basic movement of tiles, what can be tested?

•	Move tiles to the left

•	Move tiles to the right

•	Move Tiles up

•	Move Tiles down


Anomaly checklist:

•	Do tiles ‘fall off’ board (eg, need to stop at edge).

TEST: Merging of tiles
========
[UNIT TEST]
Test to see if tiles merge after tilt, how to test?

1.	Tilt in a direction that would result in an expected merge of tiles.
2.	Did tiles merge?
3.	If(no) fix else cool


TEST: Game initialization
========
[UNIT TEST]
Does game initialize with two randomly placed tiles each with a value of two and score is set to zero?

•	Load game

•	Inspect

TEST: Game end point
========
[UNIT TEST]

The game ends when there is either; a tile of value 2048 or no more free spaces on board and no more possible merges. To test this:

•	Make a tile 2048 → Did this bring the game to a defined end?

•	Fill boards and have no more available merges → Did this bring the game to a defined end?

User should be notified and denied the ability of further action on the game if it is at its end point.

TEST: New Tiles after each tilt
========
[UNIT TEST]

New tiles must be created at random positions after each tilt. Test:

1.	Tilt
2.	Does new tiles appear?

I think after briefly playing the game two tiles each with a value of two should be created.

TEST: Tiles merge with appropriate tiles
========
[UNIT TEST]

Very similar to the second test, this is trying to break the game by merging tiles with different values.

1.	Line up tiles with different values
2.	Spam tilt in the direction that would otherwise result in a merge.
3.	Did the suspect tiles merge?

Tiles of different values should NEVER merge.

TEST: Scoring
========
[UNIT TEST]

Does score update while game is playing? How will the user be able to compare scores with others or past attempts with out this? Test:

•	Start game

•	Play

•	Is score adding and displaying accordingly?

TEST: Event Handling
========
[BLACK BOX TEST]
 Does program handle events properly such as, action listener → tilt → merge → score.

This is tested in relatively similar means as most of the tests here however in this instance we are testing all of them. SO in this instance it’s a black box test because it is the whole system.

TEST: event recognition
========
[UNIT TEST]

Does system recognize when an event takes place? Test:

•	Do something that would result in a response from the system

•	Was there a valid/expected result?

TEST: Action Listener
========
[UNIT TEST]

DO the action listeners cause appropriate function on system. 

•	Press key to tilt left.

•	Did game tilt left?

•	If(yes) action listener work for left tilt (no) check action Listener


Other methods of testing
========

Other methods, apart from those used above (unit and black box), can be used to greater the game. Comparison testing could expand/refine the requirements of what makes a game appealing to the user. This is done by testing other games of the same genre.



