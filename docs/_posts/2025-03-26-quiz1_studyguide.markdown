---
layout: post
title:  "Quiz 1 Study Guide"
date:   2025-03-26 00:00:00 +0000
categories: announcement
katex: True
---

On 28 March 2025 (Friday), we will have an in-class quiz. You can expect the quiz to contain five (5) problems, very similar to the following questions.

You are expected to show all work when applicable, and simplify your answers when applicable.

1. Write the mathematical definition of a rational number.
2. Simplify

    $$\frac{\frac{a}{b} + \frac{c}{d}}{\frac{e}{f}}$$
3. Does $$(a + b)^2 = a^2 + b^2$$ for any numbers $$a,b$$? Why or why not? Explain.
4. Find the equation of a line connecting $$(a,b)$$ and $$(c,d)$$.
5. List all the elements of the set $$\{3k: k \in \mathbb{N} \text{ and } k \leq 10\}$$

## Suggested Solution

1. A rational number is a number of the form $$\frac{n}{d}$$ such that:
    - $$n, d \in \mathbb{Z}$$
    - $$d \not = 0$$
    - $$\frac{n}{d}$$ is simplified
2. Let us simplify this expression, one part at a time.
    - $$\frac{a}{b} + \frac{c}{d} = \frac{ad+bc}{bd}$$
    - Division by $$\frac{e}{f}$$ is equivalent to multiplying by $$\frac{f}{e}$$. 
    Therefore,
    $$\frac{ad+bc}{bd} \div \frac{e}{f} = \frac{ad+bc}{bd} \cdot \frac{f}{e} = \frac{f(ad+bc)}{ebd}$$
    (You can distribute $$f$$ in the numerator if you would like.)
3.  In general, $$(a+b)^2 \not = a^2 + b^2$$, but there certainly exist some numbers where you can satisfy the equality. Consider the following:
    - $$(a+b)^2 = (a+b)(a+b) = a^2 + 2ab + b^2$$. You can obtain this result by applying the FOIL technique.
    Now, suppose that $$(a+b)^2 = a^2 + b^2$$. It follows from the earlier result that $$a^2 + 2ab + b^2 = a^2 + b^2$$. Subtract $$a^2$$ and $$b^2$$ from both sides to obtain
    $$2ab = 0$$.
    Divide both sides by $$2$$ and now we have $$ab = 0$$. This means $$a = 0$$ or $$b = 0$$ (remember that __or__ here means the logical operation __or__.)
    In conclusion, $$(a+b)^2 = a^2 + b^2$$ if and only if $$a = 0$$ or $$b = 0$$, meaning **not any** numbers $$a$$ and $$b$$ will satisfy the equality. However, there does exist a set of numbers that will!
    Try to explain to the best of your ability on the quiz.
4.  Here is a summary of the process of finding an equation of a line given two points:
    - Find the slope
    - Pick one of the two given points. Apply the point-slope formula
    - Solve for $$y$$ to obtain the slope-intercept form.
    So, with our points $$(a,b)$$ and $$(c,d)$$, it follows that:
    - Slope: $$m = \frac{d-b}{c-a}$$
    - Point-slope form: Suppose that I choose $$(a,b)$$ as my point. Then, $$y-y_i = m(x-x_i)$$ turns into $$y - b = \frac{d-b}{c-a}(x-a)$$.
    - Finally, solve for $$y$$ by adding $$b$$ to both sides of the equation. It follows that $$y = \frac{d-b}{c-a}(x-a) + b$$, and the slope-intercept form is
    $$y = \frac{d-b}{c-a}x + (-\frac{d-b}{c-a}a + b)$$. Notice that $$a \not = c$$, otherwise the slope is undefined.
    Make sure you can do this with __actual__ numbers, not just with variables.
5.  If $$k$$ is a natural number less than equal to 10, then the following list are the possibilities for $$k: 0,1,2,3,4,5,6,7,8,9,10$$.
    So, $$3k$$ with the possibilities from above gives us the set $$\{3(0),3(1),3(2),3(3),3(4),3(5),3(6),3(7),3(8),3(9),3(10)\} = \{0,3,6,9,12,15,18,21,24,27,30\}$$.