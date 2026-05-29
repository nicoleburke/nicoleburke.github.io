---
title: ""
permalink: /aiprojects/
layout: splash
---
## AI Projects
<!-- SIDE PROJECT SENTIMENT ANALYSIS -->
<div class="project-card featured">
  <div class="card-main">
    <div class="card-badge">💡 Side Project</div>
    <div class="card-title">People Analtyics: Sentiment Analysis on open-ended employee survey responses</div>
    
    <div class="card-body">
      Built a sentiment analysis pipeline using an open-source large language model to analyze a dataset containing 400 open-ended employee survey responses. I’ve been building meaningful relationships in the People Analytics space and a common question across teams and industries is the desire to utilize open-ended survey responses on employee surveys. Open-ended survey responses contain the richest qualitative signal in any employee dataset, but hand-coding thousands of responses is prohibitively slow. Further, datasets can vary in size, which means fine-tuning an NLP model is not an option. The challenge is finding something that can work out of box to automate coding sentiment.
    </div>
    
    <div class="card-meta">
      <span class="tag tag-blue">Python</span>
      <span class="tag tag-slate">Open Source LLMs</span>
      <span class="tag tag-slate">NLP</span>
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
      <span class="detail-value">Using an open source LLM via HuggingFace, I was able to use a model to automate sentiment on open-ended employee survey responses.</span>
    </div>
    <div class="detail-row">
      <span class="detail-label">Impact & Metrics</span>
      <span class="detail-value highlight-teal">The tool makes qualitative survey data tractable at scale — giving People Analytics teams access to the full richness of what employees actually write, not just how they rate things on a Likert scale.</span>
    </div>
  </div>
</div>

<!-- NYU NLP PROJECT -->
<div class="project-card featured">
  <div class="card-main">
    <div class="card-badge">🔬 Professional Work</div> 
    <div class="card-title">NLP Classification Pipeline using ChatGPT API</div>
    
    <div class="card-body">
      Reduced manual text processing time by <strong>50% (4 to 2 months)</strong> by building an <strong>NLP classification pipeline</strong> using the <strong>ChatGPT API</strong>, achieving 77% model accuracy on a language classification task. This project directly addresses whether AI can reliably categorize nuanced human language at scale, replacing months of manual coding with automated pipelines.
    </div>
    
    <div class="card-meta">
      <span class="tag tag-blue">R</span>
      <span class="tag tag-slate">NLP</span>
      <span class="tag tag-slate">chatGPT API</span>
      <span class="tag tag-slate">Data Pipelines</span>
    </div>
  </div>

  <div class="card-detail">
    <div class="detail-row">
      <span class="detail-label">The Question</span>
      <span class="detail-value">Can LLMs reliably classify complex human language at scale to replace manual human coding?</span>
    </div>
    <div class="detail-row">
      <span class="detail-label">What I Did</span>
      <span class="detail-value">Developed a structured API pipeline to feed utterance level text into GPT model and used prompt engineering to acheieve accuracy in language classification task.</span>
    </div>
    <div class="detail-row">
      <span class="detail-label">Impact & Metrics</span>
      <span class="detail-value highlight-teal"><strong>77% overall model accuracy</strong> achieved against human-coded benchmarks. This reduced our manual text process time by <strong>50%</strong>, which allowed us to expedite time to completion for research projects.</span>
    </div>
  </div>
</div>

<!-- Side Project: Automated Voice-Part Playlist Builder (built by AI) -->
<div class="project-card featured">
  <div class="card-main">
    <div class="card-badge">💡 Side Project</div>
    <div class="card-title">Automated Voice-Part Playlist Builder (built by AI)</div>
    
    <div class="card-body">
      Built a customized playlist with .mp4 files for my choir. We receive our practice tracks as individual .mp4 files on a shared Google Drive folder for each voice part. I saw an opportunity to use AI to build a playlist that would take the .mp4 files and make a Playlist by voice-part for the choir. This will make it easier for members to practice and we can track choir member usage via the app. 
      <br><br>
      <a href="https://nicoleburke.shinyapps.io/choir_app_r/" target="_blank" style="display: inline-flex; align-items: center; color: #2c4a52; font-weight: 600; text-decoration: none; border-bottom: 2px solid #c5ecf2; padding-bottom: 2px; transition: color 0.2s ease;" onmouseover="this.style.color='#4a7c8a'; this.style.borderBottomColor='#2c4a52'" onmouseout="this.style.color='#2c4a52'; this.style.borderBottomColor='#c5ecf2'">
        Launch Live App ↗
      </a>
    </div>
    
    <div class="card-meta">
      <span class="tag tag-blue">R Shiny App</span>
      <span class="tag tag-slate">AI Prototype</span>
      <span class="tag tag-slate">Engineering</span>
    </div>
  </div>

  <div class="card-detail">
    <div class="detail-row">
      <span class="detail-label">The Question</span>
      <span class="detail-value">Can AI generate a working prototype of a customized playlist for our choir, so members do not need to manually download and organize individual files each week?</span>
    </div>
    <div class="detail-row">
      <span class="detail-label">What I Did</span>
      <span class="detail-value">Used Claude to generate an R Shiny App to make a prototype for my choir director. The entire project took ~30mins. The prototype allowed me to share a working model to receive feedback.</span>
    </div>
    <div class="detail-row">
      <span class="detail-label">Impact & Metrics</span>
      <span class="detail-value highlight-teal">The tool makes it easier for choir members to practice. We saw an increase in practice through self-reported measures, which we could validate by tracking the usage of the application.</span>
    </div>
  </div>
</div>

<!-- Contract Work: AI Evaluation Dataset Question Developer -->
<div class="project-card featured">
  <div class="card-main">
    <div class="card-badge">🤝 Contract Work</div>
    <div class="card-title">AI Evaluation Dataset Question Developer</div>
    
    <div class="card-body">
      Designed a multiple-choice evaluation dataset for an AI company to test language model understanding of cognitive development concepts, achieving clear differentiation of model failures (i.e., ~20% accuracy) as measured by performance on conceptually discriminative questions, by creating 20-25 expert-level items with carefully constructed distractor answers that targeted common conceptual confusions rather than factual recall. 
    </div>
    
    <div class="card-meta">
      <span class="tag tag-slate">AI Evaluation Dataset</span>
      <span class="tag tag-slate">Prompt Engineering</span>
    </div>
  </div>

  <div class="card-detail">
    <div class="detail-row">
      <span class="detail-label">The Question</span>
      <span class="detail-value">Can a language model truly *understand* cognitive development concepts — or is it pattern-matching on surface-level cues? I was brought in to design an evaluation dataset that could tell the difference.</span>
    </div>
    <div class="detail-row">
      <span class="detail-label">What I Did</span>
      <span class="detail-value">Designed 20–25 expert-level multiple-choice items grounded in developmental psychology, with adversarial distractor answers constructed to exploit common conceptual confusions — not factual gaps. Each question was designed to distinguish true understanding from surface-level pattern matching.</span>
    </div>
    <div class="detail-row">
      <span class="detail-label">Impact & Metrics</span>
      <span class="detail-value highlight-teal">Consistent model failure on non-obvious conceptual distinctions confirmed the dataset had high diagnostic value. The items successfully differentiated models that understood the *structure* of developmental concepts from those recombining familiar terms.</span>
    </div>
  </div>
</div>
