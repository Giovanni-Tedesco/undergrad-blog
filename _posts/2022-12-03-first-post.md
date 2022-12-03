---
layout: default
title:  "Welcome!"
date:   2022-12-03 16:39:54 -0500
categories: Miscellaneous
usemathjax: true
---
Hello!

Welcome to my blog, I will mostly be using this to document my time as an undergraduate Math and Computer Science student at the University of Toronto, and to keep track of the things that I find particularly interesting as I progress through my education. 

I will likely be posting here on a variety of topics including Course TLDR's and breakdowns, miscellaneous ramblings about mathematics, topics I happen to be interested in the moment, and perhaps the occasional proof that I find interesting.

To kick things off I'm going to share with you one of my favourite proofs. Namely this is the proof that $$\mathbb{R} \times \mathbb{R}$$ is uncountable. It is slightly less famous then it's more traditional counterpart $$(0,1)$$ or $$\mathbb{R}$$ are uncountable, and I believe that it qualifies as a fact you would hope is true but isn't quite obvious how to prove.

To show that $$\mathbb{R} \times \mathbb{R}$$ is uncountable recall that we require a bijection $$f: \mathbb{R}\to \mathbb{R} \times \mathbb{R}$$ However we will go about constructing this bijection in a slightly roundabout way that I find entertaining. 

We will begin by proving $$(0,1) \times (0,1)$$ is uncountable by constructing a bijection $$g: (0, 1) \to (0, 1) \times (0, 1)$$. Notice that if $$x \in (0, 1)$$ then $$x$$ has an infinite decimal expansion of the form $$0.a_1b_1a_2b_2a_3b_3\ldots$$ where $$a_i, b_i$$ are digits from 0-9. We define our mapping g as follows

$$
x \mapsto (0.a_1a_2a_3a_4\ldots, 0.b_1b_2b_3b_4\ldots)
$$

I will leave it to the reader to check that this is indeed a bijection. Now using $$g$$ and the fact that we know there exists a bijection $$h: (0, 1) \to \mathbb{R}$$ we can define a third mapping $$\phi: (0, 1) \times (0, 1) \to \mathbb{R} \times \mathbb{R}$$ as

$$
(x, y) \mapsto (h(x), h(y))
$$

at last we can define our function $$f$$ as the composition $$f = \phi \circ g \circ h^{-1}$$. Notice that this is a function from $$\mathbb{R} \to \mathbb{R} \times \mathbb{R}$$ and since the composition of bijections is indeed a bijection we have constructed $$f$$ as needed. 

There is one small note to add here, we will only consider representations of numbes terminating in infinitely many 0's so as to avoid issues with 0.49999... = 0.5000. For our purposes we will only accept the latter. 


If you notice any issues with my proofs or wish for further clarifications please email me at giovanni.tedesco@mail.utoronto.ca. And I will be happy to address any concerns that you might have.


