---
title: ""
permalink: /aiprojects/
layout: splash
---
## AI Projects

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
____________________________________________________________________________________________________________________________________________________

### Side Project: Sentiment Analysis on open-ended employee survey responses

##### The question

Can large language models reliably extract meaningful organizational insights from open-ended employee feedback — or does important nuance disappear when qualitative responses are analyzed at scale?

##### Why it was hard

Open-ended employee survey responses contain some of the richest signals about morale, leadership, burnout, and organizational culture, but they are notoriously difficult to analyze systematically. Manual coding is slow and difficult to scale, while traditional sentiment analysis methods often miss context, sarcasm, mixed sentiment, and emotionally complex responses.

The challenge was building a workflow that could surface meaningful patterns across hundreds of qualitative responses without flattening the human complexity that made the data valuable in the first place.

##### What I did

Built a sentiment analysis pipeline using an open-source large language model to analyze a dataset containing 400 open-ended employee survey responses. Designed prompting and classification procedures to identify patterns in employee sentiment and extract recurring themes across responses.

Used the model outputs to organize qualitative feedback into interpretable categories that could be incorporated into broader organizational analyses and decision-making workflows.

##### What it showed

The sentiment analysis surfaced patterns that were not visible in structured survey metrics alone, demonstrating the value of combining qualitative feedback with scalable NLP workflows. The project showed how open-source language models can help organizations transform large volumes of unstructured employee feedback into actionable insight while preserving much of the nuance present in human responses.
____________________________________________________________________________________________________________________________________________________

### Side Project: Automated Voice-Part Playlist Builder (built by AI)

##### The question

How can you make large collections of distributed media files actually usable for non-technical people — without asking them to manually download, organize, and manage dozens of individual files?

##### Why it was hard

My choir distributes rehearsal tracks as individual .mp4 files through a shared Google Drive. In practice, this made mobile listening frustrating: singers had to manually locate, download, and organize files one at a time, often across multiple voice parts and rehearsal sessions.

The underlying problem wasn’t file storage — it was usability. The system lacked a simple listening interface that matched how people actually consumed the content.

##### What I did

Built a lightweight R Shiny application in roughly 25 minutes using Claude as a coding collaborator. The app ingested rehearsal track files from Google Drive, automatically organized them by voice part, and generated a playlist-style listening interface optimized for mobile use.

Focused on rapid prototyping and practical UX: minimizing friction between receiving rehearsal materials and actually listening to them.

##### What it showed

The project demonstrated how quickly AI-assisted development can turn a small but meaningful user frustration into a working product. More importantly, it showed the value of combining behavioral intuition with rapid technical execution: identifying the real usability bottleneck, designing around user behavior, and shipping a functional solution almost immediately.

Even though the project was small in scope, it reflected the same mindset behind larger applied AI systems — using modern tools to reduce friction, improve user experience, and build practical solutions fast.
____________________________________________________________________________________________________________________________________________________

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