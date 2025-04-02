---
layout: post
title:  "Chapter 3 Solution Guide"
date:   2025-04-01 00:00:00 +0000
categories: lecture notes
katex: True
---

## Section 3.1: Divisibility
1. With $$12345 = 3(4115)$$ and $$12345 = 5(2469)$$, yes, $$3$$ and $$5$$ both divide $$12345$$ by the definition of divisibility. Make sure you still remember how to do long division.
2. Let $$a = 4, b=6, c=12$$. We see that $$4 \mid 12$$ and $$6 \mid 12$$, but does $$4 \cdot 6 = 24$$ divide $$12$$? What do you think?
3. Suppose that $$a \mid b$$ and $$b \mid c$$. By the definition of divisibility, there exist integers $$m$$ and $$n$$ such that $$am = b$$ and $$bn = c$$. Substitute the first equation into the second equation to obtain $$(am)n = c$$, and by the associative property, it follows that $$(am)n = a(mn)$$, therefore $$a(mn) = c$$. Since $$m$$ and $$n$$ are integers, it follows that $$mn$$ is also an integer, so we found some integer where we can multiply $$a$$ to this number to obtain $$c$$. By the definition of divisibility, we conclude that $$a \mid c$$.
4. $$145 = 7(20) + 5$$. Notice that $$5$$ is the remainder.
5.  - $$45 = 15(3) + 0$$
    - With $$12345 = 15(823)$$, $$15$$ divides $$12345$$ by the definition of divisibility.

## Section 3.2: Prime Factorization

1. $$57$$ is not a prime number, i.e., it is a composite. More specifically, $$57 = 3(19)$$, therefore $$3 \mid 57$$ by the definition of divisibility. Since $$57$$ is greater than $$1$$ and $$1$$ and $$57$$ are not the only integers that divide $$57$$, it follows that $$57$$ is not a prime by the definition of primes.
2. $$420 = 2^2 \cdot 3 \cdot 5 \cdot 7$$. Refer to the prime factor tree below:
    $$
    \begin{array}{c}
        420 \\
        / \quad \ \backslash \\
        2 \quad \ 210 \\
        \quad \quad / \quad \backslash \\
        \quad \quad 2 \quad \ 105 \\
        \quad \quad \quad \quad / \quad \backslash \\
        \quad \quad \quad \quad 3 \quad \ 35 \\
        \quad \quad \quad \quad \quad \quad / \quad \backslash \\
        \quad \quad \quad \quad \quad \quad 5 \quad \ 7 \\
    \end{array}
    $$
3. $$\{2, 3, 5, 7, 11, 13, 17, 19, 23, 29, 31, 37, 41, 43, 47, 53, 59, 61, 67, 71, 73, 79, 83, 89, 97\}$$


## Section 3.3: Common Multiples and Divisors
