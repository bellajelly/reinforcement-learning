
# reinforcement-learning

Assignment: Q-Learning with OpenAI Gymnasium (Taxi-v3)
The goal was to implement a Q-learning agent from scratch, a foundational reinforcement learning algorithm, and observe it actually learn to solve a problem through trial and error.

We built:
A taxi agent that starts knowing absolutely nothing about its environment. Over 2000 episodes it fills in a 500×6 Q-table — one row per possible state, one column per possible action — using the Bellman equation to nudge its estimates toward better and better values after every single step. Epsilon-greedy policy balanced exploration early in training with exploitation later as epsilon decayed toward zero.
What was learned conceptually:

The Q-table is the agent's memory, zeros at the start, hard-won experience by the end
The Bellman update is just "nudge your old guess toward a better-informed new guess"
The TD error is literally "how wrong were you?" — and the brain's dopamine system may work the same way
All hyperparameters involve tradeoffs — there's no perfect setting, only balance

Outcome:
A trained agent that goes from completely random behavior to reliably picking up and dropping off passengers, measurable through average test rewards and a learning curve that visibly climbs over training episodes.
