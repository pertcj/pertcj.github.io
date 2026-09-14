---
title: "Transition‑Based Acceptance for ω‑Regular Expression Synthesis"
collection: publications
category: manuscripts
permalink: /publication/2026-07-21-transition-based-synthesis/
order: 1
authors: '**Charles Pert**, Dalal Alrajeh, and Alessandra Russo'
abstract: |-
  Reactive systems, which maintain ongoing interactions with their environment, are typically modeled using ω-regular languages. These languages characterize system behavior with infinite-length execution traces and are represented as nondeterministic Büchi automata (NBAs) or ω-regular expressions. Existing methods for synthesizing expressions from NBAs only handle state-based acceptance. This limitation forces the conversion of compact transition-based NBAs into larger state-based NBAs before synthesis. This article introduces the first direct synthesis method for ω-regular expressions from transition-based NBAs, eliminating the need for this transformation. The method works by decomposing an NBA into triplets of nondeterministic finite automata, subsuming existing pair-based decompositions to handle transition-based acceptance. We prove that our decomposition is correct, establishing our method’s soundness and completeness. We discuss the time and descriptional complexity of our method. Our empirical evaluation on 185 linear temporal logic formulas supports our hypothesis; transition-based synthesis reduces postfix size by 4.1× and 1.5× for recurrence and reactivity properties, respectively. We also analyze the structural NBA factors that determine when the transition-based NBA will yield a more compact expression and develop this into a simple criterion that, when applied, yields expressions that are at least as compact as those obtained by direct state-based synthesis.
date: 2026-07-21
year: 2026
venue: 'Formal Aspects of Computing (FAC)'
note: ''
paperurl: 'https://dl.acm.org/doi/full/10.1145/3803799'
htmlurl:
codeurl: 'https://github.com/pertcj/nba-expression-synthesis'
bibtexurl: '/files/pert2026transition.bib'
citation: 'Charles Pert, Dalal Alrajeh, and Alessandra Russo. (2026). &quot;Transition‑Based Acceptance for ω‑Regular Expression Synthesis.&quot; <i>Formal Aspects of Computing (FAC)</i>.'
---
