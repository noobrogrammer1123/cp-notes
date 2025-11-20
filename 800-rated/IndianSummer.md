## Problem Name: Indian Summer
## Link: https://codeforces.com/contest/44/problem/A

## Core Idea
- Store pairs in an array to check if each pair is unique.

## My Approach
- Used two separate arrays of strings.  
- For each new input, compared both strings with all previously entered strings.  

## Common Mistakes / Pitfalls
- Incremented the answer inside the loop, causing double-counting because the check hadn’t completed for all previous pairs.  
  *Fix:* use a boolean flag to determine uniqueness, then increment after checking all previous pairs.  
- Took input inside the checking loop, which is tricky.  
  *Fix:* read all inputs first into an array.

## Reflection / What my initial thought process should have been
- Read all pairs into an array before processing.  
- Use an array of pairs to represent the inputs.  
- Use two loops:  
  1. Outer loop to pick the current pair.  
  2. Inner loop to compare with all previously stored pairs.  
- This approach avoids double-counting and keeps logic clean.
