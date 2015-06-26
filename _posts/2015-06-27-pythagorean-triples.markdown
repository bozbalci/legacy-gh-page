---
layout: post
title:  "Pythagorean triples and square roots of complex numbers"
date:   2015-06-27 22:00:00
categories: math
---

Two years ago in math class we were given this problem as exercise:

$$

\text{Find the square roots of the number } 5 + 12i.

$$

We are asked to find numbers $$x + yi$$ which satisfy the following equation:

$$

(x + yi)^2 = 5 + 12i

$$

Expanding the left-hand side of the equation gives:

$$

(x^2 - y^2) + (2xy)i = 5 + 12i

$$

By the equality of the real parts, $$x^2 - y^2 = 5$$; and by the equality of the imaginary parts, $$2xy = 12$$. We note that $$x$$ and $$y$$ must have the same signs (otherwise this product would be negative).

Let's return to the original equation for a moment. Since the Euclidean norm of both complex numbers in the equation must be equal to $$13$$, we can say that $$x^2 + y^2 = 13$$. Putting what we have found together:

$$

x^2 + y^2 = 13 \\
x^2 - y^2 = 5 \\
xy > 0

$$

Summing the two equations will yield $$x^2 = 9$$, and by back-substitution we find $$y^2 = 4$$. We carefully write two solutions in which $$x$$ and $$y$$ have the same sign:

$$

x + yi = 3 + 2i \text{, or } x + yi = -3 - 2i.

$$

This particular method made me realise a connection between complex numbers and Pythagorean triples. Before proceeding to relate with Pythagorean triples, I would like to give a few definitions.

* A **Pythagorean triple** consists of three positive integers $$a$$, $$b$$ anc $$c$$, such that $$a^2 + b^2 = c^2$$.
* We will write such triples as $$(a, b, c)$$. Example: $$(5, 12, 13)$$.
* If $$(a, b, c)$$ is a Pythagorean triple, then so is $$(ka, kb, kc)$$ for any positive integer $$k$$.
* A **primitive Pythagorean triple** is one in which $$a$$, $$b$$ and $$c$$ are coprime.

Recall how we equated the Euclidean norms of the two complex numbers in the first equation in solving the problem. Now we will use the second equation, the expanded form and equate that norm with the other. We have proved the following formula (which can also be proved by elementary algebra):

$$

(x^2 - y^2)^2 + (2xy)^2 = (x^2 + y^2)^2 \tag{1}

$$

We will see that plugging the values we've found in the solution of the problem will yield a nice result. Let's do so. We can either plug $$x = 3$$ and $$y = 2$$ or $$x = -3$$ and $$y = -2$$, I will go with the former:

$$

(3^2 - 2^2) + (2 \cdot 3 \cdot 2)^2 = (3^2 + 2^2) \\
5^2 + 12^2 = 13^2

$$

How pleasant! We know that $$(5, 12, 13)$$ is a primitive Pythagorean triple. We can try this with other Pythagorean triples we know. I tried this with $$3 + 4i$$, which is the square of $$2+i$$, and when we put $$x=2$$ and $$y=1$$ in $$(1)$$ we will arrive at the equation $$3^2 + 4^2 = 5^2$$. In this way, $$a$$, $$b$$ and $$c$$ is found by this formula:

$$

a = x^2 - y^2 \text{, } b = 2xy\text{, }c = x^2 + y^2

$$

and we can plug positive integers $$x$$ and $$y$$ to find Pythagorean triples. Taking the square roots of numbers such as $$3 + 4i$$, $$5 + 12i$$ is essentially breaking down the Pythagorean triple into a tuple when seeded to $$(1)$$ will give us the equation back.

It turns out that I was not the first one discovering this formula. Upon some research I've found that $$(1)$$ is very similar to the better known [Euclid's formula][euclids-formula] and was used to generate Pythagorean triples for thousands of years. It was proved that Euclid's formula could generate every possible primitive Pythagorean triple, and with slight modification to the formula we can generate all Pythagorean triples uniquely:

$$

a = k \cdot (m^2 - n^2) \text{, } b = k \cdot (2mn) \text{, } c = k \cdot (m^2 + n^2)

$$

where $$m$$, $$n$$, and $$k$$ are positive integers with $$m > n$$, $$m - n$$ odd, and with $$m$$ and $$n$$ coprime. A proof of Euclid's formula is given at the Wikipedia link above.

Further investigation of this relation reveals a glimpse of a very important mathematical law: the law of [quadratic reciprocity][quadratic-reciprocity]. The earliest result of quadratic reciprocity was that a prime can be written as $$p = x^2 + y^2$$ if and only if $$p \equiv 1 \pmod{4}$$. The [proof][fermat-primes] was broken up into two parts: The Descent Step which states that if $$p$$ is a divisor of the number $$a^2 + b^2$$, then $$p$$ can be written as $$x^2 + y^2$$. And then the Reciprocity Step which says that if $$p \equiv 1 \pmod{4}$$, then it divides a number in the form $$a^2+b^2$$.

