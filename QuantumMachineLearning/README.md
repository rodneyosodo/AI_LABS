Quantum machine learning
===

## Table of Contents

[TOC]

## Beginners Guide

If you are a total beginner to this, start here!

1. Quantum mechanics
2. Machine learning
3. Quantum computing with qiskit
4. Quantum machine learning

User story
---

```gherkin=
Feature: Guess the word

  # The first example has two steps
  Scenario: Maker starts a game
    When the Maker starts a game
    Then the Maker waits for a Breaker to join

  # The second example has three steps
  Scenario: Breaker joins a game
    Given the Maker has started a game with the word "silky"
    When the Breaker joins the Maker's game
    Then the Breaker must guess a word with 5 characters
```
> I choose a lazy person to do a hard job. Because a lazy person will find an easy way to do it. [name=Bill Gates]



# Theory
## Quantum mechanics
1. Newton - Light consisted of particles

2. Huygens 
        - light was a wave
        - The were both light

3. Einstein - particles, photons, consist of energy
4. Bohr - atom consist of small positive charges neucleus with electrons orbiting around each other

5. Quantum leap - movement from ne discrete energy level to another
6. quanta a minimum quantity of energy
7. Heisenberg - uncertainty principle
8. Superposition existing in both states
9. Entanglement - the quantum states of two or more objects can be desribed in reference to each other where seprerated by distance
10. classical bits = binary data
11. quantum bit - can exist in both states until measured



Quantum devices can be used to accelerate machine learning

For linear algebra we need to encode the data to quantum bits

Quantum computers will speed up some AI algorithsm, enable new AI algorithms and help AI learn know new quantum algorithms


#### Finding eigenvalues and eigenvectors of large matrices:

One of the methods to perform the classical PCA algorithm is to take the eigenvalue decomposition of a data covariance matrix. However, this is not so efficient in case of high dimensional data.

Quantum PCA of an unknown low-rank density matrix, can reveal the quantum eigenvectors associated with the large eigenvalues, exponentially faster than a linearly-scaled classical algorithm.

 
#### Finding nearest neighbours on a quantum computer:

The quantum algorithms  presented here for computing nearest neighbours that are used in supervised and unsupervised learning, place an upper bound on the number of queries to the input data required to compute distance metrics such as the Euclidean distance and inner product. The best cases show exponential and super-exponential reductions in query complexity and the worst case still shows polynomial reduction in query complexity over the classical analogue.



## Machine learning
Machine learning is taking data and finding patterns in the data.
Eg voice recognition it listens to what you say and trys to find what you are saying, your intents.

It is still hard to extract patterns from data with our classical computers.

Examples that have failed
- Supervised
    - Support vector machine
    - K nearest neighbours
- Unsupervised
    - Clustering
    - Principal Component Analysis
- Deep learning
    - Boltzmann machine

So this is just a problem in linear algebra in high vector spaces.
There are alot of machine learning algorithms that depend on linear algebra in high dimensional vector spaces. 

Methods, what lie under the hood for most machine learning algorithms.
- FFT
- Finding eigen vectors and eigen values
- Matrix inversion
 

## Quantum machine learning

Vectors are in high dimensional space. 

We need to encode data from classical data to quantum mechanical state.
![](https://i.imgur.com/IqfofDl.png)

For classical data we have d=2^(2).

For the quantum system we have states which is equal to
![](https://i.imgur.com/xcrUjwX.png)

where n is the number of possible states

This means that we have exponential compressed the data in representation

| Algorithm | Classical | Quantum |
| -------- | -------- | -------- |
|FFT|![](https://i.imgur.com/Fco801W.png)| ![](https://i.imgur.com/zVVcMG9.png)|
|Finding eigen values and eigen vectors| ![](https://i.imgur.com/ixMOprb.png)| ![](https://i.imgur.com/zVVcMG9.png)|
|Matrix inversion|![](https://i.imgur.com/Fco801W.png)|![](https://i.imgur.com/hUCKOpR.png)|

As we can see quatum states have exponentially reduced the number of bits
For classical systems the would have many data bits hence they would preprocess the data in order to reduce it to fit in a higher dimensional space. Eg netflix

For a terabyte of data we will only need to use a circuit with only 40 qubits

Deep learning doesn't necessitate faster processes but will necessitate faster linear algebra computations.

## qRAM
![](https://i.imgur.com/baghHqW.jpg)

## Quantum computing

> Read more about Gherkin here: https://docs.cucumber.io/gherkin/reference/
>
> Awesome quantum machine learning: https://github.com/krishnakumarsekar/awesome-quantum-machine-learning

## Appendix and FAQ

:::info
**Find this document incomplete?** Leave an issue !
:::
