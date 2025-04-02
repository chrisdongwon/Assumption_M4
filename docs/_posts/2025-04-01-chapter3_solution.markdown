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
2. The prime factorization of $$420$$ is: $$420 = 2^2 \cdot 3 \cdot 5 \cdot 7$$. Refer to the prime factor tree for the specific breakdown:
    
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
4.  - $$2 \cdot 3 \cdot 5 \cdot 7 + 1 = 211$$
    - Notice that $$2, 3, 5, 7$$ all do __not__ divide $$211$$ (they will all have remainder 1). So, we just found a number that is only divisible by $$1$$ and itself, meaning $$211$$ must be a prime according to our definition. **While this looks like a promising strategy, we are not guaranteed to generate prime numbers in this way! This simply shows a logical contradiction when assuming that there are finitely many prime numbers.** The formalized argument of this strategy is called Euclid's proof of the [infinitude of primes](https://en.wikipedia.org/wiki/Euclid%27s_theorem).
5.  - Let $$p_i, q_j$$ represent primes, where $$i$$ and $$j$$ represent the $$i^{th}$$ (or $$j^{th}$$) prime number, where repeating primes are allowed. Suppose that $$a$$ has $$m$$ primes in its prime factorization, and $$b$$ has $$n$$ primes in its prime factorization:

    $$a = p_1 p_2 \cdots p_m$$

    $$b = q_1 q_2 \cdots q_n$$

    Suppose that $$\sqrt{2} = \frac{a}{b}$$. It follows that:

    $$ \sqrt{2} = \frac{p_1 p_2 \cdots p_n}{q_1 q_2 \cdots q_m}$$

    If there are any common primes between $$a$$ and $$b$$ in the prime factorization, then they can be __cut__ from the fraction. Since our definition of rational numbers require that $$\frac{a}{b}$$ is simplified, it follows that for all $$1 \leq i \leq m$$ and $$1 \leq j \leq m$$, we have that $$p_i \not = q_j$$. 

    - From above, we see that $$a$$ has $$m$$ primes and $$b$$ has $$n$$ primes in the factorization. Then, $$a^2 = p_1^2 p_2^2 \cdots p_n^2$$ and $$b^2 = q_1^2 q_2^2 \cdots q_m^2$$, meaning $$a^2$$ has $$2m$$ prime factors and $$b^2$$ has $$2m$$ prime factors, and it follows that they both have an **even** number of primes in the factorization. Solving for $$a^2$$ yields:
    
    $$a^2 = 2b^2$$
    
    However, on the right side of the equality, $$2b^2$$ also includes another prime factor $$2$$. Therefore, $$a^2$$ has an even number of prime factors, but $$2b^2$$ has an odd number of prime factors, since an even number plus one is always an odd integer.
    - By the fundamental theorem of arithmetic, prime factorizations are **unique**. This means there is one and only one way to write the prime factorization. It follows that it is not possible for a number to have an even number of prime factors **and** and an odd number of prime factors - it must be one or the other! This is a logical contradiction, and it means that $$\sqrt{2}$$ can never be a rational number.

## Section 3.3: Common Multiples and Divisors
