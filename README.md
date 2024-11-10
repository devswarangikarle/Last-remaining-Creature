# Last-remaining-Creature

There are some creature troubling Rahul. He wants to get rid of as many creature as possible. Coincidentally the creature also don't like each other. So Rahul got an idea and he gathered all the N creature together in a pit. Now all the creature started attacking each other. They all have some health and the health of the ith creature is Hi. A creature dies when its health becomes less than 1. When a creature attacks another creature, the health of creature that is attacked is reduced by an amount that is equal to the health of the attacking creature. Since a single creature will always remain alive in the end, find out the minimum possible health of the last alive creature.

import math
from functools import reduce

def gcd_of_list(healths):
    return reduce(math.gcd, healths)

# Read input
n = int(input())
healths = list(map(int, input().split()))

# Calculate GCD of the list
result = gcd_of_list(healths)

# Print the result
print(result)
