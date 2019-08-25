---
layout: archive
collection: homework
title: "Homework 1 - Due ???"
permalink: /homework/hw1/
author_profile: true
---
## Intro 
Homework is a huge aspect of this course, both in terms of learning and in terms of grade. I strongly encourage you to work together on these homework problems, but you must turn in your own work. Collaborate with integrity!

This first homework is primarily concerned with getting up and running with Python and reviewing the vector calculus that Griffiths discusses in Chapter 1.

Handwritten solutions should be turned in on paper. Jupyter notebooks should be turned in by [linking to a Github commit dated before the deadline](http://evantilton.com/guides/linktogithubcommit/); you can send the link to the commit to me via a direct message in Slack.

## 1. Getting started with out computer-based tools

In this class, we will use Python in Jupyter notebooks, Slack for communication and collaboration, and Github to host our code. Your first job is to get these up and running. For some of these tasks, I have [guides available that might help you](http://evantilton.com/guides/).

1. Ensure that you can access our Slack team reliably at [ph410f19.slack.com](http://ph410f19.slack.com). If you have a smartphone or laptop, install the relevant app so that you can use it in class. If you do not have a smartphone or do not want to install this for some reason, let me know and we can discuss it and find a solution.
2. Set up Github.
    - Make a Github account. You can use a throwaway email address (e.g., a free gmail address that you use for nothing else), but I don't recommend it. Github is a great tool that you may want to use in the future.
    - [Create your first repository](https://help.github.com/en/articles/create-a-repo) in which you will host code you write for this class. I reccommend giving it a clear name -- for example, if I were setting one up, I might call it something like "ph410-etilton". **You are required to set this repository to private. Homework will not be accepted if it ever existed in a public repo.**
    - Add me as a collaborator in this repo. If you don't know how to do this, go to https://github.com/emtilt/YOUR_REPO_NAME_HERE/settings/collaboration once you are logged in to Github, altering the URL with your repo name. Then search for "Evan M Tilton" in the search field and add me as a collaborator. This will allow me to see and access files in this repo. I will never modify them, and I will not be able to see any of your other private repos. I will only use this to help you with homework and accept homework submission.
3. Get access to a way of working on Python Jupyter notebooks. I strongly suggest installing Anaconda, especially if you have one personal computer that you will use regularly, but Google Colab is another decent option for a cloud-based solution. Again, some [guides here might help you](http://evantilton.com/guides/).
4. Make a test notebook and ensure you know how to get it synced with Github. Google Colab allows opening and saving from Github. If you have a local Anaconda installation, I suggest the Github Desktop app or git from the commandline (again, see [guides available that might help you](http://evantilton.com/guides/)).

## 2. Vector math
Dot products and cross products will show up all over this course. Let's remind ourselves of their properties once more.
- Given the vectors $\vec{A}$ and $\vec{B}$

## 3. Integrals
In this course, you will perform many different kinds of integrals, some of which you have seen in other courses. In this problem, we will practice those integration techniques. 

1. *Line (or path) integrals* - You may have encountered these when discussing energy and work in a previous physics class. We'll use them frequently, especially when we talk about electric potential.
  - Determine the work done by the vector force $\mathbf{F} = y^2\;\hat{x} - 2x^2\;\hat{y}$ along the path $y=\sqrt{x}$ from (0,0) to (4,16). In case you forgot, recall that $W=\int \mathbf{F}\cdot d\mathbf{l}$.
  - Descibe in words what the line integral $W=\int \mathbf{F}\cdot d\mathbf{l}$ is doing. What is being "summed up"? Why is there a dot product?
  - Is this line integral path-independent (i.e., is $\mathbf{F}$ a [conservative vector field](https://en.wikipedia.org/wiki/Conservative_vector_field))? Explain how you can tell.
2. *Surface integrals* - Calculating the flux through a particular surface is a common way of determine the electric field, and doing so requires evaluating a surface integral.
  - Evaluate the integral $\int_S \mathbf{v}\cdot d\mathbf{A}$ where $\mathbf{v}(x,y,z) = 5x\;\hat{y} + 2y\;\hat{z}$ and $S$ is the rectangular surface lying in x-z plane from (0,0,0) to (1,0,5). Choose the direction of $+\hat{y}$ to be indicative of positive flux.
  - Explain how the resulting sign of the flux makes sense. You can use sketches or diagrams, if it helps.
3. *Volume integrals* - It will be common for you to determine the amount of total charge in a situation where the charge is distributed in space according to some function. You might be familiar with this concept from the perspective of distributed mass.
  - Consider two different spheres: one with uniform mass density, $\rho_0$, and the other with a radially varying density, $\rho(r)=\frac{3\rho_0}{4R^2}r^2$.
  - If both spheres have the same radius $R$, which has more mass?


#### 4. What operations can be done to different kinds of functions?
1. Given an arbitrary **scalar** function $T(x,y,z)$ (e.g., the temperature at any point in the room or the pressure at any point in the ocean), which of the three main differencal caulculus operations (div, grad, and/or curl) can be used to operate on $T$? For each which can:
  - give a formula for the result,
  - explain in words how you would interpret the result, and
  - identify if the result a vector or scalar.
2. Given an arbitrary  **vector** function $\vec{V}(x,y,z)$ (e.g., the velocity of air flowing in the atmosphere), which of the three operations (div, grad, and/or curl) can be used to operate on $\vec{V}$? For each which can:
  - give a formula for the result,
  - explain in words how you would interpret the result, and
  - identify if the result a vector or scalar.

#### 5. Determine the gradient of a scalar function
In Griffiths, $\vec{\mathfrak{r}}$ represents the separation vector between source charges $\langle x', y', z' \rangle$ and the field point -- location of test charge -- $\langle x, y, z \rangle$. The separation vector is a **critically important** vector in electrodynamics as it underlies all of the mathematical models that describe how source charges produce electric and magnetic fields. To that end, you will often do some mathematical manipulations of the separation vector. You are asked to perform two common manipulations below.

1. Calculate the gradient of the magnitude of the separation vector (i.e., $\nabla\|\vec{\mathfrak{r}}\|$).
2. Calculate the gradient of the inverse of the magnitude of the separation vector (i.e., $\nabla \dfrac{1}{\|\vec{\mathfrak{r}}\|}$).
3. Show the gradients of these functions can be written as functions of the separation vector ($\vec{\mathfrak{r}}$) and/or its magntiude ($\|\vec{\mathfrak{r}}\|$). (*Hint: it might be easier to do this by explicitly writing out the function in Cartesian coordinates.*)
4. What vector identities have you developed for the separation vector? This is just asking you to state them based on your answers from parts 1, 2, and 3.


#### 4. Analyzing divergence and curl visually
While it is important to be able to analytically calculate divergences and curls, it is also exceedingly useful to be able to identify them visually. This skill has many uses: it allows you to check the plausibility of analytical results or computer simulations, it can imply easier ways of solving some problems, and it can help you identify potential roadblocks when setting up experiments or simulations.Hence, visual inspection of a field (in our case, electromagnetic fields) is an important tool to understand which models might be used to analyze the field. This will also be important in our distinction between electric and magnetic fields, and will become even more useful when the fields begin to vary with time.

For each of the four vector fields sketched below:

1. Which of them have a nonzero *divergence* somewhere? (If the divergence is nonzero *only* at isolated points, which point(s) would that be?)
2. Which of the following fields have nonzero *curl* somewhere? (If the curl is nonzero *only* at isolated points, which point(s) would that be?)
3. Provide a brief explanation for each of your answers above.

![vector fields](../../images/hw1-divcurlfields.png "vector fields") 
|

#### 5. Plotting vector functions with `matplotlib`
Physics is both a mathematical and visual science. It is important to develop the ability to sketch and plot figures of various types. For the early part of this class, plotting the field generated by electric charges is important to understanding the field itself. In this problem, you will learn to use the [`matplotlib` library](http://matplotlib.org) to [plot vector fields](http://matplotlib.org/examples/pylab_examples/quiver_demo.html). As with the previous computational problem, you can [download this working Jupyter notebook](../jupyter/HW1-VectorFieldsProblem.ipynb) ([view it here](https://github.com/dannycab/phy481msu_f2019/blob/master/jupyter/HW1-VectorFieldsProblem.ipynb)), which describes how this kind of plotting is done for a specific case ($\vec{v}(x,y)=y\hat{x}$).

It will be up to you to plot additional figures for these cases:

1. $\vec{v}(x,y)=r\hat{r}$ (where $\vec{r}$ refers to the usual $\vec{r}$ in spherical coordinates.)
2. $\vec{v}(x,y)=\hat{r}/r$
3. $\vec{v}(x,y) = \dfrac{x}{(\sqrt{x^2+y^2})^3}\hat{x}+\dfrac{y}{(\sqrt{x^2+y^2})^3}\hat{y}$
4. $\vec{v}(x,y) = \hat{\phi}$ (where $\\phi$ is the usual plane-polar coordinate.)
5. For each case above, can you describe a physical situation where the field would be applicable?

**When we construct different kinds of fields in this class, you will use code like this to visualize the field and discuss it.**


#### 6. Vector proofs can be incredibly useful
In electromagnetism, developing a deep understanding of vector mathematics can facilitate a deeper understanding of the physical systems that we will investigate. While we will rarely ask you to prove relationships outright, knowing how certain proofs are done can often help you simplify a complicated problem.

For example, in this problem, you will learn how we often use general vector operations with unspecified surfaces to make general statements about the field. In Griffiths, you read about a few integral theorems: the gradient theorem, Gauss's theorem (for divergences), and Stokes' theorem (for curls). You will make use of those theorems to prove a few things to develop some intuition about vector calculus.

1. From vector calculus, you know that the curl of any gradient of any scalar field is zero: $\nabla \times \nabla T(x,y,z) = 0 $.
  - Use the corollary of the gradient theorem, namely that closed loop integral of any gradient of a scalar field is zero, $\oint \nabla T\cdot d\mathbf{l} = 0$, along with Stokes' theorem, $\int_S(\nabla \times \mathbf{v})\cdot d\mathbf{a} = \oint_C \mathbf{v}\cdot d\mathbf{l}$, to demonstrate that the curl of a gradient is zero.
  - What is the essential argument that needs to be made that proves that the result is generalizable to any situation? (*Hint: The surface (S) and thus the line (C) that bounds the surface are not specified.*)
  - What does your result from the previous question tell you about possibility of swirly-ness of the gradient of a temperature field, $\nabla T$, over any specified surface?
2. From vector calculus, you know that the divergence of the curl of any vector field is zero, $\nabla \cdot (\nabla \times \mathbf{v}) = 0$.
  - Use the corollary of Stokes' theorem, namely that the closed surface integral of the curl of a vector field is zero, $\oint_S (\nabla \times \mathbf{v})\cdot d\mathbf{a} = 0 $, along with the divergence theorem, $\int(\nabla \cdot \mathbf{v}) d\tau = \oint_S \mathbf{v}\cdot d\mathbf{a}$, to demonstrate that the divergence of a curl is zero.
  - What is the essential argument that needs to be made the proves the result is generalizable to any situation? (*Hint: The volume (V) and thus the surface (S) that bounds it are not specified.*)
3. By doing these two proofs, what do you feel like you learned about vector calculus that you didn't already know?

#### 7. Applying vector calculus knowledge

Griffiths and other E&M writers like to use elegant conceptualizations that quickly get you to a result with seemingly very little work. This relies on a deeper understanding of vector calculus, which you will develop in this course. In this problem, you will explain a conceptualization that helps you come to a result, then you will connect that conceptualization to a mathematical proof. For this, consider the surface integral that we define as the ''vector area'',

$\mathbf{a} = \iint_S d\mathbf{a}$.

1. For a hemispherical bowl (a half sphere) of radius $R$, you will find $\mathbf{a}$. Sketch the situation and show the vector $d\mathbf{a}$ in your sketch. In which direction will $\mathbf{a}$ point once the integral is complete? How do you know?
2. What is a reasonable guess for the value of $\vert\mathbf{a}\vert$? Why is that a reasonable guess?
3. Compute directly the value of $\mathbf{a}$ and comment on your guesses from parts 1 and 2. It's ok if your answers to parts 1 and 2 don't match the computed answer. Explain how things fit together (e.g., What did you get right? What needs more work on your conceptualization?).
4. The value of $\mathbf{a}$ takes on the same value for _any_ closed surface. What is a reasonable guess for $\mathbf{a}$ in this case? What is your rationale that makes that guess reasonable?
5. Show using the gradient theorem what the value of $\mathbf{a}$ is for any closed surface. Compare your result to your answer to part 4. Again, it's ok if your answer to part 4 don't match the computed answer. Explain how things fit together (e.g., What did you get right? What needs more work on your conceptualization?).
