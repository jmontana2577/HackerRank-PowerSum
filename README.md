# HackerRank-PowerSum
My solution(s) to the HackerRank problem called <a href="https://www.hackerrank.com/challenges/the-power-sum">Power Sum</a>. It's in the <i>Algorithms</i> track in the <i>Recursion</i> section.

Currently, this repo contains just one solution, but I'll be exploring others.

## Recursion with Subtraction
Here's the approach:  
  - Define a function that will loop through the possible natural numbers as bases for the given number and power (i.e. if 50 is the number and 2 is the power, loop through 1-7 because 7 is the largest natural number that when raised to the power of 2 is less than or equal to 50).
  - Raise the base to the specified power, and subtract that from the given number. 
  - Call the function again for the result of the subtraction, but increment the base by 1 to see how many ways that can happen.
  - The recursion stops in two instances:
    - The result of the subtraction equals 0, which means that a possible combination has been identified and the count gets incremented by 1.
    - The result of the base raised to the power is greater than the current number being passed to the function, so there's no need to look for combinations starting with that base.