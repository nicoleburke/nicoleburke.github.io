---
title: ""
permalink: /aiprojects/
layout: splash
---
## AI Projects
<div class="project-card featured">
  <div class="card-main">
    <!-- <div class="card-badge">🚀 Core Project · NLP</div> -->
    <div class="card-title">NLP Classification Pipeline using ChatGPT API</div>
    
    <div class="card-body">
      Reduced manual text processing time by <strong>50% (4 to 2 months)</strong> by building an NLP classification pipeline using the ChatGPT API, achieving 77% model accuracy on a language classification task. This project directly addresses whether AI can reliably categorize nuanced human language at scale, replacing months of manual coding with automated pipelines.
    </div>
    
    <div class="card-meta">
      <span class="tag tag-teal">ChatGPT API</span>
      <span class="tag tag-teal">R</span>
      <span class="tag tag-teal">NLP</span>
      <span class="tag tag-slate">Data Pipelines</span>
    </div>
  </div>

  <div class="card-detail">
    <div class="detail-row">
      <span class="detail-label">The Question</span>
      <span class="detail-value">Can LLMs reliably classify complex, nuanced human language at scale to replace manual human coding?</span>
    </div>
    <div class="detail-row">
      <span class="detail-label">What I Did</span>
      <span class="detail-value">Developed a structured API pipeline to feed utterance level text into GPT model and used prompt engineering to acheieve accuracy in outputs.</span>
    </div>
    <div class="detail-row">
      <span class="detail-label">Impact & Metrics</span>
      <span class="detail-value highlight-teal"><strong>77% overall model accuracy</strong> achieved against human-coded benchmarks. This reduced our manual text process time by <strong>50%</strong>, which allowed us to expedite time to completion for research projects.</span>
    </div>
  </div>
</div>

<div class="project-card featured">
  <div class="card-main">
    <!-- <div class="card-badge">🚀 Core Project · NLP</div> -->
    <div class="card-title">Side Project: Sentiment Analysis on open-ended employee survey responses</div>
    
    <div class="card-body">
      Built a sentiment analysis pipeline using an open-source large language model to analyze a dataset containing 400 open-ended employee survey responses. I’ve been building meaningful relationships in the People Analytics space and a common question across teams and industries is the desire to utilize open-ended survey responses on employee surveys. Open-ended survey responses contain the richest qualitative signal in any employee dataset — but hand-coding thousands of responses is prohibitively slow. Further, datasets can vary in size, which means fine-tuning a NLP model is not an option. The challenge is finding something that can work out of box to automate coding sentiment.
    </div>
    
    <div class="card-meta">
      <span class="tag tag-teal">Open Source LLMs</span>
      <span class="tag tag-teal">Python</span>
      <span class="tag tag-teal">NLP</span>
      <span class="tag tag-slate">Data Pipelines</span>
    </div>
  </div>

  <div class="card-detail">
    <div class="detail-row">
      <span class="detail-label">The Question</span>
      <span class="detail-value">How can People Analytics teams extract meaningful signal from open-ended employee survey responses without spending months on manual coding?</span>
    </div>
    <div class="detail-row">
      <span class="detail-label">What I Did</span>
      <span class="detail-value">Using an open source LLM via HuggingFace, I was able to use a model to automate sentiment on open-ended employee survey responses. Code available here: LINK.</span>
    </div>
    <div class="detail-row">
      <span class="detail-label">Impact & Metrics</span>
      <span class="detail-value highlight-teal">The tool makes qualitative survey data tractable at scale — giving People Analytics teams access to the full richness of what employees actually write, not just how they rate things on a Likert scale.</span>
    </div>
  </div>
</div>




ABOVE IS TESTING

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

_____________________________________________________________________________________________________________________________________________________

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