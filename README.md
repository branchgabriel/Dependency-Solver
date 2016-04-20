# Dependency-Solver
Kata exercise for sorting dependencies

Senior Level Coding Assignment

{Candidate}, your assignment is to write some code that calculates how dependencies propagate between things such as classes in a program.

In many languages, static dependencies can be determined by source code analysis. Tools such as JDepend that look for explicit dependencies in the source and list them out.

One of the insidious things about dependencies is that they are transitive—if A depends on B and B depends on C, then A also depends on C. 

 Given the following input, we know that A directly depends on B and C, B depends on C and E, and so on.

1
2
3
4
5
6
  A   B   C
  B   C   E
  C   G
  D   A   F
  E   F
  F   H
The program should use this some data like this to calculate the full set of dependencies. In this example, looking at B, we see it directly depends on C and E. C in turn relies on G, E relies on F, and F relies on H. This means that B ultimately relies on C, E, F, G, and H. 

The result below shows a solution from the set of data above.

1
2
3
4
5
6
  A   B C E F G H
  B   C E F G H
  C   G
  D   A B C E F G H
  E   F H
  F   H
You don't necessarily need to use letters you could also use numbers
You can use any language you like. 
Please setup a github account if you don't have one already and create a repo for this exercise. 
Commit often showing your progress as you write tests that prove out the solution. 
Let {staffing professional} know when you can complete the assignment and if you have any questions about the requirements you can email those to {staffing professional or interviewer email}.
