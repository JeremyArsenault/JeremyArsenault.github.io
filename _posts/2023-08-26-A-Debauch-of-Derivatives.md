---
layout: post
title: A Debauch of Derivatives
date: 2023-08-26
published: false
---

# UNDER CONSTRUCTION

After literally and figuratively sleeping through two years of an undergraduate curriculum in mathematics, I found myself in a course on partial differential equations where I was confronted by concise mathematical expressions that not only completely describe huge classes of dynamical systems, but were important in ostensibly unrelated fields of physics including electromagnetism, relativity, and quantum field theory. My curiosity, and therefore my interest, in math was rekindled, so armed with but a textbook and a pencil I impetuously manipulated expressions and chain ruled my way into the dawn...

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

### The Tangent Space on $$\mathbb{R}^n$$

### Chain Rule and Linearity of the Derivative

The chain rule is how we compute the derivative of compositions of functions. It is usually justified using the following (incomplete) proof (when $$g$$ is not constant at $$t$$)

$$(f\circ g)'(t) = \lim_{\delta\to 0} \frac{f(g(t+\delta))-f(g(t))}{\delta} = \lim_{\delta\to 0} \frac{f(g(t+\delta))-f(g(t))}{g(t+\delta)-g(t)}\cdot \frac{g(t+\delta)-g(t)}{\delta} $$


$$= f'(g(t))\cdot g'(t)$$

Similarly, stated in terms of the directional derivative, the chain rule for functions $$g:\mathbb{R}^n\to \mathbb{R}^m$$, $$f:\mathbb{R}^m\to \mathbb{R}^l$$, and $$x,v\in\mathbb{R}^n$$ is

$$D_v(f\circ g)^i(x) = D_{(D_vg^1(x),...,D_vg^m(x)}f^i(g(x))$$

An interesting consequence of this is property is that the derivative is a linear operator.

$$D_vf^i(x) = (\sum_{j=1}^m v^jD_jf^i)(x)$$

Where $$D_i=D_{(\delta_i^1,...,\delta_i^n)}$$ denotes the directional derivative with respect to the $$i$$th standard basis vector of $$\mathbb{R}^n$$.

We find this interesting later... can we preview that now? Maybe scope of essay is too broad... lecture on tangent space and differentiable manifolds is huge?

### Submaniflods and Parameterization

## Differentiation on Manifolds

### (Differentiable) Manifolds

Imagine you want to ...

Tangent vectors ...

To this point I've done my best to avoid expressing vectors as ... when working in Rn it can be useful to identify tangent vectors with column vectors and linear transformations as jacobian matricies.... great computationally, perfectly fine until you get to more complicated constructions on manifolds / tensors

## Ordinary Differential Equations

key point of essay: 

Itentification of R with TR -> gives rise to initial conditions of ODEs

Can all ODEs (and PDEs) be expressed as differential forms?



want to note that the ordinary 1d deriv is a rule for comparing tangent spaces, this is where initial conditions come from (w/o integral)

## Recap: Notational Equivalence on $$\mathbb{R}$$