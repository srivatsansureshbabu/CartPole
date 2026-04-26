# CartPole
The Cart Pole is a simulated environment, where there is, simply a cart and a pole together. The cart has to move a certain way in order to keep the pole upright. However, this is much harder than it looks, we can't just use simple if statements on the positioning in order to self balance the pole. We need to use a special kind of machine learning, called reinforcement learning. 

# Knowns
From the Cart-Pole, we have four different variables that we know. We have the cart position, cart velocity, pole angle, and pole angular velocity. These variables are from observations of the frame. With this observation, we then need to take the most optimal action next. When we take an action, we get a new observation, and we keep stacking observations and actions. 
# Policy
For our policy, we used the Proximal Policy Optimization, with the MLPPolicy. The Proximal Policy Optimization rule is essentially to try different actions, many many times. It learns which actions are good, and which actions are bad. The MLPPolicy, just refers to the architecture that this PPO model uses. It returns a tensor of [left,right], where it will show the probability of the cart going left, and the probability of the cart going right. For example, [0.2,0.8], is the probability that the cart goes left is 20%, and the probability that the cart goes right is 80%. 


[Watch CartPole Demo](CartPole_Balancing_RL_10000.mp4)
