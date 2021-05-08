---
layout: default
---
[back](./full-list.md)

<h1>
Bayesian Network</h1>
<h4>
Date: 2021-05-08
</h4>
<p>
What is a model?<br>
A model is a declerative representation of our understanding of the world. It's a representation
within a computer that captures our understanding of what these variables are and how they interact with
each other. Declerative means that the representation stands on its own which means that we make sense
of it aside from any algorithm that we might choose to apply on.
<br>
This means that the same model can be used in the context of one algorithm that answers any one kind
of question or other algorithms that might answe different kinds of questions, or the same question
in more efficient ways, or that make different trade-offs between accuracy and complicational cause.
<br>
Also, we can separate out the construction of the model from the algorithms that are used to reason it.
We can construct methodologies that elicit these models from a human expert or ones that learn it from
historical data using statistical machine learning techniques or a combination of the two.
<br>
<br>
What is probabilistic?<br>
Uncertainty. Uncertainty comes in many forms and for many
different reasons such as:<br>
- Partial knowledge of state of the world<br>
- Noisy observations<br>
- Phenomena not covered by our model<br>
- Inherently stochastic(randomly determined)<br>
<br>
Probability theory is a framework that allows us to deal with uncertainty in ways that are pricipled
and that bring to bear important and valuable tools.
- Declarative representation with clear semantics<br>
- Powerful reasoning patterns<br>
- Established learning methods<br>
<br>
What is graphical?<br>
Probabilistic graphical models are a synthesis between ideas from probability theory in statistics and
ideas from computer science.<br>
In order to capture probability distributions over spaces involving such a large number of factors, we
need to have probability distributions over what are called random variables.<br>
We need to represent the world through these variables each of which captures some facet of the world.<br>
Our goal is to capture our uncertainty about the possible states of the world in terms of their probability 
distribution or what's called a joint distribution over the possible assignments to the set of random 
variables.
<br>
<br>
An example of a graphical model is Bayesian networks.<br>
It uses a directed graph as the intrinsic (native) representation. In this case, the randome variables
are represented by nodes in the graph. The edges in the grpah represent the probabilistic connections
between those random variables in a way that is very formal.
<br>
Another example of a graphical model is called Markov networks.
It is an undirected graph.
<br>
Graphical representation is:<br>
- intuitive and compact data structure<br>
- efficient reasoning using general-purpose algorithms<br>
- sparse parameterization: feasible elicitation, learning from data - in both cases a reduction in
the number of parameters is very valuable<br>
<br>
<br>
Representation:<br>
- directed and undirected<br>
- temporal and plate models<br>
<br>
Inference (reasoning):<br>
- exact and approximate<br>
- decision making<br>
<br> 
Learning:<br>
- parameters and structure<br>
- with and without complete data<br>
<br>
Join Distribution in the student example:<br>
- variable 1: intelligence(I) - it has 2 values: low, high<br>
- variable 2: difficulty(D) - it has 2 values: easy, hard<br>
- variable 3: grade(G) - it has 3 values: g1, g3, g3<br>
<br>
P(I,D,G) = 2x2x3 = 12 probabilities
We also have indipendent parameters whose value is not completely determined by the value of other
parameters.<br>
All the probabilites have to sum to 1 so if you tell me eleven out of the twelve, I know what the 
twelfth is so the number of independent parameters is eleven.
<br>
Conditioning: Reduction<br>
- if we know one parameter this will cause reduction of the probabilities we came in the beginning.
This operation is called reduction.<br>
Unnormalized measure which means it doesn't sum to 1. So we need to normalize this distribution - make 
them sum to 1.<br>
Marginalization<br>
- marginalize over I or D - P(I,D)<br>
<br>
Factor:<br>
This is a function or a table that takes arguments (a set of variables), and just like any function
it gives us a value for every assignment.<br>
The set of variable is called the scope of the factor.<br>
A join distribution is a factor.<br>
For every value of I, D and G, a combination of values, I get a number that's why it's a factor.<br>
<br>
Conditional Probability Distribution (CPD)<br>
It gives us the conditional probability of the variable G given I and D - P(G | I,D).
This means for every combination of values to the variables I and D, we have a probability distribution over G.<br>
<br>
Factor Product<br>
 
Factor Marginalization<br>

Factor Reduction<br>
<br>
Why factors?<br>
- It turns out that these are the fundamental building block for defining distributions in high-dimensional spaces. That is the way in which we're going to define an exponentially large probability putting them together by multiplying factors in order to define these high dimensional probability distributions.<br>
- Also, the same set of basic operation that we use to define the probability distributions in these high dimensional spaces are also what we use for manipulating them in order give us a set of basic inference algorithms.<br>
Test:
1 - 0.16 0.45 0.6 
2 - 42 85 96 30
3 - A & B
4 - 108 135 79 141


  




</p>

