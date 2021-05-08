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

 


</p>

