# Chess_AI_Engine

This is Chess AI engine i.e a set of algorithms that analyses positions and make decisions leading to the best possible move.
This involves several algorithms in order to make AI as efficient and as intelligent as possible.

## Usage
The project contains two cpp files:-
1. chess.cpp (naive algorithm)
2. negamax_alpha_beta.cpp (optimized one)

Run any of these files on terminal

## References to Algorithms used
Tree Traversing Algorithms
In order to develop a chess engine, an initial foundation layer has to be implemented: ‘min-max’ algorithm. This is a tree traversing type of algorithm and it is responsible for creating the tree itself and the rules for traversing it. A layer called ‘alpha-beta’ is added after, that improves tree traversing, by pruning it significantly. 
With all these features implemented, the chess engine can traverse a tree with a depth of 4-5 in couple of seconds. All these algorithms together with the evaluation function are described below.

[Minimax](https://en.wikipedia.org/wiki/Minimax)

[Alpha beta pruning](https://en.wikipedia.org/wiki/Alpha%E2%80%93beta_pruning)

[Negamax](https://en.wikipedia.org/wiki/Negamax)

Evaluation function:-
The purpose of the evaluation function is to assign a score to each node from the bottom of the tree. The more complex the evaluation function is, the slower the tree traversing will be, even though the assigned score will be more accurate. The most basic evaluation function contains a feature called material evaluation, in which the score is assigned depending on the number of pieces each side has and their weights. For example, a bishop is worth much more than a pawn.

[Simplified Evaluation Function](https://www.chessprogramming.org/Simplified_Evaluation_Function)

## Complexity of Chess 
    • 20 possible start moves, 20 possible replies, etc.
    • 400 possible positions after 2 ply (half moves) 
    • 197 281 positions after 4 plies 
    • Exponential explosion! 
    • Approximately 40 legal moves in a typical position 
    • There exist about 10120 possible chess games

Chess is so complicated that a computer can never solve the game. Computer can work smart and respond optimally to the user move with help of some decision-making algorithms.

## Real time performance of this chess engine
We analysed the average time taken for one ply (taking depth 5) by chess.cpp and negamax_aplha_beta.cpp

chess.cpp - 140 seconds

negamax_aplha_beta.cpp - 20 seconds
