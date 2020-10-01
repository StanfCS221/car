# car
Modeling car-tracking as a Hidden Markov Model.
Tests and solutions for Stanford's CS221 class. This specific repo is focused on Bayesian Networks, modelling car-tracking as a Bayesian Network and calculating the probability of cars position being (x,y).
Observing distance provided by a noisy sensor reading and then using that reading to calculate the probabilities of car being in a position (x,y).
Using cars current position to estimate the probabilities of car travelling to a new position in a given time in order to avoid crashes.
Finally, using the fact that cars cannot teleport and have a partially predictable direction of moving we can totally dismiss calculating the probabilities of very distant position and just assume the probability of car being there to be 0 (if at a time t sensor says car is in Belgrade than we don't have to worry about it being in Paris at a time t+1). This shortcut is implemented using Particle Filtering.
