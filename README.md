[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-24ddc0f5d75046c5622901739e7c5dd533143b0c8e959d652212380cedb1ea36.svg)](https://classroom.github.com/a/FgMJElkj)
# Theory vs. Practice

- List 3 reasons why asymptotic analysis may be misleading with respect to
  actual performance in practice.

- Suppose finding a particular element in a binary search tree with 1,000
  elements takes 5 seconds. Given what you know about the asymptotic complexity
  of search in a binary search tree, how long would you guess finding the same
  element in a search tree with 10,000 elements takes? Explain your reasoning.

- You measure the time with 10,000 elements and it takes 100 seconds! List 3
  reasons why this could be the case, given that reasoning with the asymptotic
  complexity suggests a different time.

Add your answers to this markdown file.

**1. Asymptotic analysis disregards constants, which can make considerable differences, especially in cases of small amounts of data sets.**

**2. Whenever 2 algorithms have the same asymptotic complexity, it seems that they would have the same runtime. This is misleading as that is often untrue, depending on many factors, including the distribution of the data sets.**

**3. The actual implementation of the algorithm can substantially impact its performance. Small choices in code as well as the choices of data structures and compiler optimizations.**