What we have done in the solution of the problem above is an example of the Descent Step. To see this, notice that $$13$$ divides $$13^2 = 5^2 + 12^2$$. The Descent Step says that we should be able to write $$13$$ as the sum of two squares, and if we look at the numbers we've found in the solution of the question above, we'll see that $$13=2^2+3^2$$.

Complex numbers enter the discussion once we see that a number can be written as $$n = x^2 + y^2$$ if and only if it can be written as $$n = (x + yi)(x - yi)$$ (the right-hand side of both equations are equal). It factors nicely, when we allow $$i$$ to be used. So, quadratic reciprocity says that a prime will factor after allowing $$i$$ if and only if the prime $$p \equiv 1 \pmod{4}$$.

So how does this give us Pythagorean Triples? If I let $$x$$ and $$y$$ be any integers, then

$$

n = x^2 + y^2 = (x+yi)(x-yi)

$$

is an integer (and a product of two [Gaussian integers][gaussian-integers], at that!) If we square both sides of the equation,

$$

n^2 = (x+yi)^2 \cdot (x-yi)^2 = \big( (x^2 - y^2) + 2xyi \big) \cdot \big( (x^2 - y^2) - 2xyi \big)

$$

and this means that we have a Pythagorean triple: $$n^2 = a^2 + b^2 = (a+bi)(a-bi)$$ where $$a = x^2 - y^2$$ and $$b=2xy$$, this is exactly the generating formula for Pythagorean triples. Now, if I have a Pythagorean triple, $$a^2 + b^2 = c^2$$ then this means I can write $$c^2=(a+bi)(a-bi)$$. The Descent Step tells me that I can then find the square root of $$a+bi$$. It says that $$c$$ itself can be written like $$c=(x+iy)(x-iy)$$ and by the formula we've found in this text we must have $$a+bi=(x+yi)^2$$ which gives us the formula for $$x$$ and $$y$$ in terms of $$a$$ and $$b$$, just like we've found while rediscovering Euclid's formula.

A few final notes:

* This will only work if we start with a Pythagorean triple. If we don't, we will get complex numbers with irrational coefficients.

* This will work in more general cases. If $$a^2 + nb^2 = c^2$$, then the Descent Step still holds (but not the Reciprocity Step) and we can write $$c=x^2+ny^2$$ and we will have the following equality:

$$

c = (x + \sqrt{-n}y)(x - \sqrt{-n}y)

$$

with $$a + \sqrt{-n}b = (x + \sqrt{n}y)^2$$ and so $$a = x^2 - ny^2$$ and $$b=2xy$$. Let's call this an **n-Pythagorean triple**. An example would be with $$x=2$$, $$y=1$$ and $$n=3$$:

$$

7 = 2^2 + 3(1^2) = (2 + \sqrt{-3})(2 - \sqrt{3}).

$$

Squaring,

$$

49 = (2^2 - 3(1^2))^2 + 3(2 \cdot 2 \cdot 1)^2 = 1 + 3 \cdot 16 = 49

$$

and so $$49 = 1^2 + 3(4^2)$$ is a 3-Pythagorean triple. So the square root of $$(1+4\sqrt{-3})$$ is $$(2 + \sqrt{-3})$$, and we got this result via Pythagorean triple methods. Neat!

If you would like to read more about this topic, I would suggest you to read on [algebraic number theory][algebraic-number-theory] and especially the subfield "Class Field Theory" which uses extensions of numbers (like the way we allow $$i$$ in our calculations) to figure properties of numbers. Also I've been suggested [Primes of the form $$x^2 + ny^2$$][primes-of-the-form] by Brian Cox, which starts with questions very similar to we investigated in this text and end with completely answering this very question (the relation between Pythagorean triples and complex multiplication) after going through three hundred years of mathematical development.

Happy math!

[euclids-formula]: https://en.wikipedia.org/wiki/Pythagorean_triple#Generating_a_triple
[quadratic-reciprocity]: https://en.wikipedia.org/wiki/Quadratic_reciprocity
[fermat-primes]: http://math.ucsd.edu/~abucur/oldcourses/2013/104a/fermatprimes.pdf
[gaussian-integers]: https://en.wikipedia.org/wiki/Gaussian_integer
[algebraic-number-theory]: https://en.wikipedia.org/wiki/Algebraic_number_theory
[primes-of-the-form]: http://www.amazon.com/Primes-Form-ny2-Multiplication-Mathematics/dp/1118390180/ref=sr_1_1?ie=UTF8&qid=1390926725&sr=8-1&keywords=primes+of+the+form
