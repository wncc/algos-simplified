# Mini-Max Algorithm
Mini-max algorithm is a recursive or backtracking algorithm which is used in decision-making and game theory. 
It is a very useful concept when you are coding an Artificial Intelligence for a Two player game where the players are playing opposite to each other, for eg: Chess or Tic-Tac-Toe. <br>
At any point in the game, it provides an optimal move for a player assuming that the opponent is also playing optimally.
<!Let's say we are playing a Two-player game like Tic-tac-toe or chess.
Now if we want to design an artifical intelligence which can play as one of the players, one way to do that would be to write a search algorithm which would search through all the moves possible at any point in the game and then decide its move accordingly. 
But as you might have guessed, this AI will be extremely slow as even in a game as simple as Tic-Tac-Toe, there are many possible ways in which the game can end and going through each one of them will turn out to be computuatinally very heavy. 
So for this we use another algorithm called as the Mini-Max algorithm. >

Take a look at this short video which will help you understand the basic concept behind the Mini-Max algorithm. <br>
[MiniMax Algorithm](https://www.youtube.com/watch?v=l-hh51ncgDI&list=PLVvtilrUrltXmTs4Lw0gHxzckiqXC-gV2&index=2&t=0s)
<br>
## Alpha-Beta Pruning
 Now that you have a basic idea on what exactly is MiniMax and how it works, let us see how we can make it work even faster! <br>
 Alpha–beta pruning is a search algorithm that seeks to decrease the number of nodes that are evaluated by the Minimax algorithm in its search tree.<br>
 Alpha-Beta pruning is not actually a new algorithm, rather an optimization technique for minimax algorithm. It reduces the computation time by a huge factor. This allows us to search much faster and even go into deeper levels in the game tree.
 It is called Alpha-Beta pruning because it passes 2 extra parameters in the minimax function, namely alpha and beta.
<br>
 
 Checkout this video which explains aplha-beta pruning in much more detail - <br>
 [Alpha-Beta Pruning](https://www.youtube.com/watch?v=xBXHtz4Gbdo)
 <br>

## Dive Deep
 Now that you have read about how you can make your MiniMax algorithm even faster, let's put that knowledge to use! <br>
 Your task is to make a Tic-Tac-Toe AI using your knowledge of MiniMax algorithm and then using optimisation techniques like Alpha Beta Pruning to make it run even faster. 
 Lets see if you can beat your AI or your AI beats you! <br>
 
* First try writing the Max and the Min function by yourself. You can make use of any programming language you prefer. You can refer to this article if you get stuck or if any part of the algorithm is still unclear - <br>
    [MiniMax Algorithm in Game Theory](https://www.geeksforgeeks.org/minimax-algorithm-in-game-theory-set-1-introduction/)
    <br>
    
 
* Once you are done with writing the Max and the Min function, your next task is to write the 'Evaluation Function' which should only be called when the game has ended and should return the result of the game ( X win, O win or Tie ).
    You can checkout this link if you are having trouble writing some part of the code - <br>
    [Evaluation Function](https://www.geeksforgeeks.org/minimax-algorithm-in-game-theory-set-2-evaluation-function/?ref=rp)
    <br>
 
*  Now you are almost done with your game. Let's combine whatever you have learnt till now, and then use that to write your final piece of code!
    <br> For this task, You have to write a function which determines the next optimal move for the AI. This function will make use of the Evaluate function and the Min-Max functions that you previously wrote. 
    <br> Checkout this link for reference - <br>
    [Optimal Move Function](https://www.geeksforgeeks.org/minimax-algorithm-in-game-theory-set-3-tic-tac-toe-ai-finding-optimal-move/?ref=rp) 
    <br>
 
* Now, you can see that your AI takes some time to process in the first few moves because the cases to search through are more.
    Your next task will be to implement Alpha Beta Pruning in your code to make your AI faster!. Check out this link if you get stuck - <br>
    [Alpha Beta Pruning in Tic-Tac-Toe](https://www.geeksforgeeks.org/minimax-algorithm-in-game-theory-set-4-alpha-beta-pruning/)
    <br>

 <b>Great!</b> You are all done now and you have finally created your first-ever AI. If your code is correct, you can see that the AI never loses! Let's see if you can beat your own AI!
 
 
 Checkout this amazing video which explains the whole process from start to beginning in a concise manner - 
 <br>
[Tic-Tac-Toe with MiniMax algorithm from The Coding Train!](https://www.youtube.com/watch?v=trKjYdBASyQ)
<br>
