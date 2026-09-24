---
layout: page
title: Projects
permalink: /projects/undergraduate/
description: Undergraduate projects in software, culture, and sustainability.
nav: true
nav_order: 3
---

<style>
.student-intro { max-width: 760px; margin: 0 0 2rem; font-size: 1.1rem; line-height: 1.65; }
.student-project { --accent: #6941c6; border: 1px solid var(--global-divider-color); border-radius: 18px; padding: clamp(1.2rem, 3vw, 2rem); margin: 1.6rem 0; background: var(--global-card-bg-color); box-shadow: 0 12px 30px rgba(35,25,76,.07); }
.student-project:nth-of-type(3n) { --accent: #13877b; }
.student-project:nth-of-type(4n) { --accent: #b66a25; }
.student-project h2 { margin: .25rem 0 .55rem; font-size: 1.55rem; }
.student-meta { color: var(--accent); font-size: .83rem; font-weight: 700; letter-spacing: .025em; text-transform: uppercase; }
.student-project p { max-width: 740px; margin-bottom: .9rem; }
.student-feature { display: grid; grid-template-columns: minmax(0, 1.5fr) minmax(240px, 1fr); gap: 1.3rem; align-items: start; }
.student-feature > div:first-child { min-width: 0; }
.student-photo, .student-certificate { margin: .8rem 0 0; }
.student-photo img { width: 100%; border-radius: 12px; }
.student-photo figcaption, .student-certificate figcaption, .student-gallery figcaption { color: var(--global-text-color-light); font-size: .8rem; padding-top: .45rem; }
.student-certificate { border: 1px solid var(--global-divider-color); border-radius: 12px; overflow: hidden; background: #f6f2ff; }
.student-certificate a { display: block; }
.student-certificate img { display: block; width: 100%; max-height: 235px; object-fit: contain; }
.student-certificate figcaption { padding: .55rem .75rem; background: var(--global-card-bg-color); }
.student-awards { display: grid; grid-template-columns: repeat(2, minmax(0,1fr)); gap: .7rem; }
.student-gallery { display: grid; grid-template-columns: repeat(4, minmax(0,1fr)); gap: .8rem; margin: 1.5rem 0 0; }
.student-gallery figure { margin: 0; }
.student-gallery img { display: block; width: 100%; aspect-ratio: 9 / 15; object-fit: cover; object-position: top; border: 1px solid var(--global-divider-color); border-radius: 12px; box-shadow: 0 8px 18px rgba(20,20,45,.12); }
.student-gallery a:hover img, .student-certificate a:hover img { filter: brightness(.95); }
@media (max-width: 700px) { .student-feature { grid-template-columns: 1fr; } .student-gallery { grid-template-columns: repeat(2, minmax(0,1fr)); } }
</style>

<p class="student-intro">Before my research career, I enjoyed building things with a purpose. These undergraduate projects in Nepal grew from ideas about food and culture, language preservation, playful learning, and conserving resources.</p>

<section class="student-project student-project-featured">
  <div class="student-feature">
    <div>
  <div class="student-meta">2016 · Android app · Second place, TechBihani 2.0</div>
  <h2>Food Tours Nepal</h2>
  <p>Built an app for exploring Nepal through its food, from individual dishes and regional cuisines to nearby places to eat. The prototype brought together food guides, community and recommendation views, and a map with filters for distance, price, and rating. Presented at Yomari Code Camp and earned second place in the TechBihani 2.0 software competition.</p>
  <div class="student-awards">
    <figure class="student-certificate"><a href="{{ '/assets/img/undergrad/food-tour-acem-2016.jpg' | relative_url }}"><img src="{{ '/assets/img/undergrad/food-tour-acem-2016.jpg' | relative_url }}" alt="TechBihani 2.0 certificate for second place in the software competition" loading="lazy"></a><figcaption>Second place · TechBihani 2.0</figcaption></figure>
    <figure class="student-certificate"><a href="{{ '/assets/img/undergrad/food-tour-yomari-2016.jpg' | relative_url }}"><img src="{{ '/assets/img/undergrad/food-tour-yomari-2016.jpg' | relative_url }}" alt="Yomari Code Camp 2016 participation certificate" loading="lazy"></a><figcaption>Yomari Code Camp · 2016</figcaption></figure>
  </div>
    </div>
    <figure class="student-photo"><a href="{{ '/assets/img/undergrad/food-tour-team.jpg' | relative_url }}"><img src="{{ '/assets/img/undergrad/food-tour-team.jpg' | relative_url }}" alt="Deep Shankar Pandey and teammates wearing medals in a 2016 group photo" loading="lazy"></a><figcaption>With teammates in 2016</figcaption></figure>
  </div>
  <div class="student-gallery">
    <figure><a href="{{ '/assets/img/undergrad/food-tour-foods.jpg' | relative_url }}"><img src="{{ '/assets/img/undergrad/food-tour-foods.jpg' | relative_url }}" alt="Food Tours Nepal app screen showing a grid of Nepali foods" loading="lazy"></a><figcaption>Explore dishes</figcaption></figure>
    <figure><a href="{{ '/assets/img/undergrad/food-tour-cuisines.jpg' | relative_url }}"><img src="{{ '/assets/img/undergrad/food-tour-cuisines.jpg' | relative_url }}" alt="Food Tours Nepal app screen showing regional cuisines" loading="lazy"></a><figcaption>Discover cuisines</figcaption></figure>
    <figure><a href="{{ '/assets/img/undergrad/food-tour-dish.jpg' | relative_url }}"><img src="{{ '/assets/img/undergrad/food-tour-dish.jpg' | relative_url }}" alt="Food Tours Nepal app screen with information about momo" loading="lazy"></a><figcaption>Learn about food</figcaption></figure>
    <figure><a href="{{ '/assets/img/undergrad/food-tour-map.jpg' | relative_url }}"><img src="{{ '/assets/img/undergrad/food-tour-map.jpg' | relative_url }}" alt="Food Tours Nepal map screen with nearby food places" loading="lazy"></a><figcaption>Find nearby places</figcaption></figure>
  </div>
</section>

<section class="student-project">
  <div class="student-feature"><div>
  <div class="student-meta">2015 · Android app · Best Idea, Yomari Code Camp</div>
  <h2>Lingo App</h2>
  <p>Led development of an app designed to help people learn endangered languages in Nepal and support their preservation. The idea began at a LOCUS 2015 hackathon and was refined for Yomari Code Camp, where it won Best Idea.</p>
  </div><figure class="student-certificate"><a href="{{ '/assets/img/undergrad/lingo-locus-2015.jpg' | relative_url }}"><img src="{{ '/assets/img/undergrad/lingo-locus-2015.jpg' | relative_url }}" alt="LOCUS 2015 hackathon participation certificate" loading="lazy"></a><figcaption>LOCUS 2015 · Hackathon</figcaption></figure></div>
</section>

<section class="student-project">
  <div class="student-feature"><div>
  <div class="student-meta">2014 · C# and Windows 8.1 · Third place</div>
  <h2>Save the Tree</h2>
  <p>Led the team and programmed a game that introduced children to nature conservation through play. Won third place at the Windows 8.1 Dev Camp at Pulchowk Campus.</p>
  </div><figure class="student-certificate"><a href="{{ '/assets/img/undergrad/save-the-tree-2014.jpg' | relative_url }}"><img src="{{ '/assets/img/undergrad/save-the-tree-2014.jpg' | relative_url }}" alt="Windows 8.1 Dev Camp third-place certificate" loading="lazy"></a><figcaption>Third place · Windows 8.1 Dev Camp</figcaption></figure></div>
</section>

<section class="student-project">
  <div class="student-feature"><div>
  <div class="student-meta">2014 · Hardware prototype · LOCUS</div>
  <h2>Home Automator</h2>
  <p>Built a proof of concept that senses when a water tank is full and switches off the pump, helping prevent overflow and unnecessary electricity use.</p>
  </div><figure class="student-certificate"><a href="{{ '/assets/img/undergrad/water-tank-locus-2014.jpg' | relative_url }}"><img src="{{ '/assets/img/undergrad/water-tank-locus-2014.jpg' | relative_url }}" alt="LOCUS 2014 hardware competition participation certificate" loading="lazy"></a><figcaption>LOCUS 2014 · Hardware competition</figcaption></figure></div>
</section>

<section class="student-project">
  <div class="student-feature"><div>
  <div class="student-meta">Undergraduate project · C programming</div>
  <h2>2D Plane Game</h2>
  <p>Developed a single-player game in C: guide a plane to its destination within a time limit while avoiding obstacles. Presented it at a student C project competition at Pulchowk Campus.</p>
  </div><figure class="student-certificate"><a href="{{ '/assets/img/undergrad/plane-game-c-competition.jpg' | relative_url }}"><img src="{{ '/assets/img/undergrad/plane-game-c-competition.jpg' | relative_url }}" alt="C project competition participation certificate" loading="lazy"></a><figcaption>C project competition · Pulchowk Campus</figcaption></figure></div>
</section>
