---
title: ""
permalink: /aiprojects/
layout: single
---
## AI Projects

### AI Evaluation Dataset Question Developer  

##### The question

Can a language model truly *understand* cognitive development concepts — or is it pattern-matching on surface-level cues? I was brought in to design an evaluation dataset that could tell the difference.

#####  Why it was hard

Most evaluation datasets test factual recall. A model can score well by memorizing associations without any real conceptual understanding. Building a diagnostically useful benchmark requires the opposite: questions where a model that "knows the facts" still fails, because the distractors target the exact conceptual confusions a non-understanding system would make.

#####  What I did

Designed 20–25 expert-level multiple-choice items grounded in developmental psychology, with adversarial distractor answers constructed to exploit common conceptual confusions — not factual gaps. Each question was designed to distinguish true understanding from surface-level pattern matching.

The target accuracy for a non-understanding model was ~20% — roughly chance — which served as the benchmark signal that the questions were diagnostically valid.

#####  What it showed

Consistent model failure on non-obvious conceptual distinctions confirmed the dataset had high diagnostic value. The items successfully differentiated models that understood the *structure* of developmental concepts from those recombining familiar terms.

### Built NLP Classification Pipeline using chatGPT

##### The question

Can large language models reliably classify nuanced human language at scale — or do they break down when the categories require contextual interpretation rather than simple keyword matching?

##### Why it was hard

The dataset involved complex language classifications where meaning depended heavily on context, phrasing, and subtle semantic distinctions. Traditional rule-based approaches struggled to generalize, while manual coding required months of researcher time and introduced bottlenecks into the analysis pipeline.

The challenge was building a system accurate enough to meaningfully reduce human labor without sacrificing reliability on ambiguous cases.

##### What I did

Built an end-to-end NLP classification pipeline using the ChatGPT API to automate language classification within a large behavioral dataset. Designed prompts, preprocessing workflows, and validation procedures to evaluate model performance against human-coded benchmarks.

Iteratively refined the classification framework to improve consistency on edge cases and reduce systematic classification errors.

##### What it showed

The final pipeline achieved 77% classification accuracy while reducing manual text processing time by 50% — from roughly four months to two. The project demonstrated that large language models can substantially accelerate qualitative research workflows when paired with rigorous validation and thoughtfully designed evaluation procedures.




1. Side Project: Employee Sentiment 

2. NLP classification pipeline 

3. shiny app built in 25 mins 

4. AI evaluation dataset 
•	Designed a multiple-choice evaluation dataset for an AI company to test language model understanding of cognitive development concepts, achieving clear differentiation of model failures (i.e., ~20% accuracy) as measured by performance on conceptually discriminative questions, by creating 20-25 expert-level items with carefully constructed distractor answers that targeted common conceptual confusions rather than factual recall. 
•	Improved evaluation quality for model benchmarking by ensuring high diagnostic value of questions as measured by consistent model failure on non-obvious conceptual distinctions, by leveraging domain expertise in developmental psychology to construct adversarial answer choices that distinguished true conceptual understanding from surface-level pattern matching.

