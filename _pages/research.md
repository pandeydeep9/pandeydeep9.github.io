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
.research-list { border-top: 1px solid var(--global-divider-color); }
.research-card { --research-accent: #6941c6; position: relative; border-bottom: 1px solid var(--global-divider-color); padding: 1.3rem 0 1.4rem 1.4rem; min-width: 0; }
.research-card::before { content: ''; position: absolute; left: 0; top: 1.45rem; bottom: 1.45rem; width: 3px; border-radius: 4px; background: var(--research-accent); }
.research-card:nth-child(3n + 2) { --research-accent: #147e76; }
.research-card:nth-child(3n) { --research-accent: #ad6924; }
.research-meta { font-size: .76rem; font-weight: 700; letter-spacing: .035em; text-transform: uppercase; color: var(--research-accent); }
.research-card h3 { font-size: 1.24rem; line-height: 1.35; margin: .3rem 0 .3rem; }
.research-authors { color: var(--global-text-color-light); font-size: .84rem; margin-bottom: .75rem; line-height: 1.5; }
.research-card p { max-width: 780px; font-size: .96rem; line-height: 1.65; margin: 0 0 .65rem; }
.research-card a { color: var(--research-accent); font-size: .88rem; font-weight: 650; text-decoration: none; }
.research-card a:hover, .research-card a:focus { text-decoration: underline; }
.research-thesis { --research-accent: #147e76; border-top: 1px solid var(--global-divider-color); }
</style>

<p class="research-intro">I study how AI can learn from limited data and make reliable predictions, especially when a model is uncertain. My work spans evidential and Bayesian deep learning, few-shot learning, and applications in vision, behavioral data, and physical science.</p>

<section class="research-section" aria-labelledby="research-methods">
  <h2 id="research-methods">Trustworthy learning</h2>
  <p>Methods for learning with fewer examples and understanding what a model knows.</p>
  <div class="research-list">
    <article class="research-card">
      <div class="research-meta">IEEE TPAMI · 2026</div>
      <h3>Help evidential models keep learning</h3>
      <div class="research-authors">Deep Shankar Pandey · Hyomin Choi · Qi Yu</div>
      <p>Evidential networks can estimate fine-grained uncertainty, but some activation functions give almost no learning signal for examples assigned little evidence. We analyzed how this happens across different activations and designed a family of activations and matching regularizers that lets the model continue updating its evidence.</p>
      <p>This extends the ICML 2023 result beyond one training setting. Experiments cover image classification, few-shot recognition, and blind face restoration.</p>
      <a href="https://doi.org/10.1109/TPAMI.2026.3660699">Generalized Regularized Evidential Deep Learning Models ↗</a>
    </article>
    <article class="research-card">
      <div class="research-meta">NeurIPS · 2024</div>
      <h3>More reliable adaptation of vision models</h3>
      <div class="research-authors">Deep Shankar Pandey · Spandan Pyakurel · Qi Yu</div>
      <p>Parameter-efficient fine-tuning can adapt a vision foundation model with very few examples, yet the resulting predictions may be too uncertain. Bayesian-PEFT strengthens the model's prior belief using knowledge acquired during pretraining and adds a diverse evidential ensemble to represent what remains uncertain.</p>
      <p>Across few-shot settings and fine-tuning methods, the paper evaluates both predictive accuracy and how well confidence matches outcomes.</p>
      <a href="https://proceedings.neurips.cc/paper_files/paper/2024/hash/4f1fbd5ab8d58d0ecf33c95fd46b900e-Abstract-Conference.html">Be Confident in What You Know ↗</a>
    </article>
    <article class="research-card">
      <div class="research-meta">ICML · 2023</div>
      <h3>Learn from every training example</h3>
      <div class="research-authors">Deep Shankar Pandey · Qi Yu</div>
      <p>We traced the weak performance of some evidential classifiers to a specific training failure: an activation can map an example into a zero-evidence region, leaving the model unable to learn from its label. Our theoretical analysis led to a regularizer that restores a learning signal for those examples.</p>
      <p>Experiments on challenging datasets show that an uncertainty-aware model need not discard useful training data to produce evidence-based predictions.</p>
      <a href="https://proceedings.mlr.press/v202/pandey23a.html">Learn to Accumulate Evidence from All Training Samples ↗</a>
    </article>
    <article class="research-card">
      <div class="research-meta">AAAI · 2023</div>
      <h3>Separate kinds of uncertainty in few-shot prediction</h3>
      <div class="research-authors">Deep Shankar Pandey · Qi Yu</div>
      <p>With only a few observations, a model needs to distinguish what it has not learned from noise that is inherent in the data. Evidential Conditional Neural Processes replace the usual Gaussian prediction of a conditional neural process with a hierarchical Bayesian structure that separates those two sources of uncertainty.</p>
      <p>The analysis explains the connection to standard conditional neural processes and the model's robustness to noisy training tasks; experiments test it on few-shot regression problems.</p>
      <a href="https://doi.org/10.1609/aaai.v37i8.26125">Evidential Conditional Neural Processes ↗</a>
    </article>
    <article class="research-card">
      <div class="research-meta">CVPR · 2022</div>
      <h3>Choose the most useful few-shot tasks</h3>
      <div class="research-authors">Deep Shankar Pandey · Qi Yu</div>
      <p>Meta-learning often trains on randomly chosen tasks, even though labeling and processing every task is costly. We developed a multidimensional belief measure that estimates a task's uncertainty and uses it to select informative tasks for training.</p>
      <p>A theoretical link between conflicting and incorrect belief makes this selection possible; a multi-query task design further improves label and compute efficiency in few-shot image classification.</p>
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
      <div class="research-authors">Joshua Hinz · Dayou Yu · Deep Shankar Pandey · Hitesh Sapkota · Qi Yu · Deyan I. Mihaylov · Valentin V. Karasiev · S. X. Hu</div>
      <p>Equations of state must predict energy and pressure without contradicting thermodynamics. The team built a physics-informed model that learns an underlying Helmholtz free-energy function from simulated energy and pressure, so its predictions are linked by the same physical structure.</p>
      <p>On warm dense polystyrene, the reported fit is within 1% relative error for both quantities and satisfies the Maxwell and Gibbs–Duhem relations.</p>
      <a href="https://doi.org/10.1063/5.0192447">Physics-informed equation-of-state model ↗</a>
    </article>
    <article class="research-card">
      <div class="research-meta">Machine Learning: Science and Technology · 2024</div>
      <h3>Predict energy and pressure consistently</h3>
      <div class="research-authors">Dayou Yu · Deep Shankar Pandey · Joshua Hinz · Deyan Mihaylov · Valentin V. Karasiev · S. X. Hu · Qi Yu</div>
      <p>Equation-of-state tables cover wide ranges of physical conditions, but simulations are expensive and training samples are sparse. This work combines a meta-learning style deep regressor, a kernel-based uncertainty regularizer, and an ensemble to improve the stability of energy and pressure estimates.</p>
      <p>The study verifies thermodynamic consistency with automatic differentiation, testing whether the learned table remains useful beyond an accurate numerical fit.</p>
      <a href="https://doi.org/10.1088/2632-2153/ad2626">Deep energy-pressure regression ↗</a>
    </article>
    <article class="research-card">
      <div class="research-meta">ICML · 2023</div>
      <h3>Discover patterns in behavior over time</h3>
      <div class="research-authors">Dingrong Wang · Deep Shankar Pandey · Krishna Prasad Neupane · Zhiwei Yu · Ervine Zheng · Zhi Zheng · Qi Yu</div>
      <p>Behavioral signals can be spread across time and different kinds of interaction. Deep Temporal Sets represent their temporal relationships, while Evidential Reinforced Attentions use uncertainty to explore which moments may be informative.</p>
      <p>Using visual and touch behavior from child-computer interactions, the study distinguishes children with autism spectrum disorder from typically developing children and identifies characteristic patterns in the data.</p>
      <a href="https://proceedings.mlr.press/v202/wang23ab.html">Deep Temporal Sets with Evidential Reinforced Attentions ↗</a>
    </article>
    <article class="research-card">
      <div class="research-meta">IEEE Big Data · 2021</div>
      <h3>Find the informative part of a long time series</h3>
      <div class="research-authors">Yuansheng Zhu · Weishi Shi · Deep Shankar Pandey · Yang Liu · Xiaofan Que · Daniel E. Krutz · Qi Yu</div>
      <p>A long vessel trajectory may contain only a short period that reveals its type. The proposed uncertainty-aware multiple-instance framework searches for that discriminative period instead of treating every observation as equally useful.</p>
      <p>Its uncertainty estimate also flags less trustworthy trajectory predictions and guides fusion with synthetic-aperture radar imagery when that additional information is available.</p>
      <a href="https://doi.org/10.1109/BigData52589.2021.9671469">Uncertainty-Aware Multiple Instance Learning ↗</a>
    </article>
  </div>
</section>

<section class="research-section" aria-labelledby="research-undergraduate">
  <h2 id="research-undergraduate">Undergraduate research</h2>
  <div class="research-card research-thesis">
    <div class="research-meta">Pulchowk Campus · Undergraduate thesis · 2017</div>
    <h3>Redirected Walking in Virtual Reality</h3>
    <div class="research-authors">Project team: Deep Pandey · Bidur Wagle · Ashu Adhikari · Sujal Dhungana · Supervisor: Prof. Dr. Shashidhar Ram Joshi</div>
    <p>How can someone walk through a virtual world larger than the room around them? As the main developer, I implemented translation, rotation, and curvature gains in Unity to subtly change the relationship between physical and virtual movement.</p>
    <p>We combined the techniques in a playable HTC Vive game and studied participants' navigation and experience. The thesis grew alongside my work at Paracosma.</p>
    <a href="https://drive.google.com/file/d/1bM9cF2aNjRDZ9Yr5If0ON40mX6NfcCc7/view?usp=sharing">Read the project report ↗</a> <span aria-hidden="true"> · </span> <a href="{{ '/projects/undergraduate/' | relative_url }}#redirected-walking">See the project ↗</a>
  </div>
</section>
