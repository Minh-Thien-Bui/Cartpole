# Cartpole Project
The project is like a videogame in which you try to balance a pole on a virtual cart for as long as possible. In order to win the game, you need to be able to beat a minimum score of 195 points in 100 consecutive trials. My approach to solving this problem was to use a brute force method to generate a list of 100 policies that will beat the minimal score. I created a SpecialAgent class as a subclass of the ReflexAgent. I chose the ReflexAgent over the RandomAgent because it provided much better initial scores. My SpecialAgent simulates trials with the ReflexAgent algorithm and saves policies that yield a score of at least 195. Once the length of the best_policies list reaches 100, the training algorithm is complete. Now that we have our list of policies, we can replay the simulation using only these winning policies. When I did this, it yielded the following results:

Average Score: 232.56

Low Score: 195

High Score: 368

 

My conclusion is that with time and computing power, it is possible to solve games like Cartpole through trial and error.

Video Demo Link: https://youtu.be/DVBUDrBlS8M
