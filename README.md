# Generating-A-Batting-Lineup-Using-Genetic-Algorithm
Optimization Problem Choosing seven batsmen from a pool of 15 batsmen to maximize the number of runs scored in an innings in a T20 game.

#Optimization Problem
Choosing seven batsmen from a pool of 15 batsmen to maximize the number of runs scored in an innings in a T20 game.

#Why choose a genetic algorithm?
There are two limiting factors for run-scoring in cricket--the number of balls allowed per innings and
number of wickets allowed.
An innings in a T20 game, disregarding extras, consists of 120 balls. Even though each team is allowed
10 wickets in an innings, it is the wickets of batsmen that matter the most. Since more often than not
teams play seven batsmen, a team’s batting ability is exhausted once these seven batsmen are dismissed.
Thus, we can consider the number of balls available in an innings as 120 and the number of wickets
available are 7.
The goal of a batting team is to score as many runs as possible. This is achieved by minimizing the
number of wickets they lose and maximizing the number of runs they score per ball. Cricket teams, often,
come up with different combinations of batsmen to meet this goal.
For instance, a team could play three batsmen who, on average, face 50 balls and strike at 100 at the top
of the order. This would mean that the team is most likely to score 120 runs off their 120 balls with a loss
of two wickets. This is a waste of resources since the team has not made use of their remaining four
batsmen. In contrast, a team could play seven batsmen who average 15 balls per innings at the strike rate
of 150. This would mean that the team would end up scoring 157 runs but would have faced only 105
balls--which is a waste of 15 balls. So, the goal here is to ensure both the balls available and the wickets
remaining are made optimum use of to maximize run scoring.
When a pool of x players is considered, choosing 7 batsmen out of the pool becomes a permutation (as the
order matters) problem. x!/(x-7)!
If we assume x to be 50, and we try to handpick seven batsmen from this pool with the objective of
maximizing the number of runs scored, then the search space for this problem is 503,417,376,000, which
is extremely large. As x could be any number, the quest to find out the best permutation of seven batsmen
generates a search space that is theoretically infinite.
Since exploring such a large state space is computationally very expensive, and thus, practically
implausible, we need to adopt a heuristic approach to find the optimum combination. So, a genetic
algorithm suits our needs better than a mathematical solution.
For this assignment, we will keep x to 15, a more realistic case where seven genuine batsmen are selected
from (generally) a fifteen-member squad. Could compare the performance of the algorithm compared
with other approaches.
For x=15, the search space is 32,432,400
= 15!
(15−7)!
