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

**We know that the time complexity of searching in a binary search tree is O(logn), and thus we can expect a logarithmic increase in the time it takes to find an element as the value of n is increased. We know that the search when n = 1,000 (we can say T(1,000) was 5 seconds. Let's formulate an equation using the values we have thus far.**

**T(10,000)/T(1,000) = log(10,000)/log(1,000)**

**We can then plug in 5 seconds for T(1,000) to get T(10,000)/5 = log(10,000)/log(1,000)**

**When we multiply both sides by 5, we get T(10,000) = 5 * ((log(10,000)/log(1,000))**

**We can simplify this to T(10,000) = 5 * (4/3) which comes out to T(10,000) ≈ 6.67 seconds. So we can conclude that it would take about 6.67 seconds to find the same element in a search tree with 10,000 elements.**

**Hmm... that should not be possible. Even if the new data set is worst case, the time should not be 100 seconds. Unless the fault is some unique external circumstance, then it is not possible that the 10,000 element search would take 20 times longer than 1,000 element search.**
