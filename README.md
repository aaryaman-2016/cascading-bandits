# Restless Cascading Bandits
Research Project on cascading multi-arm bandits where the rewards follow Markov Chains
This was my Summer Undergraduate Research Graduate Experience topic at IIT Kanpur during the summer of 2025 under the guidance of Professor Subramanya Swamy Peruru. 
We tudied the online restless bandit problem and have tried to implement the cascading effect to it. In our problem statement, the state of each arm of the Multi-Armed Bandit problem evolves according to a Markov Chain. The reward is based on the arm we pull and the current state of the corresponding Markov Chain. Additionally, unlike the traditional case, we are not restricted to pulling a single arm in each time-step. It is based on the Cascading Model, where up to K ≤ N arms can be pulled, where N is the total number of arms present in our case. The application ofthis concept is in various domains, for example cognitive radios. The importance of our problem statement is that it is more realistic than the case where we assumed the reward from an arm is identically and independently distributed because there is a chance of correlation between the past state and current state. For example: In cognitive radios, if a channel is sensed at some timestep t, and it is occupied, there is a higher probability of it being occupied in the timestep t + 1. In our research, we are attempting to propose an algorithm that efficiently combines the Restless-UCB Algorithm with modifications to adapt to the Cascading nature of our problem, using Whittle’s index as the Oracle to define the policy we use, and we attain $O(N)$ computationally complexity with sublinear bound on regret with respect to time i.e of the order $O(NT^{\alpha}) \ \alpha < 1$.

### Repository Contents 
This repository contains all the files related to the work done during the research which are 
1. The code through which we implemented the model
2. Test Cases on which we tested it which we picked up from [Restless-UCB](https://arxiv.org/pdf/2011.02664)
3. The report on the project
4. The poster for the project

