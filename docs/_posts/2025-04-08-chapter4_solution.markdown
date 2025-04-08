---
layout: post
title:  "Chapter 4 Solution Guide"
date:   2025-04-08 00:00:00 +0000
categories: lecture notes
katex: True
---

## 4.1: Absolute Values

1.  By the definition of absolute values, we have that

    $$
    |2x+5| = 
    \begin{cases}
        2x+5 & \text{if } 2x+5 \geq 0 \\
        -(2x+5) & \text{if } 2x+5 < 0
    \end{cases}
    $$

    (Notice that I just replaced $$x$$ with $$2x+5$$ in the original definition)

    There are two cases to consider:
    *   Suppose that $$2x+5 \geq 0$$. Then, $$|2x+5| = 2x+5 = 9$$. Solving for $$x$$ here yields $$x = 2$$.
    *   Suppose that $$2x+5 < 0$$. Then, $$|2x+5| = -(2x+5) = -2x-5 = 9$$. Solving for $$x$$ here yields $$x = -7$$.
    
    Therefore, the solutions are $$x = 2$$ and $$x = -7$$. 

2.  In a similar sense, we get the following from the definition of absolute values:

    $$
    |x^2 - 4| = 
    \begin{cases}
        x^2 - 4 & \text{if } x^2 - 4 \geq 0 \\
        -(x^2 - 4) & \text{if } x^2 - 4 < 0
    \end{cases}
    $$

    So, let us consider the two cases again:
    *   Suppose that $$x^2 - 4 \geq 0$$. Then, $$|x^2 - 4| = x^2 - 4 = 1$$. Solving for $$x$$ here yields $$x = \pm \sqrt{5}$$.
    *   Suppose that $$x^2 - 4 < 0$$. Then, $$|x^2 - 4| = -(x^2 - 4) = -x^2 + 4 = 1$$. Solving for $$x$$ here yields $$x = \pm \sqrt{3}$$.
    
    Therefore, the solutions are $$x = \pm \sqrt{3}$$ and $$x = \pm \sqrt{5}$$.

3.  Here, we can apply the same techniques from the earlier two problems, but let us take another approach here by applying the proposition from the text on page 73. 
    
    Suppose that $$|3x+2| \leq 5$$. By the proposition, it follows that

    $$-5 \leq 3x+2 \leq 5$$

    (You will also end up with this if you apply the same technique from the earlier problems - here, we just have one long inequality instead of the two cases we considered).
    Let us solve the inequalities, one pair at a time.

    *   Solving $$-5 \leq 3x + 2$$ yields $$-\frac{7}{3} \leq x$$. 
    *   Solving $$3x + 2 \leq 5$$ yields $$x \leq 1$$. 

    Therefore, we have that $$-\frac{7}{3} \leq x$$ and $$x \leq 1$$, meaning $$\frac{7}{3} \leq x \leq 1$$ if we combine the inequalities together.

4.  Once again, by the definition of absolute values, we end up with two cases.
    *   Suppose that $$4 - x \geq 0$$. Then, $$|4 - x| = 4 - x > 4$$, and the solution here is $$0 > x$$. 
    *   Suppose that $$4 - x < 0$$. Then, $$|4 - x| = -(4 - x) = -4 + x > 4$$, and it follows that $$x > 8$$.

    Therefore, it appears that the solution here is $$x < 0$$ or $$x > 8$$. Notice the usage of the word __or__ here, because you cannot have a number $$x$$ that is both negative and greater than 8!

5.  

## 4.2: Radical Expressions

## 4.3: Quadratic Equations