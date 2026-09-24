---
layout: page
title: Research
permalink: /research/
description: Research on trustworthy AI, learning from limited data, and uncertainty-aware applications.
nav: true
nav_order: 3
---

<style>
.research-intro { max-width: 780px; font-size: 1.09rem; line-height: 1.7; margin: .3rem 0 2rem; }
.research-section { margin: 2rem 0 2.6rem; }
.research-section > h2 { margin-bottom: .25rem; }
.research-section > p { color: var(--global-text-color-light); margin-bottom: 1.15rem; }
.research-list { display: grid; grid-template-columns: repeat(2, minmax(0, 1fr)); gap: 1rem; }
.research-card { --research-accent: #6941c6; border: 1px solid var(--global-divider-color); border-top: 3px solid var(--research-accent); border-radius: 13px; padding: 1.15rem 1.3rem; background: var(--global-card-bg-color); min-width: 0; }
.research-card:nth-child(3n + 2) { --research-accent: #147e76; }
.research-card:nth-child(3n) { --research-accent: #ad6924; }
.research-meta { font-size: .76rem; font-weight: 700; letter-spacing: .035em; text-transform: uppercase; color: var(--research-accent); }
.research-card h3 { font-size: 1.12rem; line-height: 1.35; margin: .35rem 0 .55rem; }
.research-card p { font-size: .94rem; line-height: 1.6; margin: 0 0 .8rem; }
.research-card a { color: var(--research-accent); font-size: .85rem; font-weight: 650; text-decoration: none; }
.research-card a:hover, .research-card a:focus { text-decoration: underline; }
.research-thesis { --research-accent: #147e76; max-width: 800px; }
@media (max-width: 700px) { .research-list { grid-template-columns: 1fr; } }
</style>

<p class="research-intro">I study how AI can learn from limited data and make reliable predictions, especially when a model is uncertain. My work spans evidential and Bayesian deep learning, few-shot learning, and applications in vision, behavioral data, and physical science.</p>

<section class="research-section" aria-labelledby="research-methods">
  <h2 id="research-methods">Trustworthy learning</h2>
  <p>Methods for learning with fewer examples and understanding what a model knows.</p>
  <div class="research-list">
    <article class="research-card">
      <div class="research-meta">IEEE TPAMI · 2026</div>
      <h3>Help evidential models keep learning</h3>
      <p>Generalized the regularization behind our ICML 2023 work to multiple evidential activation functions. The analysis explains when training can stall and how to restore a useful learning signal; experiments span classification, few-shot recognition, and image restoration.</p>
      <a href="https://doi.org/10.1109/TPAMI.2026.3660699">Generalized Regularized Evidential Deep Learning Models ↗</a>
    </article>
    <article class="research-card">
      <div class="research-meta">NeurIPS · 2024</div>
      <h3>More reliable adaptation of vision models</h3>
      <p>Introduced Bayesian parameter-efficient fine-tuning to address underconfidence when adapting pretrained vision models with few examples. It combines a stronger prior from pretraining with an evidential ensemble for better calibrated uncertainty.</p>
      <a href="https://proceedings.neurips.cc/paper_files/paper/2024/hash/4f1fbd5ab8d58d0ecf33c95fd46b900e-Abstract-Conference.html">Be Confident in What You Know ↗</a>
    </article>
    <article class="research-card">
      <div class="research-meta">ICML · 2023</div>
      <h3>Learn from every training example</h3>
      <p>Identified why evidential networks can stop learning from examples that fall in zero-evidence regions. Proposed a regularizer that lets those examples contribute to training, improving performance on challenging datasets.</p>
      <a href="https://proceedings.mlr.press/v202/pandey23a.html">Learn to Accumulate Evidence from All Training Samples ↗</a>
    </article>
    <article class="research-card">
      <div class="research-meta">AAAI · 2023</div>
      <h3>Separate kinds of uncertainty in few-shot prediction</h3>
      <p>Developed Evidential Conditional Neural Processes to distinguish uncertainty caused by scarce knowledge from uncertainty inherent in the data. The model is designed for few-shot regression and robustness to noisy training tasks.</p>
      <a href="https://doi.org/10.1609/aaai.v37i8.26125">Evidential Conditional Neural Processes ↗</a>
    </article>
    <article class="research-card">
      <div class="research-meta">CVPR · 2022</div>
      <h3>Choose the most useful few-shot tasks</h3>
      <p>Developed a multidimensional belief measure to estimate uncertainty in meta-learning tasks and guide which tasks to label and train on. A multi-query formulation further reduces labeling and computation in few-shot image classification.</p>
      <a href="https://openaccess.thecvf.com/content/CVPR2022/html/Pandey_Multidimensional_Belief_Quantification_for_Label-Efficient_Meta-Learning_CVPR_2022_paper.html">Multidimensional Belief Quantification ↗</a>
    </article>
  </div>
</section>

<section class="research-section" aria-labelledby="research-collaborations">
  <h2 id="research-collaborations">Research collaborations</h2>
  <p>Applying uncertainty-aware and physics-informed learning to real-world data.</p>
  <div class="research-list">
    <article class="research-card">
      <div class="research-meta">APL Machine Learning · 2024</div>
      <h3>Learn physical laws from sparse simulations</h3>
      <p>Developed a physics-informed equation-of-state model that learns an underlying free-energy function from simulated energy and pressure. This construction yields accurate predictions while respecting thermodynamic relationships.</p>
      <a href="https://doi.org/10.1063/5.0192447">Physics-informed equation-of-state model ↗</a>
    </article>
    <article class="research-card">
      <div class="research-meta">Machine Learning: Science and Technology · 2024</div>
      <h3>Predict energy and pressure consistently</h3>
      <p>Built a deep regression approach for equation-of-state tables with scarce training data, using meta-learning style training, uncertainty regularization, and ensembling. The work also checks thermodynamic consistency of its predictions.</p>
      <a href="https://doi.org/10.1088/2632-2153/ad2626">Deep energy-pressure regression ↗</a>
    </article>
    <article class="research-card">
      <div class="research-meta">ICML · 2023</div>
      <h3>Discover patterns in behavior over time</h3>
      <p>Combined temporal set representations with uncertainty-aware attention to find informative patterns in visual and touch interactions. The study evaluates the approach on child-computer interaction data for autism research.</p>
      <a href="https://proceedings.mlr.press/v202/wang23ab.html">Deep Temporal Sets with Evidential Reinforced Attentions ↗</a>
    </article>
    <article class="research-card">
      <div class="research-meta">IEEE Big Data · 2021</div>
      <h3>Find the informative part of a long time series</h3>
      <p>Developed uncertainty-aware multiple-instance learning to identify the useful segment of a long vessel trajectory, then combine it with satellite imagery when the trajectory prediction is unreliable.</p>
      <a href="https://doi.org/10.1109/BigData52589.2021.9671469">Uncertainty-Aware Multiple Instance Learning ↗</a>
    </article>
  </div>
</section>

<section class="research-section" aria-labelledby="research-undergraduate">
  <h2 id="research-undergraduate">Undergraduate research</h2>
  <div class="research-card research-thesis">
    <div class="research-meta">Pulchowk Campus · Undergraduate thesis · 2017</div>
    <h3>Redirected Walking in Virtual Reality</h3>
    <p>Explored how to navigate a larger virtual environment within a smaller physical room. As the main developer, I implemented translation, rotation, and curvature gains in Unity, brought them into an HTC Vive game, and evaluated the experience with participants.</p>
    <a href="https://drive.google.com/file/d/1bM9cF2aNjRDZ9Yr5If0ON40mX6NfcCc7/view?usp=sharing">Read the project report ↗</a> <span aria-hidden="true"> · </span> <a href="{{ '/projects/undergraduate/' | relative_url }}#redirected-walking">See the project ↗</a>
  </div>
</section>
