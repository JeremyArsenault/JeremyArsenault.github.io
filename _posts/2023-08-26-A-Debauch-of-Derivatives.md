---
layout: post
title: A Debauch of Derivatives
date: 2023-08-26
---

# UNDER CONSTRUCTION

After sleeping through two years of an undergraduate curriculum in mathematics, I awoke to maths beauty and intrigue during a course in partial differential equations - a semester long treatment of the heat and wave equations. How can one not be awestruck by single, concise, mathematical expression that completely describes a huge class of dynamical systems? So as the torrent of due dates and exams relentlessly approached I impetuously manipulated expressions and chain ruled my way into the dawn...

But I was foolhardy, and ignorance is bliss. Only during my later studies of calculus did I realize the true depth of my confusion - my truancy had caught up with me. I *felt* like I understood the derivative, but what were these objects that I was manipulating? How was $$\frac{\partial f}{\partial t}$$ different from $$\frac{df}{dt}$$? Are they infinitesimal fractions? What does that mean for expressions involving $$dt$$? 

**My goal then is to motivate and define: $$f'$$, $$Df$$, $$\frac{\partial}{\partial x}$$, $$\frac{d}{dt}$$, $$df$$ such in a way that, as a letter to my past self, will answer these questions and address some common misconceptions that may arise.**

***********************

## Differentiation on the Reals

Our journey begins with $$f:\mathbb{R}\to \mathbb{R}$$ where you may remember the *limit definition of the derivative*

$$f'(t):=\lim_{\delta\to 0} \frac{f(t+\delta)-f(t)}{\delta}$$

We generalize this idea to vector valued functions $$f:\mathbb{R}^n\to \mathbb{R}^m$$ by defining define the $$i$$th component of the *directional derivative* of $$f$$ in the direction $$v\in\mathbb{R}^n$$ as

$$(D_vf^i)(x):=\lim_{\delta\to 0} \frac{f^i(x^1+\delta v^1,...,x^n+\delta v^n)-f^i(x^1,...,x^n)}{\delta}$$

Using this notation, $$f'=D_1f$$.

These derivative formulas tell you how the output of $f$ changes respect to its input at every point on the domain.

Note that the derivative is only meaningful for *smooth functions*. Smoothness generally refers to the continuity of the derivatives of a function. If $$f',f'',...,f^{(k)}$$ all exist and are continuous, we say $$f$$ is of class $$C^k$$. In this essay, we assuming the (unnessecarily strict) condition that all functions are of class $$C^\infty$$.

### Chain Rule and Linearity of the Derivative

The chain rule is how we compute the derivative of compositions of functions. It is usually justified using the following (incomplete) proof (when $$g$$ is not constant at $$t$$)

$$(f\circ g)'(t) = \lim_{\delta\to 0} \frac{f(g(t+\delta))-f(g(t))}{\delta} = \lim_{\delta\to 0} \frac{f(g(t+\delta))-f(g(t))}{g(t+\delta)-g(t)}\cdot \frac{g(t+\delta)-g(t)}{\delta} $$


$$= f'(g(t))\cdot g'(t)$$

This method of proof can be used to show that the derivative at any point is a linear map. For $$f:\mathbb{R}^n\to \mathbb{R}^m$$, $$u,v\in\mathbb{R}^n$$, and $$a,b\in\mathbb{R}$$

$$D_(av+bu)f^i = aD_vf^i+bD_uf^i$$

Linear map means vector space... rn has natural basis, and if f is




AT A POINT
1. Vector Space,
1. Linearity: acts on functions,  

For any functions

$$ D_1c(t)$$

Perhaps what is most interesting about this property is that it implies the *linearity of derivative*. Let $$\phi(t)_a=t_0+a(t-t_0)$$ be the linear function with derivative $$a$$ and $$\phi(t_0)=t_0$$, then $$(f\circ \phi_a)'(t_0)=af'(t_0)$$. This construction 

The same proof, when applied to

A similar procedure shows that

This construction may seem clunky

Where $$D_i$$ denotes $$D_{(0,...,1^i,...,0)}$$

Explains the name 

The derivative is pushing around the tangent vector


## Differentiation on Manifolds

### (Differentiable) Manifolds

Imagine you want to ...


To this point I've done my best to avoid expressing vectors as ... when working in Rn it can be useful to identify tangent vectors with column vectors and linear transformations as jacobian matricies.... great computationally, perfectly fine until you get to more complicated constructions on manifolds / tensors

## Differential Equations

## Equivalence on $$\mathbb{R}$$