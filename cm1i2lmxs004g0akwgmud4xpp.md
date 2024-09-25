---
title: "Complexities in DSA"
seoTitle: "Complexities in Data Structures and Algorithms"
datePublished: Wed Sep 25 2024 16:19:12 GMT+0000 (Coordinated Universal Time)
cuid: cm1i2lmxs004g0akwgmud4xpp
slug: complexities-in-dsa
cover: https://cdn.hashnode.com/res/hashnode/image/upload/v1727279023019/f2abef85-114b-40de-9c57-f4eb73a1f4d9.png
ogImage: https://cdn.hashnode.com/res/hashnode/image/upload/v1727281105084/a9bb8832-adcf-4ee5-a67d-71eb8377a3fa.png
tags: algorithms, computer-science, data-structures, complexity, time-complexity, dsa, space-complexity

---

## What are Complexities

One of the main reasons for Data Structures and Algorithms (DSA), is to solve problems effectively and efficiently. To determine the **efficiency** of a program, we look at two types of complexities:

1. **Time Complexity**: This tells us how much time our code takes to run.
    
2. **Space Complexity**: This tells us how much memory our code uses.
    

## Types of Complexities

1. Constant (1)
    
2. Logarithmic (log n)
    
3. Linear (n)
    
4. Quadratic (n²)
    
5. Factorial (n!)
    
6. Exponential (c^n)
    

## Asymptotic Notation

To compare efficiencies of algorithms, we use what we call asymptotic notation, a mathematical tool that estimates **time** based on **input size** without running the code. It focuses on the number of basic operations in the program.

> As stated above, the time is based on input size and not on the actual time it takes to process the information. This is because using the actual time won’t be fair, as different users have different hardware, different applications running or even different programming languages: which will definitely affect the speed of the operation.

There are multiple Asymptotic Notations which include (but not limited to):

1. Big-O (O)
    
2. Omega ([**Ω**](https://www.geeksforgeeks.org/analysis-of-algorithms-big-omega-notation/)**)**
    
3. Theta (θ)
    
4. Little-o
    
5. Little-omega
    

For this article, we are only going to be looking at the three major ones which are:

* Big-O
    
* Omega
    
* Theta
    

### Worst Case - Big-O notation

The most commonly used notation for code analysis is Big O Notation, providing an **upper limit** or **upper bound** on the running time or memory usage concerning the input size.

You may ask, why start with the worst case scenario? Well that is because, when designing systems, you will want to go with a solution where even at the worst possible case, it still performs well.

Mathematically, the Big-O notation is expressed as:

> *O (g(n)) = {f(n): there exist positive constants c and n<sub>0</sub> such that f(n) ≤ c\*g(n) for all n ≥ n<sub>0</sub>}.*

This means that

> *f(n) = O(g(n)), If there are positive constants n<sub>0</sub> and c such that, to the right of n<sub>0</sub> the f(n) always lies on or below c\*g(n).*

By using **big O- notation**, we can asymptotically limit the **expansion** of a running time to a range of constant factors above and below. It is a model for quantifying **algorithm performance.**

### Best Case - Omega

**Omega notation** represents the lower bound of the runtime of an algorithm. It gives the **best-case** complexity of an algorithm.

It is defined as the condition that allows an algorithm to complete statement execution in the **shortest amount of time.**

Mathematically, this is represented as:

> *Ω (g(n)) = {f(n): there exist positive constants c and n<sub>0</sub> such that 0 ≤ c\*g(n) ≤ f(n) for all n ≥ n<sub>0</sub>}.*

This means that,

> This means that, f(n) = Ω(g(n)), If there are positive constants n<sub>0</sub> and c such that, to the right of n<sub>0</sub> the f(n) always lies on or above c\*g(n).

### Average Case - Theta Notation

Mathematically, it is represented as

> ***Θ (g(n))*** *\=* ***{f(n):*** *there exist positive constants c<sub>1</sub>, c<sub>2</sub> and n<sub>0</sub> such that* ***0 ≤ c<sub>1 </sub> g(n) ≤ f(n) ≤ c<sub>2 </sub> g(n)*** *for all n ≥ n<sub>0</sub>}*

This means,

> f(n) = Θ(g(n)), If there are positive constants n<sub>0</sub> and c such that, to the right of n<sub>0</sub> the f(n) always lies on or above c<sub>1</sub>\*g(n) and below c<sub>2</sub>\*g(n).

## Steps To Calculate Complexity

1. Find the fastest growing term in the function
    
2. If the fastest growing term has a coefficient, remove it.
    

As time goes on and as we look at different data structures and algorithms, we will analyze the complexities of the different operations that can be done on these data structures and the time complexities of different algorithms as well.

For a more comprehensive guide to complexities, you can check out this article on GFG. [https://www.geeksforgeeks.org/complete-guide-on-complexity-analysis/](https://www.geeksforgeeks.org/complete-guide-on-complexity-analysis/)