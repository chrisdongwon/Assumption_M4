---
layout: post
title:  "Chapter 1 Solution Guide"
date:   2025-03-21 00:00:00 +0000
categories: lecture notes
katex: True
---

## Section 1.1: The Rational Numbers

1. Definition of **rational numbers**:

    A number of the form $$\frac{n}{d}$$ where the following conditions **must** be satisfied:
    - $$n$$ and $$d$$ are integers
    - The denominator is not zero. Symbolically, $$d \not = 0$$
    - $$\frac{n}{d}$$ is simplified. More specifically, we say that $$n$$ and $$d$$ have no factors in common (more on this in Chapter 3). 

2. $$2.4$$ is not an integer and $$1.2$$ is not an integer. Therefore, the condition that the numerator and the denominator must be integers is not satisfied, meaning $$\frac{2.4}{1.2}$$ is not a rational number by the definition. 

3. $$\frac{2}{4}$$ is not simplified - but it *can* be simplified to $$\frac{1}{2}$$. Therefore, $$\frac{1}{2}$$ is not a rational number by the definition. 

4. $$\frac{0}{0} = 1$$ if we simply follow the convention that the same numbers at the top and at the bottom yields $$1$$. In a similar sense, $$\frac{0}{0} = 0$$ if we only look at the numerator and see that it is $$0$$. Therefore, $$\frac{0}{0} = 1$$ and $$\frac{0}{0} = 0$$, but **no number is both 0 and 1**. $$\frac{0}{0}$$ is undefined for this reason. 

5.
- If we follow the formula in the text, we get:

$$\frac{2}{3} + \frac{5}{7} = \frac{2 \cdot 7 + 3 \cdot 5}{3 \cdot 7} = \frac{29}{21}$$

- We do not always have to follow the formula *if you can identify a common denominator*. In this case, the common denominator is:

$$18 \cdot 4 = 24 \cdot 3 = 72$$

Therefore,

$$\frac{11}{18} - \frac{13}{24} = \frac{4}{4} \cdot \frac{11}{18} - \frac{13}{24} \cdot \frac{3}{3} = \frac{44 - 39}{72} = \frac{5}{72}$$

- When we multiply fractions, we multiply *straight across*.

$$\frac{ab}{cd} \cdot \frac{c}{b} = \frac{abc}{cdb} = \frac{a}{d}$$

Notice that $$b, c, d \not = 0$$ since the denominator cannot be $$0$$.

- This is simply a fraction division problem.

$$\frac{a+b}{c+d} \div \frac{e-f}{g-h} = \frac{a+b}{c+d} \cdot \frac{g-h}{e-f} = \frac{(a+b)(g-h)}{(c+d)(e-f)}$$

Once again, notice that the denominators cannot be 0. Since $$c+d, e-f, g-h$$ all appear in the denominators of any present fractions, they also cannot be $$0$$. 

## Section 1.2: The Field Axioms

1. Consider the algebraic expression $$ax^2 + bx + c$$. We say that $$x$$ is the variable with exponents $$2$$ for $$x^2$$ and $$1$$ for $$x^1 = x$$. The coefficients are $$a$$ and $$b$$, and the constant term is $$c$$.

2. Notice that

    $$(1+2)^2 = 3^2 = 9$$

    and

    $$1^2 + 2^2 = 1 + 4 = 5$$

    Once again, you **DO NOT** distribute the exponent, because you have to apply the addition in the parentheses first before you apply the exponent, not the other way around. 

3. With $$(a+b)^2 = (a+b)(a+b)$$, it follows that

    $$(a+b)(a+b) = a^2 + ab + ba + b^2 = a^2 + 2ab + b^2$$

4. By the distributive property, it follows that

    $$(a+b)(c+d) = (a+b)c + (a+b)d$$

    By two applications of the distributive property, it follows that

    $$(a+b)c + (a+b)d = (ac + bc) + (ad + bd)$$

    By the associative property, it follows that

    $$(ac + bc) + (ad + bd) = ac + (bc + ad) + bd$$

    Finally, by the commutative property, we have that

    $$ac + (bc + ad) + bd = ac + (ad + bc) + bd$$

5. By the distributive property, it follows that

    $$x^2 + (b+d)x + bd = x^2 + (bx + dx) + bd$$

    By the associative property, it follows that

    $$x^2 + (bx + dx) + bd = (x^2 + bx) + (dx + bd)$$

    By the commutative property, it follows that

    $$(x^2 + bx) + (dx + bd) = (x^2 + bx) + (xd + bd)$$

    By two applications of the distributive property, it follows that

    $$(x^2 + bx) + (xd + bd) = (x + b)x + (x + b)d$$

    By the distributive property, we finally have that

    $$(x + b)x + (x + b)d = (x + b)(x + d)$$

## Section 1.3: Linear Equations

1. If we follow the order of operations (PEMDAS), it looks like the following operations are being applied to $$x$$ in the provided order:
    - Square $$x$$
    - Multiply 7
    - Subtract 9
    To solve for $$x$$, we consider the inverse operations in the reverse order:
    - Add 9
    - Divide 7
    - Square root
    Therefore, it follows that $$x = \pm \sqrt{\frac{11}{7}}. Notice that there are two solutions: the positive one and the **negative** one.

2. Take a look at page 20 towards the bottom of the page: the process of converting $$ax + by = c$$ to the slope-intercept form ($$y = mx + b$$) is explained there. Notice that $$a = 5, b = 7, c = 11$$ with our given problem. 

3. $$y=1$$ is a horizontal line, so two possible points are $$(0,1)$$ and $$(1,1)$$ (of course, as a line is a set of ordered pairs, there are infinitely many choices). In a similar sense, $$x = 2$$ is a vertical line, and two possible points are $$(2,0)$$ and $$(2,1)$$. If you calculate the slope, you should get $$m = 0$$ for a horizontal line and an undefined $$m$$ value for the vertical line with a $$0$$ in the denominator.

4. I recommend that you use graphing calculators such as [desmos](https://www.desmos.com/calculator) to have a precise look at the graph. However, it is still important that you are able to do this without any digital assistance, so consider the following:
    - $$y = -\frac{3}{4}x + 2$$ is in slope-intercept form. This means the slope of the line is $$-\frac{3}{4}$$ and the y-intercept is $$2$$.
    - Start by drawing an $$xy$$ grid, and place a point at $$(0,2)$$, which is the y-intercept. Remember that ordered pairs are in the form $$(x,y)$$, meaning that the first number are along the $$x$$ axis and the second number is along the $$y$$ axis.
    - Slope $$-\frac{3}{4}$$ can be interpreted as: go down by $$3$$ units, and the to right by $$4$$ units. If you start with the point $$(0,2)$$ and go down by $$3$$ units, you end up at $$(0,-1)$$. From $$(0,-1)$$, if you go to the right by $$4$$ units, then you end up at $$(4,-1)$$.
    - Connect $$(0,2)$$ and $$(4,-1)$$ and there you go, that is the graph of the linear equation $$y = -\frac{3}{4}x + 2$$.

5. There's a lot of computation here, and it is important that you try this out on your own. Here is a [video](https://www.youtube.com/watch?v=lzqTD0JWwhY) guide that I would recommend you to watch and follow, if you find the written explanation in the text to be overwhelming. 