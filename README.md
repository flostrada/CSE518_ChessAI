# CSE518_ChessAI
# Introduction
The trade-off between intuition and calculation is a recurrent issue in chess. Calculation is exactly thinking over moves that the opponent can play to contradict your move, whereas intuition is finding plays that just "feels right" and "works well" in the position.
Positional play is related with intuition, while tactical play is associated with calculation. Tactical plays, on the other hand, can't be found without intuition, and positional play can't be done without some math. In this project, I'll aim to combine two algorithms, an intuition-based algorithm and a calculation-based algorithm, to create a more powerful algorithm than either of them could have been on their own.

# Approach
For creating the Chess AI, we will be using the convolutional neural network algorithm which will have an intuition-based algorithm and calculation-based algorithm to make an algorithm which is stronger than both alone.
->	We will be creating a board as a matrix which will be fed into the neural network(hybrid) as a processed 8x8 matrix and then it gives a move that can be played from the current position. We created the chess board by using the library. 
->	We created random boards to evaluate the possible moves. The analysing of the possible moves helps to predict the next move. Also, associating scores to the pieces helps to analyse and predict the next move. We created 14 boards to evaluate the position of pieces on the board. 
->	We created the convolutional neural layers to increase the accuracy of the moves using the relu and sigmoid function and also implemented a tensorflow library to execute the layers.
->	After creating the layers, we used to flatten and dense to get one possible move which can be played in order to win. We used 150000 board positions to compare the moves. After that we also added 25 epochs for testing.

![s](https://user-images.githubusercontent.com/68383587/143404281-fde4998a-eb74-44fb-93e4-e304620d9cd8.png)

![s1](https://user-images.githubusercontent.com/68383587/143404304-dd8db6ed-68f5-4200-b92d-4135a1fbbfed.png)

->	Next, we implemented the Minmax algorithm by visualizing all moves that can be made and evaluates finals moves Along with this we will be using alpha-beta pruning to optimize all the moves we got from minmax algorithm to find out the best move that can be made.
->	We used a stockfish engine to test our chess bot to evaluate the moves. 
Result
For the result we made the stockfish algorithm play with our Chess bot. Our programme sends 25 epochs to train and get the best move out of it. The bot plays against Stockfish. The bot couldn't win any games against the stockfish as we had a low accuracy rate and also we deployed only 25 epoch which limits the accuracy of the move. 
![image](https://user-images.githubusercontent.com/68383587/143404221-ba90817a-f94b-4101-9f0b-293ab458614a.png)
![image](https://user-images.githubusercontent.com/68383587/143404241-afcea0de-6972-4170-8dea-61a3528de9bb.png)
# References
1.	FreeCodeCamp.org. (2017, March 15). A step-by-step guide to building a simple chess AI. Retrieved from https://www.freecodecamp.org/news/simple-chess-ai-step-by-step-1d55a9266977/
2.	About DecodeChess - Company, Technology, and Management Team. (2021, February 24). Retrieved from https://decodechess.com/about/
3.	Paquier, M. (2020, July 21). Implementing a Chess engine from scratch. Retrieved from https://towardsdatascience.com/implementing-a-chess-engine-from-scratch-be38cbdae91
4.	Start Here with Machine Learning. (2021, October 25). Retrieved from https://machinelearningmastery.com/start-here/
5.	Start Here with Machine Learning. (2021, October 25). Retrieved from https://machinelearningmastery.com/start-here/
6.	S, V. (2021, August 23). Implementing A Deep Learning Chess Engine From Scratch. Retrieved from https://towardsdatascience.com/implementing-a-deep-learning-chess-engine-from-scratch-275e5c9b9e21#3fe4
7.	J, M. (2017, September 04). Chess Game Dataset (Lichess). Retrieved from https://www.kaggle.com/datasnaek/chess
8.	K, B. (2021, April 02). AI In Chess: The Evolution of Artificial Intelligence In Chess Engines. Retrieved from https://towardsdatascience.com/ai-in-chess-the-evolution-of-artificial-intelligence-in-chess-engines-a3a9e230ed50
