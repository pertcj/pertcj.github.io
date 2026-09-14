---
title: "RNN Generalization to Omega-Regular Languages"
collection: publications
category: workshops
permalink: /publication/2025-10-26-rnn-generalization/
order: 1
authors: '**Charles Pert**, Dalal Alrajeh, and Alessandra Russo'
abstract: |-
  Büchi automata (BAs) recognize 𝜔-regular languages defined by formal specifications like linear temporal logic (LTL) and are commonly used in the verification of reactive systems. However, BAs face scalability challenges when handling and manipulating complex system behaviors. As neural networks are increasingly used to address these scalability challenges in areas like model checking, investigating their ability to generalize beyond training data becomes necessary. This work presents the first study investigating whether recurrent neural networks (RNNs) can generalize to 𝜔-regular languages derived from LTL formulas. We train RNNs on ultimately periodic 𝜔-word sequences to replicate target BA behavior and evaluate how well they generalize to out-of-distribution sequences. Through experiments on LTL formulas corresponding to deterministic automata of varying structural complexity, from 3 to over 100 states, we show that RNNs achieve high accuracy on their target 𝜔-regular languages when evaluated on sequences up to 8× longer than training examples, with 92.6% of tasks achieving perfect or near-perfect generalization. These results establish the feasibility of neural approaches for learning complex 𝜔-regular languages, suggesting their potential as components in neurosymbolic verification methods.
date: 2025-10-26
year: 2025
venue: 'Artificial Intelligence and Formal Verification, Logic, Automata, and Synthesis (OVERLAY)'
note: ''
paperurl: 'https://ceur-ws.org/Vol-4142/paper2.pdf'
htmlurl:
codeurl: 'https://github.com/pertcj/omega-generalization'
bibtexurl: '/files/pert2025rnn.bib'
citation: 'Charles Pert, Dalal Alrajeh, and Alessandra Russo. (2025). &quot;RNN Generalization to Omega-Regular Languages.&quot; <i>7th International Workshop on Artificial Intelligence and Formal Verification, Logic, Automata, and Synthesis (OVERLAY 2025),</i>.'
---
