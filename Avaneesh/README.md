DQN Notebook

I started by implementing a tabular q-learning approach. This uses a q-table, where rows are different states, and columns are different actions. Each cell is a state-action value (q-value), and it's an estimate of how good taking that action in that state would be. 

In this process, the agent learns by taking an action according to the Epsilon-Greedy Strategy, where a random number is generated and compared against epsilon to determine whether the agent takes a random action or the best possible action in the CURRENT observation state. The environment progresses with this action and the reward/state of the agent in the next action are returned. Based on this reward, as well as the current q-values for the agent at this state/action and the next state (in the next state, the maximum possible q-value is selected), the current q-value is updated. This process repeats, allowing for the q-values to better reflect the rewards for picking each state.

TODO - do DQN and PPO