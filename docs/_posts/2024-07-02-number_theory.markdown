---
layout: post
title:  "Elementary Number Theory"
date:   2024-07-02 00:00:00 +0000
categories: lecture notes
katex: True
---

## Natural Numbers

Let us begin with some basic notions of arithmetic (number theory):

* Natural numbers: $$\mathbb{N} = \{0, 1, 2, \ldots \} $$
(Here, $$\mathbb{N}$$ represents the _set_ of natural numbers.)  

Notice that the only reasonable operation to perform on the natural numbers is addition, and consequently multiplication, which is simply repeated addition in our case.

Also, it appears that we just need $$0$$ and $$1$$ in order to express any natural number in terms of addition. As an example, $$4 = ((((0 + 1) + 1) + 1) + 1)$$, meaning perhaps, the symbol $$4$$ is simply a representation of four instances of $$1$$ in additional series. For a deep explanation on this, look into [Peano Axioms](https://en.wikipedia.org/wiki/Peano_axioms).

## Integers

When dealing with the natural numbers, notice that subtraction and division are not always meaningful. As an example, notice that $$1 - 2 = -1$$, which is not a natural number, and $$1 \div 2 = \frac{1}{2}$$, which is also not a natural number. So, we need to be slightly more cautious when dealing with subtraction and division.

So, what are the requirement in order to facilitate subtraction? Let us recall that _subtraction_, in an algebraic sense, is addition by the negative, technically referred to as the additive inverse. So, now we introduce the notion of **integers**:

* Integers: $$\mathbb{Z} = \{\ldots, -2, -1, 0, 1, 2, \ldots\}$$  
(Here, $$\mathbb{Z}$$ represents the set of integers. Z stands for Zahlen, German for numbers).  

Now, the number $$0$$ has a bit more significance than it did with just the natural numbers. Of course, any number added to $$0$$ is simply that number. This was true with the natural numbers as well. However, with the introduction of the negative whole numbers, we also see that whenever a number is paired with its negative in addition, the sum will always be $$0$$. In this sense, we refer to $$0$$ as the _additive identity_, and analogously, we say that $$1$$ is the _multiplicative identity_ as any number multiplied by $$1$$ is simply itself. So, what is up with all the fancy terms here? You will see why when we start discussing division.

## Divisibility

In a similar sense, it appears that the existence of _fractions_ is the requirement to facilitate the operation that we referred to as division. Analogously, in an algebraic sense, division is multiplication by the _multiplicative inverse_, and we refer to the inverse here as the **reciprocal**. 

The notion of fraction and division are closely related - at the end of the day, the quantity in question is part over whole, and computationally, we find such value by performing long-division, e.g. repeated subtraction. 

As far as addition and subtraction are concerned, it appears that for all integers, there exists a negative inverse, namely the _opposites_. For examples, $$1 + (-1) = 0$$, $$(-50) + -(-50) = 0$$, and similarly, $$0 + (-0) = 0$$. So, a natural question to ask is, **does any integer have a reciprocal?**

For the most part, yes, with one critical exception - namely zero. To see why $$0$$ does not have a reciprocal, i.e. the multiplicative inverse, let us consider what we mean by being able to divide in the first place. As a motivating example, we see that $$3$$ divides into $$27$$ because $$3$$ times $$9$$ is $$27$$. We see that $$5$$ divides into $$40$$ because $$5$$ times $$8$$ is $$40$$.  

Similarly, we see that $$2$$ does not divide into $$5$$ because $$2 \times 2 = 4$$ and $$2 \times 3 = 6$$. There are no integers strictly between $$2$$ and $$3$$, and it appears that such figure is precisely the requirement for $$5$$ to be divisible by $$2$$. Let us formalize this intuition.  

We say a number is divisible by the **divisor** (also known as a _factor_) if there exists some integer such that the integer times the divisor is the number. In other words, an integer $$d$$ divides into another integer $$n$$ if there exists an integer $$k$$ such that $$n = dk$$, meaning $$d$$ times $$k$$. **Remember that when variables are written next to each other with no symbols in between, that always means the numbers represented by those variables are being multiplied.**

So, if $$0$$ has a reciprocal, then that means $$0$$ divides into some integer. As a concrete example, let's see if $$0$$ divides $$100$$. In order for $$100$$ to be divisible by $$0$$, it looks like $$0$$ times some integer should be $$100$$. However, $$0$$ times any number is simply $$0$$. Does $$100$$ equal to $$0$$? Only if you get robbed, meaning this was probably a nonsense to begin with, and we claim that $$0$$ does not divide $$100$$.  

As a matter of fact, $$100$$ can be replaced with any nonzero integer, and the same conclusion holds. This implies that $$0$$ does not divide any number and hence **there does NOT exist a reciprocal (the multiplicative inverse) for zero**.

With this notion of divisibility, let us see what kind of integers are divisible and what kind of integers are indivisible. This concept reduces to the existence of the prime numbers and the composite integers.

## Primality

We witnessed how any natural number can be represented by adding $$1$$ __a bunch of times__. In a similar sense, can we represent any negative integer with a repeated addition of $$-1$$. As an example, see that $$-3 = (-1) + (-1) + (-1)$$. So, as the bare minimum, it appears that $$\{-1, 0, 1\}$$ are the _building blocks_ (technically known as the _generators_) for the set of integers in the context of addition. What kind of analogy can we make here in regards to multiplication?  

In other words, can we represent __any integer__ by multiplying a bunch of numbers? If so, what are those numbers called? This brings us to the notion of [the Fundamental Theorem of Arithmetic](https://en.wikipedia.org/wiki/Fundamental_theorem_of_arithmetic), which states that:  

**Any natural number greater than 1 is either a prime, or a product of primes, where such product is uniquely determined by the primes and their exponents.** (Uniqueness here simply means there is only one way and one way only to write such _prime factorization_. As an intuitive example, $$8 = 2 \times 2 \times 2 = 2^3$$, and this is the only way to express $$8$$ as a product of primes. The small $$3$$ in the upper right corner indicates an exponent, which is the number of repeated multiplication with the same number, also known as the __base__: $$2$$ in our case here.)  

This proposition binds nicely with the definition of prime and composite numbers. Hence, let us recall that:  

* Prime: any natural number greater than $$1$$ that is divisible only by $$1$$ and the number itself.  
* Composite: any natural number greater than $$3$$ that is not a prime. 

This implies that $$2$$ is the least natural number that is prime and $$4$$ is the least natural number that is composite. Well, what about $$1$$? Well, first of all, $$1$$ is not greater than 3, so it certainly is not composite. Is it prime then? Unfortunately, [no](https://en.wikipedia.org/wiki/Prime_number#Primality_of_one). Therefore, we say that, by convention, $$1$$ **is neither a prime nor a composite**, and the same argument can be said about $$0$$ as well. 

Furthermore, this argument works for any integer, as any nonnegative integer is simply a natural number and a negative integer is a natural number multiplied by $$-1$$, where the natural numbers have unique prime factorization to begin with.  

## Factors and Multiples

Let us begin with the notion of __multiples__. Let $$n \in \mathbb{Z}$$. We say that the multiples of $$n$$ are of the set $$\{..., -3n, -2n, -n, 0, n, 2n, 3n, ...\} = \{nk : k \in \mathbb{Z}\}$$. For example, in the __times table__ that you are often forced to memorize, you are actually listing the nine positive multiples of the integers from $$2$$ to $$9$$. Let $$a, b \in \mathbb{Z}$$, i.e. $$a$$ and $$b$$ are integers. Formally, we say that $$a$$ is a multiple of $$b$$ if there exists an integer $$k$$ such that $$a = bk$$. See the following examples for better intuition:

* $$10$$ is a multiple of $$10$$ because $$10 = 10 \times 1$$. Clearly, for all integers $$n$$, $$n$$ is a multiple of $$n$$.
* The set of multiples of $$12$$ looks something like $$\{..., -36, -24, -12, 0, 12, 24, 36, 48, 60, ...\}$$. 
* $$51$$ is a multiple of $$3$$ because $$51 = 3 \times 17$$. 
* $$0$$ is a multiple of any integer, because for all integers $$n \in \mathbb{Z}$$, it follows that $$n \times 0 = 0$$.

As you may have noticed, it appears that the notion of divisibility and multiples are closely related. One difference is that $$0$$ does not divide any integer and $$0$$ is a multiple of all integers. Same-same but different.

Notice in the last prime factorization example that we __extracted__ a prime in each level of the prime factorization tree, which resulted in a regular _factor_ that is not necessarily a prime. This brings us to the notion of **factors**, which binds nicely with the notion of divisibility (see above). Let $$a,b \in \mathbb{Z}$$, e.g. $$a$$ and $$b$$ are integers. We say that $$a$$ is a factor of $$b$$ if $$a$$ divides $$b$$, meaning that there exists an integer $$k$$ such that $$b = ak$$. Do you see how $$a$$ and $$b$$ swapped their places in the definitions for a multiple and a factor? Take a look at the following examples for better intuition:

* $$\{1,2,4,8,16,32\}$$ is the set of (positive) factors for $$32$$.

* Since $$31$$ is a prime number, it follows that only $$1$$ and $$32$$ are its factors. 

* Because $$1$$ divides any integer, it follows that $$1$$ is a factor for any integer $$n$$, including itself. 

* Things get quite tricky when $$0$$ is concerned. Since $$0$$ times any integer is $$0$$, we could say that any integer is a factor of $$0$$, meaning $$0$$ has infinitely many factors. Thus, in general, the notion of factors is not very applicable for $$0$$ as we often times ask about finitely many factors. 

## Greatest Common Divisor and Least Common Multiples

Let $$a, b \in \mathbb{N}$$, meaning $$a$$ and $$b$$ are natural numbers (if you don't remember what natural numbers are, scroll to the top!).

Recall that $$a$$ is a divisor (also called a factor) of $$b$$ if there exists an integer $$k$$ such that $$b = ak$$, and $$a$$ is a multiple of $$b$$ if there exists an integer $$m$$ such that $$a = bm$$. Given any two natural numbers $$a$$ and $$b$$, there exists a common divisor, namely $$1$$, and a common multiple, namely $$ab$$, as a bare minimum. The list of common divisors for any two nonzero integers is finite, and the list of common multiples is infinitely long. Hence, we can define two numbers known as the GCD and LCM, Greatest Common Divisor and Least Common Multiple, respectively.

* Greatest Common Divisor of $$a$$ and $$b$$: among all of the common divisors of $$a$$ and $$b$$, the greatest common divisor, suggested by its name, is the greatest one of them all.

* Least Common multiple of $$a$$ and $$b$$: among all of the common multiples of $$a$$ and $$b$$, the least common multiple, suggested by its name, is the smallest one of them all. 

For example, consider the following:

* The divisors of $$24$$ are $$\{1,2,3,4,6,8,12,24\}$$. The divisors of $$60$$ are $$\{1,2,3,4,5,6,10,12,15,20,30,60\}$$. Hence, the common divisors of $$24$$ and $$60$$ are $$\{1,2,3,4,6,12\}$$ and thus it follows that the maximum amongst the common divisors is $$12$$, i.e. $$GCD(24,60) = 12$$.

* The positive multiples of $$7$$ are $$\{7,14,21,28,35,42,...\}$$ and the positive multiples of $$3$$ are $$\{3,6,9,12,15,18,21,24,...\}$$. Hence, the common multiples of $$7$$ and $$3$$ are $$\{21,42,63,...\}$$, thus it follows that the minimum of the common multiples is $$21$$, i.e. $$LCM(7,3) = 21$$. 

Generally, by trial and error and perhaps with good intuition, it is not too difficult to find the greatest common divisor of $$a$$ and $$b$$ if both are relatively small numbers. However, the process might be quite challenging if the given numbers are rather large.

For example, could you figure out the greatest common divisor between $$7587346732894923$$ and $$23243423329932023$$ within a reasonable period of time? If you were to list all the divisors of both numbers and find the common divisors, it might take a while. As a matter of fact, according to Wolfram Alpha, the divisors of $$7587346732894923$$ are $$\{1, 3, 19, 57, 128857, 386571, 2448283,$$
$$7344849, 1033016027, 3099048081, 19627304513, 58881913539, 133111346191139,$$
$$399334038573417, 2529115577631641, 7587346732894923\}$$ and the divisors of $$23243423329932023$$ are $$\{1, 887, 26204535884929, 23243423329932023\}$$. Frustratingly enough, as it turns out, the common divisors of those two numbers is only $$\{1\}$$, hence the greatest common divisor is just $$1$$. Without computational assistance, it would not be a wise use of time to proceed with such lengthy process for a surprisingly trivial answer. Is there a better way to solve the problem of identifying the greatest common divisor?

## The Division Algorithm

The goal of this section is to be able to describe, and hopefully, understand the Euclidean Algorithm, and there are some necessary prerequisites to mention starting with the **division algorithm**.

* Division Algorithm: Let $$a,b \in \mathbb{Z}$$ with $$b \not = 0$$. Then, there exists unique $$q,r \in \mathbb{Z}$$ such that $$a = bq + r$$, where $$0 \leq r < \lvert b \rvert$$. Note that $$\lvert b \rvert$$ represents the absolute value of $$b$$. 

There are two important aspects of the division algorithm:

1. For any integers $$a$$ and nonzero $$b$$, we can always identify the quotient and the remainder of the division of $$a$$ by $$b$$. This is what we mean by the _existence_. 
1. The quotients and the remainders are _unique_, meaning when you divide $$a$$ by $$b$$, you will always find a single number for the quotient and a single number for the remainder. In other words, there will never be a case where you have two different remainders with the same quotient and vice versa.

Examples:

* Suppose that $$a = 123$$ and $$b = 45$$. Then, by the division algorithm, it follows that $$123 = 45(2) + 33$$, where $$2$$ is the quotient and $$33$$ is the remainder. With such remainder between $$0$$ and $$45$$ (including $$0$$ and excluding $$45$$), $$2$$ is the only possible quotient. Similarly, for the quotient value of $$2$$, the only possible remainder is $$33$$.
* What if $$a = 45$$ and $$b = 123$$? Well, $$45 = 123(0) + 0$$, so this is fine as well.
* How about $$a = -123$$ and $$b = -45$$? Well, we can still perform the division algorithm and say that $$-123 = (-45)(3) + 12$$. The remainder of $$12$$ is not intuitive at all, but the statement of division algorithm still valid.
* Now, let $$a = -123$$ and $$b = 45$$. Then, we have $$-123 = 45(-3) + 12$$, so the result is very similar to the previous example. 

In any cases, positive or negative will not make a difference in the validity of the statement except that the divisor, $$b$$ in our case, must not be $$0$$. 

## Optional: Proof of the Division Algorithm

For those who are interested as to why the division algorithm is a valid assertion, I would like to provide you with the proof of the statement for the sake of logic. As indicated above, there are two parts to prove in this assertion: the existence of the quotient and the remainder, and the uniqueness of the quotient and the remainders. This proof will rely on a seemingly trivial mathematical fact known as the **well-ordering principle**: in any nonempty subset of the natural numbers, i.e. $$A \subseteq \mathbb{N}$$ with $$A \not = \{\}$$, then there exists a minimal element for $$A$$. 

* Claim: Let $$a,b \in \mathbb{Z}$$ with $$b \not = 0$$. Then, there exists $$q,r \in \mathbb{Z}$$ such that $$a = bq + r$$, where $$0 \leq r < \lvert b \rvert$$.

  Proof: Let $$S = \{a - bq: q \in \mathbb{Z}\}$$, the multiples of $$b$$ subtracted from $$a$$ where we look at differences that are not negative. Here are three cases to consider:
  
  1. If $$a$$ and $$b$$ are both positive, then either $$a - b(1) \geq 0$$ (for the case that $$a \geq b$$) or $$a - b(-1) \geq 0$$ (for the case that $$a \leq b$$), hence $$a - bq \in S$$ for some integer $$q$$ meaning $$S$$ is not empty. 
  1. Both $$a$$ and $$b$$ are negative.
  1. One of $$a$$ and $$b$$ is positive and the other is negative.
    
   In any case, $$S$$ will not be an empty set, hence by the well-ordering principle stated above, there exists a minimal element (i.e. the smallest number of the set) of $$S$$. Let us call this minimal element $$r$$. As $$r \in S$$, it follows that there exists $$q \in \mathbb{N}$$ such that $$r = a - bq$$, and adding $$bq$$ to both sides of equation yields $$a = bq + r$$. (Need to show that $$r < b$$). 