<!DOCTYPE html>
<html>
<head>
	<meta charset="utf-8">
	<link rel="stylesheet" href="https://use.fontawesome.com/releases/v5.7.1/css/all.css">
	<meta name="viewport" content="width = device-width, initial-scale = 1">
	<link rel="stylesheet" type="text/css" href="index.css">
	
	<link href="https://fonts.googleapis.com/css2?family=Major+Mono+Display&amp;display=swap" rel="stylesheet">
	
	
	<link rel="stylesheet" href="https://fonts.googleapis.com/css?family=Tangerine">
	<link rel="shortcut icon" href="./Assets/pyramid.ico" type="image/x-icon"/>
	<title> Game of Nim </title>
</head>
<body>

	<div id = 'header'>
		<div id='heading'>
			<h1>
				The Game of Nim
			</h1>
		</div>

		<span id="help"> <button> Instructions </button></span>
	</div>


	<div class="card-container" id="help-container">
		<div class="card ">
			<div class="info">
				<h1 class="card-title"> Man vs. Machine! </h1>
				<p>
					<p>How to play?<p>
					<p>Hello mortal!<p>
					<p>You and the computer take turns and in each turn, you choose one row and remove one or more sticks present in that row.
					You must remove at least one and may also choose to remove all the sticks from that row! But you must remove sticks only from one chosen row in a turn.
					Whoever removes the last stick loses the game! So your objective must be to make the computer remove the last stick.
					Also, you decide who goes first. You clearly have the upper hand, or do you?<p>
					<p>Good Luck!<p>
				</p>

				<div class="play-game" id="play-button">
					<a href="#" class="button instagram"><span class="gradient"></span>Enter Game</a>
				</div>

			</div>
			
		</div>
	</div>

	<div id="game-container">
		<div id="board">
			<div id="row1" class="row">
		        <div id="stick" *ngFor="let stick of sticks[0]; let i = index" onclick="hideStick(0, 0)">

		        </div>
		    </div>
		    <div id="row2" class="row">
		        <div id="stick" *ngFor="let stick of sticks[1]; let i = index" onclick="hideStick(1, 0)">

		        </div>
		        <div id="stick" *ngFor="let stick of sticks[1]; let i = index" onclick="hideStick(1, 1)">

		        </div>
		        <div id="stick" *ngFor="let stick of sticks[1]; let i = index" onclick="hideStick(1, 2)">

		        </div>
		    </div>
		    <div id="row3" class="row">
		        <div id="stick" *ngFor="let stick of sticks[2]; let i = index" onclick="hideStick(2, 0)">

		        </div>
		        <div id="stick" *ngFor="let stick of sticks[1]; let i = index" onclick="hideStick(2, 1)">

		        </div>
		        <div id="stick" *ngFor="let stick of sticks[1]; let i = index" onclick="hideStick(2, 2)">

		        </div>
		        <div id="stick" *ngFor="let stick of sticks[1]; let i = index" onclick="hideStick(2, 3)">

		        </div>
		        <div id="stick" *ngFor="let stick of sticks[1]; let i = index" onclick="hideStick(2, 4)">

		        </div>
		    </div>
		    <div id="row4" class="row">
		        <div id="stick" *ngFor="let stick of sticks[3]; let i = index" onclick="hideStick(3, 0)">

		        </div>
		        <div id="stick" *ngFor="let stick of sticks[1]; let i = index" onclick="hideStick(3, 1)">

		        </div>
		        <div id="stick" *ngFor="let stick of sticks[1]; let i = index" onclick="hideStick(3, 2)">

		        </div>
		        <div id="stick" *ngFor="let stick of sticks[1]; let i = index" onclick="hideStick(3, 3)">

		        </div>
		        <div id="stick" *ngFor="let stick of sticks[1]; let i = index" onclick="hideStick(3, 4)">

		        </div>
		        <div id="stick" *ngFor="let stick of sticks[1]; let i = index" onclick="hideStick(3, 5)">

		        </div>
		        <div id="stick" *ngFor="let stick of sticks[1]; let i = index" onclick="hideStick(3, 6)">

		        </div>
		    </div>

		    

		    <div id="next-move">
		        <button mat-raised-button color="warn" onclick="computerMove()">Machine's move!</button>
		    </div>

		    <div id="new-game">
		        <button mat-raised-button color="primary" id="new-game" onclick="newGame()">
		            New Game
		        </button>
		    </div>



		</div>

		<div id="winner-div">
			
		</div>

		<div id="scoreboard">
	      <div>
	        Machine
	      </div>
	      <div>
	        You
	      </div>
	      <div id="machine-score">
	        0
	      </div>
	      <div id="your-score">
	        0
	      </div>
    	</div>
		
	</div>


	<script type="text/javascript" src='index.js'></script>

</body>
</html>