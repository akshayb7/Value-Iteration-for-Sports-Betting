# Value Iteration for Sport Betting

A betting man has the opportunity to make bets on the outcomes of a sporting event. If the team he bets on wins, he wins as many dollars as he has staked on that result; if his team loses, he loses his stake. The game ends when the betting man wins by reaching his goal of $100, or loses by running out of money. On each bet, he must decide what portion of his capital to stake, in integer numbers of dollars.

The problem can be formulated as an undiscounted, episodic, finite MDP. The state is the betting man’s capital, s ∈ {1, 2, . . . , 99} and the actions are stakes, a ∈ {0, 1, . . . , min(s, 100−s)}. The reward is zero on all transitions except those on which the gambler reaches his goal, when it is +1. The state-value function then gives the probability of winning from each state. A policy is a mapping from levels of capital to stakes. The optimal policy maximizes the probability of reaching the goal.

We will use value iteration method (Dynamic Programming) to solve this problem and hence assume that the agent knows the environment dynamics such as reward function and number of states.
