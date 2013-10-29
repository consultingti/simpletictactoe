simpletictactoe
===============

simple angularjs tictactoe game - basic - tutorial

Basically we wanted to focus to the initial part of our study around this book providing examples 
around data binding, the watch function and CSS classes. We did not wanted to do the “Hello world” example 
from the book; as always we tried to do something fun, so we thought, let’s do a simple TIC-TAC-TOE game experience. 

For our little experiment we used AngularJS (of course, the star of the article) and also BootStrap as we wanted to play a little more and combined tools. Below you can find a brief definition of both items. After we’ll go into the example:
1)	AngularJS: open-source javascript framework, maintained by Google that assists with running single-page applications. Its goal is to augment browser-based applications with MVC capability, in an effort to make both development and testing easier. – Wikipedia
2)	$watch: this is used in AngularJS. It is a $scope function that is called with an expression to observe and a callback that gets invoked whenever that expression changes. 
3)	Bootstrap: sleek, intuitive and powerful mobile front-end framework for faster and easier web development. – Bootstrap

What do you need?
1.	Download Bootstrap from http://getbootstrap.com
2.	Download AngularJS from http://angularjs.org 
3.	Some knowledge about HTML, CSS, Javascript. But no expert level is required for this simple example. 

Try the TicTacToe here: http://www.sunitedsolutions.com/tictactoe/default.html 

Explanation of the Controller code:
-	simpleGameController: is our AngularJS controller receiving the scope object, which refers to the application model. 
-	Player variable: to flag if is “X” or “O” that is playing. In our example “X” is the starting user always. As I said it is a simple demo so in this example you don’t get to choose who plays first, in this case the “X” will always play first. 
-	There are 3 arrays (row1, row2, row3) for the rows. In each array you have:
o	 Title. Initialize with string ”xod”. As the player clicks this value will change either to “X” or “O”, depending on the user. 
o	Played. Initialize to “false”. As the player clicks it will change to “true” indicating you cannot click again on that cell. 
-	Winner: function that indicates if a user won. 
-	Clickrow: it is triggered when you click a cell where the user is playing. It received the parameter rowCoord, which indicates what cell was clicked. It also loads the modal window indicating the turn of the user.
-	Inigame: just called when the page loads to start the game, indicating the first player. 
-	$watch: angularjs goodie that we use to observe the player variable. When this variable changes the value the winner function gets trigger to check if there was a winner or not. 

You can read the post here: 
