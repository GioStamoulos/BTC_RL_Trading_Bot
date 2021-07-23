# BTC_RL_TRADING_BOT

**About**

A trading bitcoin agent was created with deep reinforcement learning implementations. Various experiments were performed on the type of neural network, the type of reinforcement
learning algorithm and the number of daily input values that initially required the agent to make the first decision. Also, the agent was made with the assumption that for each 
day could ‘Sell’ or ‘Buy’. 

**Environment & RL Algorithms**

The agent’s environment (StocksEnv) is an environment that simulates buying and selling situations and can be found at https://github.com/AminHP/gym-anytrading. More specifically, 
the transactions concern Bitcoin cryptocurrencies and for the training of the agent the "Historical Bitcoin Dataset" was utilized, which consists of Bitcoin values from January 
2012 to March 2021. The reinforcing learning algorithms used are the Asynchronous Advantage Actor Critic (A2C), Actor Critic using Kronecker-Factored Trust Region (ACKTR), 
Proximal Policy  Optimization  (PPO1) and Trust Region Policy Optimization (TRPO) that was entered through the stable baselines library (https://stable-
baselines.readthedocs.io/en/master/index.html ). Every  agent was trained in whole dataset  except the last 100 days-values, which are used to evaluate the agent based on the 
price of profit. Finally, the time window's size was 20 or 30 or 50 daily input values.

