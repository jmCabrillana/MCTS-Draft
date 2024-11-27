# Parrallel implementation of Monte Carlo Tree Search for Game Drafting

This library is a high speed implementation of Monte Carlo tree search guided by a policy and critic (based on transformer or Xgboost) for exploration. 
The tree is represented with a vectorize hash table (with pandas). Rollouts are performed in batch after a warm-up to discover the first elements of the game tree.

This code can run around 100k rollouts in 10 seconds which is suitable for online drafting in MOBA games
