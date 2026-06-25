---
title: "Antonin's AI Logbook"
date: 2026-06-17
categories: [AI]
tags: [machine-learning, mathematics, python]
author: antonin
description: Antonin's AI logbook
math: true
---

Wednesday, June 17, 2026. It has been nearly four years since ChatGPT was first released. Back then, I was in the third year of my bachelor's degree. The tool was not yet known to the general public, and nobody anticipated the scale of the revolution it would spark. 

At the time, I wasn't particularly well-versed in artificial intelligence. I only knew the bare fundamentals: a few key dates and the main fields like machine learning or deep learning. What attracted me the most to AI approaches was event or growth prediction, as well as classification.

Today, I am a PhD student in optimization within the field of Operations Research (OR). What is fascinating is the sheer number of parallels between OR and AI. Some principles are so closely related that it is sometimes difficult to draw a clear line between the two. Looking back, here is how I distinguish them: 

* **Operations Research (OR)** seeks the best possible decision by using mathematical models, constraints, and optimization algorithms.
    * *Examples:* Finding the least costly delivery route for 100 trucks, scheduling employees, or optimizing a supply chain.
* **Artificial Intelligence (AI)** seeks to mimic certain human capabilities, such as learning from data, recognizing images, understanding text, or making decisions in complex situations.
    * *Examples:* Recognizing a face in a photo, translating text, or predicting customer preferences.

Even though AI is far more than just ChatGPT, it is undeniable that this tool sparked a powerful new momentum, fostering numerous hybrid approaches across various fields. Operations Research is no exception: today, more and more optimization papers integrate artificial intelligence. For instance, we see machine learning models being used to predict good initial solutions to speed up mathematical solvers, or reinforcement learning applied to complex routing problems.

Learning and understanding the mechanisms of AI to eventually apply them to my own research has therefore become an obvious next step. It is in this context that I created this logbook, with the desire to share my learning journey from scratch, my reflections, my findings, as well as concrete examples and illustrations.

### What you will find in this logbook

Since I am starting (almost) from scratch, the idea is to document my progress step by step. Here is what I plan to explore in the coming weeks and months:
1. **Mathematical Foundations**
- Linear algebra, Probability and statistics, Optimization, Differential calculus, Numerical analysis
2. **Data & Feature Engineering**
- Data cleaning, Data visualization, Data pipelines, Feature engineering, Data quality
3. **Machine Learning**
- Regression, Classification, Clustering, Ensemble methods (Random Forest, Gradient Boosting, ...), Validation and metrics, Interpretability
4. **Deep Learning**
- Neural networks, CNN, RNN/LSTM, Attention mechanisms, Transformers
5. **Generative Models**
- Autoencoders, GANs, Diffusion Models, LLMs, Multimodal AI
6. **OR / AI Hybridization**
- Combinatorial optimization, Operations Research, Constraint Programming, Metaheuristics, Reinforcement Learning + OR, Decision Intelligence
7. **AI Systems & Architecture**
- Distributed systems, Vector databases, Caching, Event-driven architecture, Cost optimization
8. **AI Safety, Ethics & Governance**
- Bias, Explainability, Robustness, Privacy, AI regulation

This blog is primarily a personal note-taking space, but if you are curious to see behind the scenes of this learning process, you are more than welcome. Feel free to share your feedback or point out any beginner mistakes I might make along the way.

Let the learning journey begin!


# Mathematical Foundations

### Sets

In mathematics, a **set** $S$ is a collection of differents things. These things are called elements and can be everything.
> - $\emptyset$: Empty set
> - {red, green, blue}: Set of colors
> - $\mathbb{R}$: Set of real numbers
> - $\mathbb{N}_0$: Set of natural numbers including $0$
> - {$\mathbb{R}$, $\mathbb{N}_0$, $\emptyset$}: set of sets 
{: .prompt-info }

We denote by $\lvert S \rvert$ the cardinality of the set $S$, i.e. the number of elements inside
> - $\lvert$ {$\emptyset$} $\rvert = 1$ 
> - $\lvert$ {red, green, blue} $\rvert = 3$
{: .prompt-info }

We shall say that $K$ is a field if it satisfies the following conditions for the addition:

| **Property** | **Formalism** |
| Commutative | $x+y=y+x$ for all $x,y \in K$ |
| Associative | $x + (y + z) = (x +y) + z$ for all $x,y,z \in K$ |
| Existence of $0$ | $x+0=x$ for all $x\in K$ |
| Existence of the inverse | $\forall x$ there is $\exists -x \implies x + (-x) = 0$ |

And for the multiplication:

| **Property** | **Formalism** |
| Commutative | $x \cdot y=y \cdot x$ for all $x,y \in K$ |
| Associative | $x \cdot (y \cdot z) = (x \cdot y) \cdot z$ for all $x,y,z \in K$ |
| Existence of $1$ | $1\cdot x=x \cdot 1$ for all $x\in K$ |
| Existence of the inverse | $x^{-1}$ or $\frac{1}{x}$ in $K$ such that $xx^{-1} = 1$ |
| Distributive | $x \cdot (y+z) = x \cdot y + x \cdot z$, for all $x,y,z \in K$ |

Besides, we can take the union of two sets $S = S_1 \cup S_2$, i.e. all the elements of $S_1$ and $S_2$ are gathered in one set without ....:
> - $S_1 =$ {$1,2,3$}
> - $S_2 =$ {$3,4,5$}
> - $S = S_1 \cup S_2 =$ {$1,2,3,4,5$} with only one occurence of the element $3$
{: .prompt-info }

Or even the intersection of two sets $S = S_1 \cap S_2$, i.e. the common element of each set:
> - $S_1 =$ {$1,2,3$}
> - $S_2 =$ {$3,4,5$}
> - $S = S_1 \cap S_2 =$ {$3$}
{: .prompt-info }

### Scalars
### Vectors
### Matrices
### Tensors

