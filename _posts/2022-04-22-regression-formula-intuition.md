---
layout: post
title: "Regression Formula Intuition"
date: 2022-04-22
author: Ayush Kanodia
categories: math statistics
usemathjax: true
---

# Regression note

I was recalling some intuition to understand the regression least squares formula, and I wrote it down in the process.

Recall the regression formula,

$$(X^T * X)^{-1} X^T y = b$$

We want $$y = X * b$$, and $$X \in R^{m*n}$$.

We know that this system has m equations and n unknowns, and

1. if m < n - multiple solutions
2. if m == n ; (mostly) exactly 1 solution (except when X is not invertible)
3. if m > n; unsolvable - this is the regression problem - find a good approximate solution for some definition of good approximate

Now if we look at the above matrix equation; it is telling us that $$y$$ is a linear combination of the columns of $$X$$, where the linear combination is given by the coefficients $$b$$.

Interpreting a column of $$X$$: a column of $$X$$ is the 'distribution' of covariate associated with that column as given by all data points. This is in the space $$R^m$$. Therefore, you can interpret the attempt to solve this equation as finding the best linear combination of the columns of $$X$$ which gives $$Y$$. 

Now; these columns each lie in an $$m$$ dimensional space and there are $$n$$ of these columns, where we have $$n << m$$ (typically) for regression. Therefore, the set $$S = space(col(X))$$ spans a subspace of $$R^m$$ (recall that you need at least m vectors to form a basis spanning $$R^m$$). Typically, y will NOT belong to $$S$$. In some sense, we are finding bs such that we go as close to $$y$$ as our subspace allows.

Recall the notion of projections from Linear Algebra. We try to project $$y$$ on to $$S$$. Recall how to do this.

$$y = X * b$$

or, $$X^T* y = X^T * X * b$$

or, $$X^T* (w + z) = X^T * X * b$$, $$w$$ is the projection of $$y$$ onto $$S$$, $$z$$ is the perpendicular vector; note that $$X^T * z = 0$$ as $$z$$ is in the nullspace of $$X$$ and the dot product of $$z$$ and each row of $$X$$ is 0.

Therefore, multiplying $$(X^T * X)^{-1}$$ on both sides, we get

$$(X^T * X)^{-1} X^T (w + z) = b$$

or, $$(X^T * X)^{-1} X^T y = b$$

Note that we could have pre multiplied anything, but with $$X^T$$, we know that:
1. $$X^T * X$$ is invertible, and
2. the meaning of $$b$$ (it is the projection and you can't get better than that!)! 