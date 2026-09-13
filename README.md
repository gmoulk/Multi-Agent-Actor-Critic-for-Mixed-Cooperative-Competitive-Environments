# Multi-Agent Actor-Critic for Mixed Cooperative-Competitive Environments
Implementation of the paper can be seen in MAAMC_RL.ipynb

At first we define 3 predators ,1 pray,2 obstacles and 25 maximum number of en-
vironment steps per episode.We define the number of episodes to 2000,gamma to 0.95
and learning rate to 10−3. We furthermore define Actor and Critic neural networks and
the ReplayBuffer and furthermore define soft-updates.
Then we proceed defining the training loop, where we first reset the environment,
for every agent chose one action, advance the environment, store information in the
replay buffers, during the training we need to update Critic and Actor and soft update.
After the training loop we implemented the evaluation loop where every agent
selects deterministically and updates the environment.
