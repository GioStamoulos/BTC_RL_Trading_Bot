# BTC_RL_TRADING_BOT

**About**  

A trading bitcoin agent was created with deep reinforcement learning implementations. Various experiments were performed on the type of neural network, the type of reinforcement
learning algorithm and the number of daily input values that initially required from agent to make the first decision. Also, the agent was made with the assumption that for each 
day could ‘Sell’ or ‘Buy’. 

**Environment & RL Algorithms**  

The agent’s environment (StocksEnv) is an environment that simulates buying and selling situations and can be found at [1] . More specifically,  the transactions concern Bitcoin 
cryptocurrencies and for the training of the agent the "Historical Bitcoin Dataset" was utilized, which consists of Bitcoin values from January 2012 to March 2021. The 
reinforcing learning algorithms used are the Asynchronous Advantage Actor Critic (A2C), Actor Critic using Kronecker-Factored Trust Region (ACKTR),  Proximal Policy Optimization  
(PPO1) and Trust Region Policy Optimization (TRPO) that was entered through the stable baselines library [2]. Every  agent was trained in whole dataset  except the last 100 
days-values, which are used to evaluate the agent based on the  price of profit. Finally, the time window's size was 20 or 30 or 50 daily input values.

**Results**  

|DRL AGENT	   |  FINAL REWARD	|        PROFIT |
| :---         |     :---:      |          ---: |
| A2C_20	|26420	|1.371|
|A2C_30	|3574	|0.814|
|A2C_50	|29394	|1.498|
|PPO1_20	|12945	|1.014|
|PPO1_30	|38136	|1.782|
|PPO1_50	|30188|	1.680|
|ACKTP_20	|19452|	1.022|
|ACKTP_30	|30300|	1.405|
|ACKTP_50	|20119|	1.248|
|TRPO_20	|29530	|1.544|
|TRPO_30	|19910	|1.110|
|TRPO_50	|14969	|1.187|


**References**  

[1]   https://github.com/AminHP/gym-anytrading  
[2]   https://stable-baselines.readthedocs.io/en/master/index.html 
