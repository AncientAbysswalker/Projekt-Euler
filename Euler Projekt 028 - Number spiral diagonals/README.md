# Number spiral diagonals

## Problem Statement

Starting with the number 1 and moving to the right in a clockwise direction a 5 by 5 spiral is formed as follows:

21 22 23 24 25
20  7  8  9 10
19  6  1  2 11
18  5  4  3 12
17 16 15 14 13

It can be verified that the sum of the numbers on the diagonals is 101.

What is the sum of the numbers on the diagonals in a 1001 by 1001 spiral formed in the same way?

## Solution
When I saw this problem, I looked at it for a little bit. The problem very quickly looked to have special symmetry of some kind... A discernable pattern. It is easiest seen in the upper right diagonal where the numbers are the squares of 1,3,5. This got me thinking of quadratics, and considering the pattern of this problem I had fair confidence that the numbers along radial paths would have quadratic formulae that apoply to them.

<>

Quadratic formulae can be solved, as seen above, from three points on the curve - which the problem has been kind enough to give us. If we generate matrix A for each diagonal and reduced-row-echelon them we do indeed get four distinct and clear quadratic formulae.

<>

Testing these on the fourth spiral confirms they are correct.

<>

After this it was a simple matter of summing over the concentric spirals, being careful not to count 1 four times.

<>