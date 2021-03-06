# Dynamic Programming

## Dynamic Programming

### General

Dynamic Programming is a method for solving complex problems, that require solutions of the same sub-problems. It does this by breaking down the initial problem in sub-problem and then tries to find a solution for these sub-problems. Once it found this, it will store these solutions for re-use later.

We can think of it as a "carefully chosen brute force" which will try all the possibilities, but avoid having an exponential amount by limiting them.

**Core ideas**

* Guessing \(Try all the different choices and take the best one\)
* Recursion \(Express the solution of a problem in terms of subproblems\)
* Memoization \(Once we found an answer, store in a lookup table = write on memo pad, and re-use later\)

> Dynamic programming will basically express a problem as a Dynamic Acyclic graph \(DAG\) and find the shortest path in it

We can find the runtime for a dynamic programming problem by using the following formula:

$$runtime = \#subproblems * time/subproblem (treat~a~recursive~call~as~Θ(1))$$

### Steps to find a solution

We can break down every dynamic programming problem in a few steps which will help us to find a problem: 1. Define the subproblems and count them \(\#subproblems\) 2. Guess \(part of the solution\), it is possible that there are no guesses. \(\#choices\)

* _Example \#1:_ In a knapsack problem we can choose between picking the item, or leaving it
* _Example \#2:_ In Fibonacci there are no choices so = 1
  1. Relate subproblem solutions \(gets the time/subproblem\)
  2. Build an algorithm using one of the two techniques described. \(make sure that subproblem is acyclic, so that we can use topological order\)
* **Recurse & Memoize \(Top-Down method\):** break down the given problem and solve + save it if it has not been solved yet. Return the saved answer
* **Build a DP table \(Bottom-up method\):** Analyze the problem, find order in which sub-problems are solved and start solving from the trivial sub-problem. Up towards the given problem.
  1. Solve the original problem

> A quick tip on learning Dynamic Programming, is to think about the problems in a top-down fashion instead of bottom-up. We will however still program the problems in a bottom-up fashion, since it makes it easier to find the time and space complexity and results in a shorter source code.

## Reference

[https://www.youtube.com/watch?v=OQ5jsbhAv\_M](https://www.youtube.com/watch?v=OQ5jsbhAv_M)  
 [https://www.youtube.com/watch?v=ENyox7kNKeY](https://www.youtube.com/watch?v=ENyox7kNKeY)  
 [https://www.youtube.com/watch?v=ocZMDMZwhCY](https://www.youtube.com/watch?v=ocZMDMZwhCY)  
 [https://www.youtube.com/watch?v=tp4\_UXaVyx8](https://www.youtube.com/watch?v=tp4_UXaVyx8)  
 [http://www.es.ele.tue.nl/education/5MC10/Solutions/knapsack.pdf](http://www.es.ele.tue.nl/education/5MC10/Solutions/knapsack.pdf)  
 [http://www.geeksforgeeks.org/dynamic-programming-set-1/](http://www.geeksforgeeks.org/dynamic-programming-set-1/)  
 [https://www.quora.com/Are-there-any-good-resources-or-tutorials-for-dynamic-programming-besides-the-TopCoder-tutorial](https://www.quora.com/Are-there-any-good-resources-or-tutorials-for-dynamic-programming-besides-the-TopCoder-tutorial)

