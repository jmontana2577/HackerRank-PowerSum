# HackerRank-PowerSum
My solution(s) to the HackerRank problem called <a href="https://www.hackerrank.com/challenges/the-power-sum">Power Sum</a>. It's in the <i>Algorithms</i> track in the <i>Recursion</i> section.

Currently, this repo contains just one solution, but I'll be exploring others.

## Recursion with Subtraction
Here's the approach:  
  - Define a function that will loop through the possible natural numbers as bases for the given number and power (i.e. if 50 is the number and 2 is the power, loop through 1-7 because 7 is the largest natural number that when raised to the power of 2 is less than or equal to 50).
  - Raise the base to the specified power, and subtract that from the given number. 
  - Call the function again for the result of the subtraction, but increment the base by 1 to see how many ways that can happen.
  - After these recursive subtractions, if the number gets to 0, then that combination can is possible and the count gets incremented by 1. 
  - The recursion stops when the base raised to the power gets bigger than the current number being passed to the function.
