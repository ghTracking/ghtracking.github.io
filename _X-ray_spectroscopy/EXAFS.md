---
layout: default
title:  "Extended X-ray Absorption Fine Structure (EXAFS)"
categories: physical
---

<!---  https://katex.org/docs/autorender.html -->
<link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/katex@0.13.11/dist/katex.min.css" integrity="sha384-Um5gpz1odJg5Z4HAmzPtgZKdTBHZdw8S29IecapCSB31ligYPhHQZMIlWLYQGVoc" crossorigin="anonymous">
<script defer src="https://cdn.jsdelivr.net/npm/katex@0.13.11/dist/katex.min.js" integrity="sha384-YNHdsYkH6gMx9y3mRkmcJ2mFUjTd0qNQQvY9VYZgQd7DcN7env35GzlmFaZ23JGp" crossorigin="anonymous"></script>
<script defer src="https://cdn.jsdelivr.net/npm/katex@0.13.11/dist/contrib/auto-render.min.js" integrity="sha384-vZTG03m+2yp6N6BNi5iM4rW4oIwk5DfcNdFfxkk9ZWpDriOkXX8voJBFrAO7MpVl" crossorigin="anonymous"
    onload="renderMathInElement(document.body);"></script>

## What is the EXAFS experimental setup?



## Why does synchrotron radiation improve EXAFS?

## How does probability relate to EXAFS?



## What is the EXAFS equation?

# Athena

## What are the basic steps in EXAFS analysis?
- Convert intensity to $\mu$, the absorption coefficient. 
- Fit background to the pre-edge and post-edge, before subtracting these functions and normalising to the absorption at the edge.
- Fit a spline function to the background for the XAFS in order to extract this. 
- Convert to $k$-space
$$k = \sqrt{\frac{2m(E-E_o)}{\hbar^2}}$$
- Multiply values by 2 or 3 in order to amplify significance of values at higher k
- Multiply by window function to avoid ringing
- Fourier transform to move to $r$-space. There will be an evident offset due to phase shift.

## What is a k-weight? 



## What is spline range?



## What is the importance of the background?



## What is Rbkg? 