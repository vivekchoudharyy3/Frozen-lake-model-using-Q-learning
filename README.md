# Frozen-lake-model-using-Q-learning

In this assignment you will build a simple reinforcement learning agent which uses q- learning to play the game frozen lake". 
The frozen lake is a 4x4 grid represented as the following: Representation Character meaning SFFF 
(S: starting point, safe) (F: frozen surface, safe) (H: hole, fall to your doom) HFFG (G: goal, where the frisbee is located) 
The description of the problem is: "Winter is here. You and your friends were tossing around a frisbee at the park
when you made a wild throw that left the frisbee out in the middle of the lake. 
The water is mostly frozen, but there are a few holes where the ice has melted. 
If you step into one of those holes, you'll fall into the freezing water. 
At this time, there's an international frisbee shortage, so it's absolutely imperative that you navigate across the lake and retrieve the disc. 
However, the ice is slippery, so you won't always move in the direction you intend." 
Below, I have started a program for you to implement a q-learning strategy to solve this problem. 
Each episode consists of restarting the environment state selecting and performing actions (for a maximum of max_steps steps) 
updating the q table after each step keeping track of the total reward for the episode 
Report the reward averaged over the episodes as well as the reward for the last episode. 
The initial hyperparameters are defined for you, but you can vary these to see how they affect performance. 
When you select an action, add some element of chance by using the exploration versus exploitation option (the value of e is provided in the code below). 
At the end of each episode, update the exploration parameter to decrease it with experience: E=minepsilon+(maxepsilon-minepsilon)xe-decayratexepisodenumber. 
Report the best results you observed and the hyperparameters that achieved those results.
