---
layout: post
title:      "Seven Bridges and Machine Learning"
date:       2020-10-07 09:55:32 -0400
permalink:  lorum_ipsum
---


## Königsberg, 1735

![Konigsberg](https://scilogs.spektrum.de/hlf/files/konigsberg_plain-1024x713.png)

In the year 1735 the Prussian city of Königsberg was divided into 4 distinct landmasses by 7 different bridges that stretched across the river Pregel. A question was poised concerning the bridges. Could a man traverse all bridges, without doubling back and end back up where they started. This perplexing question would launch a branch of mathematics on its own, and that branch of mathematics is more relevant now than ever before.

Leonhard Euler would prove this question had no answer, and the way he did it would form the foundations of **Graph Theory** . Euler would relay,

> This question is so banal, but seemed to me worthy of attention in that geometry, nor algebra, nor even the art of counting was sufficient to solve it.

to Italian mathematician and engineer, Giovanni Marinoni after having earlier states,

> . . .  Thus you see, most noble Sir, how this type of solution bears little relationship to mathematics, and I do not understand why you expect a mathematician to produce it, rather than anyone else, for the solution is based on reason alone, and its discovery does not depend on any mathematical principle.  Because of this, I do not know why even questions which bear so little relationship to mathematics are solved more quickly by mathematicians than by others.

to Carl Leonhard Gottlieb Euler, mayor of Danzig who inquired about a solution to the problem.

It is interesting to see the prospective of Euler in reference to the Seven Bridges problem. He considered this thought experiment a pure exercise in reason with no foundation in mathematics. He posited though, that mathematicians would be the quickest to solve this spurious question. In 1735 he would solve the problem by proving that there was no solution as a man could not walk all seven bridges and return to the same site from whence he started without having to at least double back a single time. He did this by considering the map as an **abstract system**. Each landmass would be a **vertex** or **node** and each bridge would be an **edge** or **link**. This would form the basis of a new mathematical structure known as a **graph**. In postulating a solution (or non-solution in this case) Euler developed an entirely new form of mathematical structure. Now, though we don't consider it often, we are faced with graphs daily. 

## Connections

![Konigsberg](https://miro.medium.com/max/660/0*qIdIy_doNTwZkCSS.jpg)

Graphs model **pairwise relations** between objects and as previously mentioned they are made up of two elements, vertices and edges. A graph can be mapped as an unordered list of every edge between vertex pair. Graphs are important because of the way they empower our ability to map relationships, and because by nature humans are visual. Graphs are an inherently visual structure that is a little less obscure than something like an equation. A graph can represent many things from connections in a social network to a measure of a movie stars fame and reach, so if you guessed they had a use in computer science, and in particular data science, then you would have guessed correctly!

## The Graph and Data Science

![https://tkipf.github.io/graph-convolutional-networks/](https://tkipf.github.io/graph-convolutional-networks/images/gcn_web.png)

Just as graphs help humans better understand relational information graphs of sufficient size and scope can stymie a person's ability to perceive the information that the graph is trying to display. In that way computers also have difficult storing large graphs and parsing them for understanding. Graphs, to that end, are also also difficult for a neural network to understand as they are an arbitrary topology. As an arbitrary topology it is hard to tell where a graph begins and where it ends. Neural networks operate more efficiently on structured data. However, there have been many experimental frameworks that can transverse a graph and successfully transform them into a vector for processing in a neural network. Working much like word embeddings graphs can have graph embeddings that seek to gain information from graphs by mapping the node relationships between graphs. 

The paper *Relational inductive biases, deep learning, and graph networks* suggests numerous methods in which one may implement graphs into their neural networks. The abstract of the paper posits:

> We argue that combinatorial generalization must be a top priority for AI to achieve human-like abilities, and that
structured representations and computations are key to realizing this objective. Just as biology
uses nature and nurture cooperatively, we reject the false choice between “hand-engineering”
and “end-to-end” learning, and instead advocate for an approach which benefits from their
complementary strengths. We explore how using relational inductive biases within deep learning
architectures can facilitate learning about entities, relations, and rules for composing them. We
present a new building block for the AI toolkit with a strong relational inductive bias—the graph
network—which generalizes and extends various approaches for neural networks that operate
on graphs, and provides a straightforward interface for manipulating structured knowledge and
producing structured behaviors. We discuss how graph networks can support relational reasoning
and combinatorial generalization, laying the foundation for more sophisticated, interpretable,
and flexible patterns of reasoning. As a companion to this paper, we have also released an
open-source software library for building graph networks, with demonstrations of how to use
them in practice.

The authors argue that the graph network will revolutionize the AI process by allowing the breakdown of knowledge by generating and parsing structured knowledge to generate structured behaviors.

## Conclusion

Graphs are a part of everyday life, and most of us do not even realize it. Even more important however is that graphs are quickly becoming a large part of data science with experts agreeing that the AI of the future will benefit the most from Machine Learning from a graph structure due to the ubiquitous nature of graphs.
