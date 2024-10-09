# CI2024_lab1

## Algorithms used
- random mutation hill climber with single and multiple tweaks
- random mutation hill climber with strength controlling mutation
- random mutation hill climber with multiple tweaks with mask with a certian probability
- simulated annealing

## Results
Starting with the same solution, composed of "True" sets with probability of 50%:
The simple RMHC with multiple tweaks resulted to be the worst solution, having a minimum cost found almost 5 times worse than the others solutions.
On the other hand the other 3 implementations got similar results.
More specifically the simultated annealing implemented uses a temperature initially set to 1565 in order to get a initial probability of 0.8 to accept a worse solution. This was chosen looking at the "deltas" between the fitnesses of the solutions. At every step the temperatures is decreased by a factor of 0.99, since reducing it more would result in a worse solution given the much higher drop of temperature for the number of MAX_STEPS performed used.
A very good solution resulted to be the random mutation hill climber with a strength controlling mutation, and with some trials it turned out to be 0.5 a good initial strengthm, combined with the 1/5 rule.

## COllaborations
Ideas and suggestions were shared with fellow  [colleague](https://github.com/GioSilve).