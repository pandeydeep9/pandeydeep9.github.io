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
.student-award { display: inline-block; margin: .3rem 0; padding: .32rem .72rem; border-radius: 100px; background: #f4e7aa; color: #704c00; letter-spacing: 0; text-transform: none; }
.student-project p { max-width: 740px; margin-bottom: .9rem; }
.student-feature { display: grid; grid-template-columns: minmax(0, 1.5fr) minmax(240px, 1fr); gap: 1.3rem; align-items: start; }
.student-feature > div:first-child { min-width: 0; }
.student-photo, .student-certificate { margin: .8rem 0 0; }
.student-photo img { width: 100%; border-radius: 12px; }
.student-logo { margin: 1rem 0 0; padding: 1rem; background: #fff; border: 1px solid var(--global-divider-color); border-radius: 14px; text-align: center; }
.student-logo img { display: block; width: 100%; height: 210px; object-fit: cover; object-position: center 52%; border-radius: 8px; }
.student-logo figcaption { font-size: .8rem; color: #666; margin-top: .35rem; }
.student-photo figcaption, .student-certificate figcaption, .student-gallery figcaption { color: var(--global-text-color-light); font-size: .8rem; padding-top: .45rem; }
.student-certificate { border: 1px solid var(--global-divider-color); border-radius: 12px; overflow: hidden; background: #f6f2ff; }
.student-certificate a { display: block; }
.student-certificate img { display: block; width: 100%; max-height: 235px; object-fit: contain; }
.student-certificate figcaption { padding: .55rem .75rem; background: var(--global-card-bg-color); }
.student-awards { display: grid; grid-template-columns: repeat(2, minmax(0,1fr)); gap: .7rem; }
.student-gallery-heading { display: flex; align-items: center; justify-content: space-between; gap: 1rem; margin-top: 1.7rem; }
.student-gallery-heading h3 { font-size: 1rem; margin: 0; }
.student-gallery-controls { display: flex; gap: .45rem; }
.student-gallery-controls button { width: 2.3rem; height: 2.3rem; border: 1px solid var(--global-divider-color); border-radius: 50%; background: var(--global-card-bg-color); color: var(--accent); font-size: 1.4rem; line-height: 1; cursor: pointer; }
.student-gallery-controls button:hover { background: var(--accent); color: white; }
.student-gallery { display: flex; gap: .85rem; margin: .8rem 0 0; overflow-x: auto; scroll-snap-type: x mandatory; scroll-behavior: smooth; scrollbar-width: thin; padding: .25rem .2rem 1rem; }
.student-gallery figure { margin: 0; flex: 0 0 clamp(160px, 24%, 215px); scroll-snap-align: start; }
.student-gallery img { display: block; width: 100%; aspect-ratio: 9 / 15; object-fit: cover; object-position: top; border: 1px solid var(--global-divider-color); border-radius: 12px; box-shadow: 0 8px 18px rgba(20,20,45,.12); }
[data-zoomable] { cursor: zoom-in; transition: transform .25s ease, filter .25s ease; }
[data-zoomable]:hover { transform: translateY(-3px); filter: brightness(.97); }
[data-zoomable]:focus-visible { outline: 3px solid #7652d2; outline-offset: 3px; }
.student-team { margin: 1.2rem 0 .3rem; }
.student-team h3 { margin: 0 0 .55rem; color: var(--accent); font-size: .82rem; font-weight: 700; letter-spacing: .05em; text-transform: uppercase; }
.student-team ul { display: flex; flex-wrap: wrap; gap: .45rem .6rem; padding: 0; margin: 0; list-style: none; }
.student-team li { border: 1px solid var(--global-divider-color); background: var(--global-bg-color); border-radius: 100px; padding: .32rem .65rem; font-size: .84rem; line-height: 1.35; }
.student-team li::before { content: "•"; color: var(--accent); font-weight: 700; margin-right: .4rem; }
.student-team .student-lead { border-color: var(--accent); }
.student-team .student-lead strong { color: var(--accent); font-size: .75rem; margin-left: .25rem; }
.medium-zoom-overlay { z-index: 2000; }
.medium-zoom-image--opened { z-index: 2001; }
@media (max-width: 700px) { .student-feature { grid-template-columns: 1fr; } .student-gallery figure { flex-basis: min(58vw, 210px); } }
@media (prefers-reduced-motion: reduce) { .student-gallery { scroll-behavior: auto; } [data-zoomable] { transition: none; } }
</style>

<p class="student-intro">Before my research career, I enjoyed building things with a purpose. These undergraduate projects in Nepal grew from ideas about food and culture, language preservation, playful learning, and conserving resources.</p>

<section class="student-project student-project-featured">
  <div class="student-feature">
    <div>
  <div class="student-meta">2016 · Android app<br><span class="student-award">★ Second place · TechBihani 2.0</span></div>
  <h2>Food Tours Nepal</h2>
  <p>Built an app for exploring Nepal through its food, from individual dishes and regional cuisines to nearby places to eat. The prototype brought together food guides, community and recommendation views, and a map with filters for distance, price, and rating.</p>
  <div class="student-team"><h3>Team</h3><ul><li class="student-lead">Deep Pandey <strong>Lead</strong></li><li>Kushal Pokherel</li><li>Drishya Chhetri</li><li>Ayush Kafle</li><li>Aashish Neupane</li><li>Pranjal Dhakal</li><li>Bidur Khanal</li></ul></div>
  <div class="student-awards">
    <figure class="student-certificate"><img src="{{ '/assets/img/undergrad/food-tour-acem-2016.jpg' | relative_url }}" alt="TechBihani 2.0 certificate for second place in the software competition" loading="lazy" data-zoomable tabindex="0"><figcaption>Second place · TechBihani 2.0</figcaption></figure>
    <figure class="student-certificate"><img src="{{ '/assets/img/undergrad/food-tour-yomari-2016.jpg' | relative_url }}" alt="Yomari Code Camp 2016 participation certificate" loading="lazy" data-zoomable tabindex="0"><figcaption>Yomari Code Camp · 2016</figcaption></figure>
  </div>
    </div>
    <div><figure class="student-photo"><img src="{{ '/assets/img/undergrad/food-tour-team.jpg' | relative_url }}" alt="Deep Shankar Pandey and teammates wearing medals in a 2016 group photo" loading="lazy" data-zoomable tabindex="0"><figcaption>With teammates in 2016</figcaption></figure>
      <figure class="student-logo"><img src="{{ '/assets/img/undergrad/food-tour-logo.jpg' | relative_url }}" alt="Food Tours Nepal original app logo" loading="lazy" data-zoomable tabindex="0"><figcaption>The original Food Tours Nepal logo</figcaption></figure>
    </div>
  </div>
  <div class="student-gallery-heading"><h3>Inside the app</h3><div class="student-gallery-controls"><button type="button" data-gallery-step="-1" aria-controls="food-tour-gallery" aria-label="Previous app screenshot">‹</button><button type="button" data-gallery-step="1" aria-controls="food-tour-gallery" aria-label="Next app screenshot">›</button></div></div>
  <div class="student-gallery" id="food-tour-gallery" role="group" aria-label="Food Tours Nepal app screenshots">
    <figure><img src="{{ '/assets/img/undergrad/food-tour-logo.jpg' | relative_url }}" alt="Food Tours Nepal app splash screen with its logo" loading="lazy" data-zoomable tabindex="0"><figcaption>App splash screen</figcaption></figure>
    <figure><img src="{{ '/assets/img/undergrad/food-tour-foods.jpg' | relative_url }}" alt="Food Tours Nepal app screen showing a grid of Nepali foods" loading="lazy" data-zoomable tabindex="0"><figcaption>Explore dishes</figcaption></figure>
    <figure><img src="{{ '/assets/img/undergrad/food-tour-map.jpg' | relative_url }}" alt="Food Tours Nepal map screen with nearby food places" loading="lazy" data-zoomable tabindex="0"><figcaption>Find nearby places</figcaption></figure>
    <figure><img src="{{ '/assets/img/undergrad/food-tour-cuisines.jpg' | relative_url }}" alt="Food Tours Nepal app screen showing regional cuisines" loading="lazy" data-zoomable tabindex="0"><figcaption>Discover cuisines</figcaption></figure>
    <figure><img src="{{ '/assets/img/undergrad/food-tour-dish.jpg' | relative_url }}" alt="Food Tours Nepal Momo screen with a photo, map button, and dish information" loading="lazy" data-zoomable tabindex="0"><figcaption>Explore Momo</figcaption></figure>
  </div>
</section>

<script>
document.addEventListener('DOMContentLoaded', function () {
  var gallery = document.getElementById('food-tour-gallery');
  document.querySelectorAll('[data-gallery-step]').forEach(function (button) {
    button.addEventListener('click', function () {
      var card = gallery.querySelector('figure');
      var gap = parseFloat(getComputedStyle(gallery).gap) || 0;
      gallery.scrollBy({ left: Number(button.dataset.galleryStep) * (card.getBoundingClientRect().width + gap), behavior: 'smooth' });
    });
  });
});
</script>

<section class="student-project">
  <div class="student-feature"><div>
    <div class="student-meta">2016 · Individual coding competition<br><span class="student-award">★ First place · ACEM Code Camp</span></div>
    <h2>ACEM Code Camp</h2>
    <p>Competed individually in the Code Camp coding challenge at TechBihani 2.0.</p>
    <div class="student-team"><h3>Participation</h3><ul><li class="student-lead">Deep Pandey <strong>Solo competitor</strong></li></ul></div>
  </div><figure class="student-certificate"><img src="{{ '/assets/img/undergrad/acem-code-camp-2016.jpg' | relative_url }}" alt="ACEM TechBihani 2.0 certificate awarding first place in Code Camp" loading="lazy" data-zoomable tabindex="0"><figcaption>First place · ACEM Code Camp, January 2016</figcaption></figure></div>
</section>

<section class="student-project">
  <div class="student-feature"><div>
    <div class="student-meta">May–September 2016 · E&amp;T–TU collaboration · Internship</div>
    <h2>Blockchain Application</h2>
    <p>Led development of a blockchain application during an E&amp;T–Tribhuvan University collaboration internship. Wrote its Python implementation, including the customer-facing interface and core application logic.</p>
    <div class="student-team"><h3>Team</h3><ul><li class="student-lead">Deep Pandey <strong>Lead developer</strong></li><li>Diman Maharjan</li><li>Pooja Khanal</li><li>Prashuna Dahal</li></ul></div>
  </div><figure class="student-certificate"><img src="{{ '/assets/img/undergrad/blockchain-internship-2016.jpg' | relative_url }}" alt="E and T–Tribhuvan University collaboration internship certificate for the Block Chain Application project, May to September 2016" loading="lazy" data-zoomable tabindex="0"><figcaption>Blockchain application · E&amp;T–TU internship, 2016</figcaption></figure></div>
</section>

<section class="student-project">
  <div class="student-feature"><div>
  <div class="student-meta">2015 · Android app<br><span class="student-award">★ Best Idea · Yomari Code Camp</span></div>
  <h2>Lingo App</h2>
  <p>Served as the main developer of an app designed to help people learn endangered languages in Nepal and support their preservation. The idea began at a LOCUS 2015 hackathon and was refined for Yomari Code Camp.</p>
  <div class="student-team"><h3>Team</h3><ul><li>Deep Pandey <strong>Main developer</strong></li><li class="student-lead">Kushal Pokherel <strong>Lead</strong></li><li>Drishya Chhetri</li></ul></div>
  </div><figure class="student-certificate"><img src="{{ '/assets/img/undergrad/lingo-locus-2015.jpg' | relative_url }}" alt="LOCUS 2015 hackathon participation certificate" loading="lazy" data-zoomable tabindex="0"><figcaption>LOCUS 2015 · Hackathon</figcaption></figure></div>
</section>

<section class="student-project">
  <div class="student-feature"><div>
  <div class="student-meta">2014 · C# and Windows 8.1<br><span class="student-award">★ Third place · Windows 8.1 Dev Camp</span></div>
  <h2>Save the Tree</h2>
  <p>Led the team and programmed a game that introduced children to nature conservation through play. Presented it at the Windows 8.1 Dev Camp at Pulchowk Campus.</p>
  <div class="student-team"><h3>Team</h3><ul><li class="student-lead">Deep Pandey <strong>Lead</strong></li><li>Krishna Chapagain</li><li>Giru Pandey</li></ul></div>
  </div><figure class="student-certificate"><img src="{{ '/assets/img/undergrad/save-the-tree-2014.jpg' | relative_url }}" alt="Windows 8.1 Dev Camp third-place certificate" loading="lazy" data-zoomable tabindex="0"><figcaption>Third place · Windows 8.1 Dev Camp</figcaption></figure></div>
</section>

<section class="student-project">
  <div class="student-feature"><div>
  <div class="student-meta">2014 · Arduino &amp; breadboard prototype · LOCUS</div>
  <h2>Home Automator</h2>
  <p>Built an Arduino and breadboard proof of concept that senses when a water tank is full and switches off the pump, helping prevent overflow and unnecessary electricity use.</p>
  <div class="student-team"><h3>Team</h3><ul><li class="student-lead">Deep Pandey <strong>Lead</strong></li><li>Bidur Wagle</li></ul></div>
  </div><figure class="student-certificate"><img src="{{ '/assets/img/undergrad/water-tank-locus-2014.jpg' | relative_url }}" alt="LOCUS 2014 hardware competition participation certificate" loading="lazy" data-zoomable tabindex="0"><figcaption>LOCUS 2014 · Hardware competition</figcaption></figure></div>
</section>

<section class="student-project">
  <div class="student-feature"><div>
  <div class="student-meta">Undergraduate project · C programming</div>
  <h2>Fly The Plane</h2>
  <p>Developed a single-player game in C: guide a plane to its destination within a time limit while avoiding obstacles. Presented it at a student C project competition at Pulchowk Campus.</p>
  <div class="student-team"><h3>Team</h3><ul><li class="student-lead">Deep Pandey <strong>Lead</strong></li><li>Bidur Khanal</li><li>Aashish Bhandari</li></ul></div>
  </div><figure class="student-certificate"><img src="{{ '/assets/img/undergrad/plane-game-c-competition.jpg' | relative_url }}" alt="C project competition participation certificate" loading="lazy" data-zoomable tabindex="0"><figcaption>C project competition · Pulchowk Campus</figcaption></figure></div>
</section>
