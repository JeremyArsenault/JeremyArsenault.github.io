---
layout: post
title: A Debauch of Derivatives
date: 2023-08-26
---

After sleeping through two years of an undergraduate curriculum in mathematics, I awoke to maths beauty and intrigue during a course in partial differential equations - a semester long treatment of the heat and wave equations. How can one not be awestruck by single, concise, mathematical expression that completely describes a huge class of dynamical systems? So as the torrent of due dates and exams relentlessly approached I impetuously manipulated expressions and chain ruled my way into the dawn...

But I was foolhardy, and ignorance is bliss. Only during my later studies of calculus did I realize the true depth of my confusion - my truancy had caught up with me. I *felt* like I understood the derivative, but what were these objects that I was manipulating? How was $$\frac{\partial f}{\partial t}$$ different from $$\frac{df}{dt}$$? Are they infinitesimal fractions? What does that mean for expressions involving $$dt$$? 

**My goal then is to motivate and define: $$f'$$, $$Df$$, $$\frac{\partial}{\partial x}$$, $$\frac{d}{dt}$$, $$df$$ such in a way that, as a letter to my past self, will answer these questions and address some common misconceptions that may arise.**

# Differentiation on the Reals

Our journey begins with $$f:\mathbb{R}\to \mathbb{R}$$ where you may remember the *limit definition of the derivative*:

$$f^'(t):=\lim_{\delta\to 0} \frac{f(t+\delta)-f(t)}{\delta}$$

Analagously, for a vector valued function $$f:\mathbb{R}^n\to \mathbb{R}$$ we define the *directional derivative*:

$$(D_{v}f)(x^1,...,x^n):=\lim_{\delta\to 0} \frac{f(x^1,...,x^i+\delta,...,x^n)-f(x^1,...,x^n)}{\delta}$$

Intuitively, these . It's important to observe that these standard defionitions

Note that the derivative is only meaningful for *smooth functions*. Smoothness generally refers to the continuity of the derivatives of a function. If $$f^',f^{''},...,f^{(k)}$$ all exist and are continuous, we say $f$ is of class $$C^k$$. In this essay, we assuming the (unnessecarily strict) condition that all functions are of class $$C^\infty$$.

## Chain Rule and Linearity of the Derivative

The chain rule is how we compute the derivative of compositions of functions. It can be understood via the following (imcomplete) proof (when $$g$$ is not constant at $$t$$):

$$(f\circ g)^'(t) = \lim_{\delta\to 0} \frac{f(g(t+\delta))-f(g(t))}{\delta} = \lim_{\delta\to 0} \frac{f(g(t+\delta))-f(g(t))}{g(t+\delta)-g(t)}\cdot \frac{g(t+\delta)-g(t)}{\delta} = f^'(g(t))g^'(t)$$

Perhaps what is most interesting is that shows us linearity of derivative.

A similar procedure shows that

Where $$D_i:=D_{(0,...,1^i,...,0)}$$

Explains the name 


# Differentiation on Manifolds

## (Differentiable) Manifolds

Imagine you want to ...


# Differential Equations

# Equivalence on $$\mathbb{R}$$