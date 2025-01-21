For transparency, we have disclosed transcripts of all games played in the experiments. These are contained in a single file, with the size of approximately 28MB, named:
experiments.txt
available at: https://github.com/MaciekArea7/data

This file contains lines of three types:

Header lines, which describe the settings of the parameters for the experiments that will follow this line until the next header line or the end of the file. For example:
Results of MCTS[Iterations=10000, PredictionFrequency=0, PredictionAccuracy=100] for Function1:

Game runs, which detail the number of the game in the current run, the moves taken by the player (as specified in the header line), and the final state of the game - where the player arrived (the x coordinate) and the game score (equal to f(x)). The moves taken during the game form a binary sequence, where 0 denotes the first action ("choose the left subset"), whereas 1 denotes the second action ("choose the right subset"), in the current state. For example:
Game 78 moves: 00000000000000101011010100 Final state: (x=0.04131346940994263, f(x)=0.9997325117156205).

Summary lines that follow the game runs. They contain a summary of the experiment described by the previous header line. They include the average score and the standard deviation. For example:
Summary of MCTS[Iterations=100, PredictionFrequency=20, PredictionAccuracy=40] Mean f(x)=163.4073 StdDeviation=132.8005.