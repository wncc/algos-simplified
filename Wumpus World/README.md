# The Wumpus World Agent
The Wumpus World Agent is an example of a Knowledge Based Agent (KBA) to represent Knowledge Representation. It is inspired by a video game **Hunt the Wumpus** by Gregory Yob in 1973.
Before we get to Wumpus World, let us first understand what are Knowledge Based Agents. 

## Knowledge Based Agents 
Watch this short video on KBAs - [Knowledge Based Agents and Entailment](https://www.youtube.com/watch?v=zOCTxedhf_c)
<br> Alternatively, you can refer to this detailed article on KBA - [Knowledge Based Agents in Artificial Intelligence](https://www.javatpoint.com/knowledge-based-agent-in-ai)

A basic Knowledge based agent can be used to solve logical puzzles where you are given some statements which only give partial information, and based on those statements you have to determine whether a statement or **query** is True or False by drawing inference and reasoning from the given knowledge. 
So instead of our brain doing the logical reasoning, we will build an AI which will do that reasoning to give the output. 

An example of such a puzzle is the **Knights and Knave** puzzle. 
The rules are that a Knight always tells the truth and a Knave always lies. Each player can be either a Knave or a Knight. 
Now lets say you are given the following information (Knowledge):
* There are two players, A and B
* A says that 'We are both Knaves'
* B says nothing. 

And your task is to determine whether a player is a Knight or a Knave. A Knowledge Based Agent should be able to finally say that A is a Knave and B is a Knight. 
<br>Basically, a KBA contains some information or **Knowledge** from the environment based on which it takes decisions on certain **actions** with proper reasoning and logic.
<br>So in the above example, the Knowledge Base will be formed using the information given in the question. Then your **Queries** will be:
* 'A is a Knight'
* 'A is a Knave' 
* 'B is a Knight'
* 'B is a Knave'

Now, the Knowledge Base will only be true for certain values of A and B, and whenever the KB is true, if the Query is true, then we say that the Knowledge Base entails the Query. This is known as **Entailment**. 

## Dive Deep
Now that you have an idea about Knowledge Based Agents and how they work, Lets try to solve the **The Wumpus World Problem**. 
<br>Head over to this link for a detailed description of the problem - [Wumpus World Description](https://www.geeksforgeeks.org/ai-the-wumpus-world-description/)
<br>You now must have a pretty good idea of the problem. Now the next step is to learn how you can convert Knowledge in form of statements into a language that your AI can understand.
For this purpose you must be familiar with different logical statements and operators. Checkout this video - [Logical Statements for evaluating Knowledge Base](https://www.youtube.com/watch?v=rfjSH-RA8So&list=PLjTSKEJpqIeDrUYF7DKspT2r9H38vg5dC&index=11)

Now you should have some idea on how you can solve the Wumpus World Problem. Try if you can code it by yourself. 
<br>If you face any problems while coding you can refer to the below links, but I would strongly suggest you to first try it yourself.
* [Wumpus World detailed](https://www.javatpoint.com/the-wumpus-world-in-artificial-intelligence) (Checkout other links on the same page)
* [Wumpus World Start-To-End implementation](https://github.com/rakeshgunduka/Wumpus-World/blob/master/wumpus.py) (Detailed Implementation of Wumpus World in Python)
* [Wumpus World further explanation](https://www.youtube.com/watch?v=C0Lcjke494w&list=PLjTSKEJpqIeDrUYF7DKspT2r9H38vg5dC&index=12)

Congratulations! You have created your first ever Knowledge Based Agent. This is just the start, try and find more implementations of KBAs for other problems and try to code them from scratch!
