---
layout: page
title: Projects
permalink: /projects/undergraduate/
description: Projects in virtual reality, games, graphics, and software.
nav: true
nav_order: 3
---

<style>
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
.student-photo figcaption, .student-certificate figcaption, .student-gallery figcaption { color: var(--global-text-color-light); font-size: .8rem; padding-top: .45rem; }
.student-certificate { border: 1px solid var(--global-divider-color); border-radius: 12px; overflow: hidden; background: #f6f2ff; }
.student-certificate a { display: block; }
.student-certificate img { display: block; width: 100%; max-height: 235px; object-fit: contain; }
.student-certificate figcaption { padding: .55rem .75rem; background: var(--global-card-bg-color); }
.student-awards { display: grid; grid-template-columns: repeat(2, minmax(0,1fr)); gap: .7rem; }
.student-food-tour .student-feature { grid-template-columns: minmax(0, 1fr) minmax(0, 1fr); }
.student-food-tour .student-awards { margin-top: .85rem; }
.student-food-tour .student-certificate img { max-height: 170px; }
.student-gallery-heading { display: flex; align-items: center; justify-content: space-between; gap: 1rem; margin-top: 1.7rem; }
.student-gallery-heading h3 { font-size: 1rem; margin: 0; }
.student-gallery-controls { display: flex; gap: .45rem; }
.student-gallery-controls button { width: 2.3rem; height: 2.3rem; border: 1px solid var(--global-divider-color); border-radius: 50%; background: var(--global-card-bg-color); color: var(--accent); font-size: 1.4rem; line-height: 1; cursor: pointer; }
.student-gallery-controls button:hover { background: var(--accent); color: white; }
.student-gallery { display: flex; gap: .85rem; margin: .8rem 0 0; overflow-x: auto; scroll-snap-type: x mandatory; scroll-behavior: smooth; scrollbar-width: thin; padding: .25rem .2rem 1rem; }
.student-gallery figure { margin: 0; flex: 0 0 clamp(160px, 24%, 215px); scroll-snap-align: start; }
.student-gallery img { display: block; width: 100%; aspect-ratio: 9 / 15; object-fit: cover; object-position: top; border: 1px solid var(--global-divider-color); border-radius: 12px; box-shadow: 0 8px 18px rgba(20,20,45,.12); }
.student-gallery .student-splash img { object-fit: contain; background: white; }
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
.student-links { display: flex; flex-wrap: wrap; gap: .55rem; margin: 1rem 0; }
.student-links a { display: inline-block; border: 1px solid var(--accent); border-radius: 999px; padding: .45rem .85rem; color: var(--accent); font-size: .88rem; font-weight: 650; text-decoration: none; }
.student-links a:hover, .student-links a:focus-visible { background: var(--accent); color: white; text-decoration: none; }
.student-wide-image { display: block; width: 100%; max-height: 420px; object-fit: cover; object-position: center; border-radius: 12px; }
.student-project-gallery { display: grid; grid-template-columns: repeat(2, minmax(0, 1fr)); gap: .85rem; margin-top: 1.2rem; }
.student-project-gallery figure { margin: 0; }
.student-project-gallery img { display: block; width: 100%; height: auto; aspect-ratio: 16 / 9; object-fit: contain; background: #191923; border-radius: 12px; }
.student-jungle-gallery { display: flex; gap: .85rem; overflow-x: auto; scroll-snap-type: x mandatory; scroll-behavior: smooth; scrollbar-width: thin; padding: .25rem .1rem 1rem; }
.student-jungle-gallery figure { flex: 0 0 clamp(275px, 48%, 530px); scroll-snap-align: start; }
.student-jungle-gallery img { width: 100%; height: 280px; aspect-ratio: auto; object-fit: contain; background: #e4fbff; }
.student-vr-links { gap: .65rem; margin: .85rem 0 1.2rem; }
.student-vr-links a { padding: .45rem .85rem; border: 1px solid #91cfac; border-radius: 999px; background: #e8f6ee; color: #17613d; font-weight: 600; }
.student-vr-links a:hover, .student-vr-links a:focus-visible { border-color: #17613d; background: #17613d; color: #fff; text-decoration: none; }
.student-vr-links a:focus-visible { outline: 2px solid #17613d; outline-offset: 2px; }
.student-vr-credit { margin: .8rem 0 0; font-size: .78rem; color: var(--global-text-color-light); }
.medium-zoom-overlay { z-index: 2000; }
.medium-zoom-image--opened { z-index: 2001; }
@media (max-width: 700px) { .student-feature, .student-food-tour .student-feature, .student-project-gallery { grid-template-columns: 1fr; } .student-gallery figure { flex-basis: min(58vw, 210px); } .student-jungle-gallery figure { flex-basis: min(85vw, 430px); } .student-jungle-gallery img { height: 230px; } }
@media (prefers-reduced-motion: reduce) { .student-gallery, .student-jungle-gallery { scroll-behavior: auto; } [data-zoomable] { transition: none; } }
</style>

<section class="student-project student-project-featured" id="redirected-walking">
  <div class="student-meta">2017 · Undergraduate major project · Virtual reality</div>
  <h2>Redirected Walking in Virtual Reality</h2>
  <p>I implemented translational, rotational, and curvature gains in Unity to let players explore a virtual world larger than their physical space. We integrated the techniques into an HTC Vive game and evaluated them with participants.</p>
  <div class="student-links student-vr-links"><a href="https://www.youtube.com/watch?v=_bluD007JiE" target="_blank" rel="noopener noreferrer">Game demo ↗</a><a href="https://drive.google.com/file/d/1bM9cF2aNjRDZ9Yr5If0ON40mX6NfcCc7/view?usp=sharing" target="_blank" rel="noopener noreferrer">Project report ↗</a><a href="https://github.com/pandeydeep9/Mazes" target="_blank" rel="noopener noreferrer">Maze algorithms ↗</a></div>
  <div class="student-team"><h3>Team</h3><ul><li class="student-lead">Deep Pandey <strong>Main developer</strong></li><li>Bidur Wagle</li><li>Ashu Adhikari</li><li>Sujal Dhungana</li></ul></div>
  <div class="student-project-gallery">
    <figure class="student-photo"><img src="{{ '/assets/img/undergrad/vr-game-one-enemy-2017.jpg' | relative_url }}" alt="Unity VR game scene with one skeletal enemy in a stone room" loading="lazy" data-zoomable tabindex="0"><figcaption>VR game environment · one enemy</figcaption></figure>
    <figure class="student-photo"><img src="{{ '/assets/img/undergrad/vr-game-two-enemies-2017.jpg' | relative_url }}" alt="Unity VR game scene with two skeletal enemies in a stone room" loading="lazy" data-zoomable tabindex="0"><figcaption>VR game environment · two enemies</figcaption></figure>
  </div>
  <p class="student-vr-credit">With thanks to Ken Ehrhart and Sujit Jha at Paracosma, and project supervisor Prof. Dr. Shashidhar Ram Joshi.</p>
</section>

<section class="student-project" id="graphics-project">
  <div class="student-meta">Third year · Computer graphics project</div>
  <h2>3D Graphics Project</h2>
  <p>Led a third-year computer graphics project to build a navigable 3D game environment with colorful corridors and geometric characters.</p>
  <div class="student-links"><a href="https://github.com/pandeydeep9/GraphicsProject" target="_blank" rel="noopener noreferrer">View project on GitHub ↗</a></div>
  <div class="student-team"><h3>Team</h3><ul><li class="student-lead">Deep Pandey <strong>Lead</strong></li><li>Giru Pandey</li><li>Manish Basnet</li></ul></div>
  <div class="student-project-gallery">
    <figure class="student-photo"><img src="{{ '/assets/img/undergrad/graphics-corridor-2017.png' | relative_url }}" alt="Original 3D graphics game screenshot of a colorful corridor viewed from above" loading="lazy" data-zoomable tabindex="0"><figcaption>Colorful 3D corridor</figcaption></figure>
    <figure class="student-photo"><img src="{{ '/assets/img/undergrad/graphics-character-2017.png' | relative_url }}" alt="Original 3D graphics game screenshot of a geometric character in a colorful corridor" loading="lazy" data-zoomable tabindex="0"><figcaption>Character and corridor in the game</figcaption></figure>
  </div>
</section>

<section class="student-project" id="locus-2017">
  <div class="student-feature"><div>
    <div class="student-meta">2017 · LOCUS Hack-A-Week</div>
    <h2>3D Mystery Survival Game</h2>
    <p>Led a team at LOCUS Hack-A-Week to prototype a multi-level 3D mystery survival game.</p>
    <div class="student-team"><h3>Team</h3><ul><li class="student-lead">Deep Pandey <strong>Lead</strong></li><li>Bidur Wagle</li><li>Aashish Neupane</li><li>Sameer Gopali</li></ul></div>
  </div><figure class="student-certificate"><img src="{{ '/assets/img/undergrad/locus-hack-a-week-2017.jpg' | relative_url }}" alt="LOCUS Hack-A-Week 2017 participation certificate for Deep Shankar Pandey" loading="lazy" data-zoomable tabindex="0"><figcaption>LOCUS 2017 · Hack-A-Week</figcaption></figure></div>
  <div class="student-project-gallery">
    <figure class="student-photo"><img src="{{ '/assets/img/undergrad/mystery-survival-blue-2017.png' | relative_url }}" alt="Blue and purple 3D game scene with illuminated paths and geometric platforms" loading="lazy" data-zoomable tabindex="0"><figcaption>Blue level prototype</figcaption></figure>
    <figure class="student-photo"><img src="{{ '/assets/img/undergrad/mystery-survival-red-2017.png' | relative_url }}" alt="Red 3D game scene with maze-like platforms and illuminated paths" loading="lazy" data-zoomable tabindex="0"><figcaption>Red level prototype</figcaption></figure>
  </div>
</section>



<section class="student-project student-project-featured student-food-tour">
  <div class="student-feature">
    <div>
  <div class="student-meta">2016 · Android app<br><span class="student-award">★ Second place · TechBihani 2.0</span></div>
  <h2>Food Tours Nepal</h2>
  <p>Built an app for exploring Nepal through its food, from individual dishes and regional cuisines to nearby places to eat. The prototype brought together food guides, community and recommendation views, and a map with filters for distance, price, and rating.</p>
  <div class="student-team"><h3>Team</h3><ul><li class="student-lead">Deep Pandey <strong>Lead</strong></li><li>Kushal Pokherel</li><li>Drishya Chhetri</li><li>Ayush Kafle</li><li>Aashish Neupane</li><li>Pranjal Dhakal</li><li>Bidur Khanal</li></ul></div>
    </div>
    <div><figure class="student-photo"><img src="{{ '/assets/img/undergrad/food-tour-team.jpg' | relative_url }}" alt="Deep Shankar Pandey and teammates wearing medals in a 2016 group photo" loading="lazy" data-zoomable tabindex="0"><figcaption>With teammates in 2016</figcaption></figure>
      <div class="student-awards">
        <figure class="student-certificate"><img src="{{ '/assets/img/undergrad/food-tour-acem-2016.jpg' | relative_url }}" alt="TechBihani 2.0 certificate for second place in the software competition" loading="lazy" data-zoomable tabindex="0"><figcaption>Second place · TechBihani 2.0</figcaption></figure>
        <figure class="student-certificate"><img src="{{ '/assets/img/undergrad/food-tour-yomari-2016.jpg' | relative_url }}" alt="Yomari Code Camp 2016 participation certificate" loading="lazy" data-zoomable tabindex="0"><figcaption>Yomari Code Camp · 2016</figcaption></figure>
      </div>
    </div>
  </div>
  <div class="student-gallery-heading"><h3>Inside the app</h3><div class="student-gallery-controls"><button type="button" data-gallery-step="-1" aria-controls="food-tour-gallery" aria-label="Previous app screenshot">‹</button><button type="button" data-gallery-step="1" aria-controls="food-tour-gallery" aria-label="Next app screenshot">›</button></div></div>
  <div class="student-gallery" id="food-tour-gallery" role="group" aria-label="Food Tours Nepal app screenshots">
    <figure class="student-splash"><img src="{{ '/assets/img/undergrad/food-tour-logo.jpg' | relative_url }}" alt="Food Tours Nepal app splash screen with its logo" loading="lazy"><figcaption>App splash screen</figcaption></figure>
    <figure><img src="{{ '/assets/img/undergrad/food-tour-foods.jpg' | relative_url }}" alt="Food Tours Nepal app screen showing a grid of Nepali foods" loading="lazy" data-zoomable tabindex="0"><figcaption>Explore dishes</figcaption></figure>
    <figure><img src="{{ '/assets/img/undergrad/food-tour-map.jpg' | relative_url }}" alt="Food Tours Nepal map screen with nearby food places" loading="lazy" data-zoomable tabindex="0"><figcaption>Find nearby places</figcaption></figure>
    <figure><img src="{{ '/assets/img/undergrad/food-tour-cuisines.jpg' | relative_url }}" alt="Food Tours Nepal app screen showing regional cuisines" loading="lazy" data-zoomable tabindex="0"><figcaption>Discover cuisines</figcaption></figure>
    <figure><img src="{{ '/assets/img/undergrad/food-tour-dish.jpg' | relative_url }}" alt="Food Tours Nepal Momo screen with a photo, map button, and dish information" loading="lazy" data-zoomable tabindex="0"><figcaption>Explore Momo</figcaption></figure>
  </div>
</section>

<script>
document.addEventListener('DOMContentLoaded', function () {
  document.querySelectorAll('[data-gallery-step]').forEach(function (button) {
    button.addEventListener('click', function () {
      var gallery = document.getElementById(button.getAttribute('aria-controls'));
      var card = gallery.querySelector('figure');
      var gap = parseFloat(getComputedStyle(gallery).gap) || 0;
      gallery.scrollBy({ left: Number(button.dataset.galleryStep) * (card.getBoundingClientRect().width + gap), behavior: window.matchMedia('(prefers-reduced-motion: reduce)').matches ? 'auto' : 'smooth' });
    });
  });
});
</script>

<section class="student-project">
  <div class="student-feature"><div>
    <div class="student-meta">2016 · Individual coding competition<br><span class="student-award">★ First place · ACEM Code Camp</span></div>
    <h2>ACEM Code Camp</h2>
    <p>Won the individual coding competition by completing all of its programming challenges first.</p>
    <div class="student-team"><h3>Participant</h3><ul><li class="student-lead">Deep Pandey <strong>Winner</strong></li></ul></div>
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

<section class="student-project" id="jungle-run">
  <div class="student-meta">2015 · C++ · Object-oriented programming</div>
  <h2>Jungle Run</h2>
  <p>Led the development of a level-based platform game in C++. Players navigate floating platforms, collect items, and track their score and lives.</p>
  <div class="student-team"><h3>Team</h3><ul><li class="student-lead">Deep Pandey <strong>Lead</strong></li><li>Drishya Chhetri</li><li>Amir Rimal</li><li>Manish Basnet</li></ul></div>
  <div class="student-gallery-heading"><h3>Game screenshots</h3><div class="student-gallery-controls"><button type="button" data-gallery-step="-1" aria-controls="jungle-run-gallery" aria-label="Previous Jungle Run screenshot">‹</button><button type="button" data-gallery-step="1" aria-controls="jungle-run-gallery" aria-label="Next Jungle Run screenshot">›</button></div></div>
  <div class="student-project-gallery student-jungle-gallery" id="jungle-run-gallery" role="group" aria-label="Jungle Run game screenshots">
    <figure class="student-photo"><img src="{{ '/assets/img/undergrad/jungle-run-gameplay-2015.png' | relative_url }}" alt="Jungle Run gameplay with a character jumping between platforms and collecting items" loading="lazy" data-zoomable tabindex="0"><figcaption>Platforming and collectibles</figcaption></figure>
    <figure class="student-photo"><img src="{{ '/assets/img/undergrad/jungle-run-start-2015.png' | relative_url }}" alt="Jungle Run start screen asking the player to enter a name" loading="lazy" data-zoomable tabindex="0"><figcaption>Start screen</figcaption></figure>
    <figure class="student-photo"><img src="{{ '/assets/img/undergrad/jungle-run-level-2015.png' | relative_url }}" alt="Jungle Run gameplay showing another section of the level with the character on a platform" loading="lazy" data-zoomable tabindex="0"><figcaption>Exploring a level</figcaption></figure>
  </div>
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
  <div class="student-meta">2014 · C programming project</div>
  <h2>Fly The Plane</h2>
  <p>Developed a single-player game in C: guide a plane to its destination within a time limit while avoiding obstacles. Presented it at a student C project competition at Pulchowk Campus.</p>
  <div class="student-team"><h3>Team</h3><ul><li class="student-lead">Deep Pandey <strong>Lead</strong></li><li>Bidur Khanal</li><li>Aashish Bhandari</li></ul></div>
  </div><figure class="student-certificate"><img src="{{ '/assets/img/undergrad/plane-game-c-competition.jpg' | relative_url }}" alt="C project competition participation certificate" loading="lazy" data-zoomable tabindex="0"><figcaption>C project competition · Pulchowk Campus</figcaption></figure></div>
</section>

<section class="student-project">
  <div class="student-feature"><div>
  <div class="student-meta">2014 · Arduino &amp; breadboard prototype · LOCUS</div>
  <h2>Home Automator</h2>
  <p>Built an Arduino and breadboard proof of concept that senses when a water tank is full and switches off the pump, helping prevent overflow and unnecessary electricity use.</p>
  <div class="student-team"><h3>Team</h3><ul><li class="student-lead">Deep Pandey <strong>Lead</strong></li><li>Bidur Wagle</li></ul></div>
  </div><figure class="student-certificate"><img src="{{ '/assets/img/undergrad/water-tank-locus-2014.jpg' | relative_url }}" alt="LOCUS 2014 hardware competition participation certificate" loading="lazy" data-zoomable tabindex="0"><figcaption>LOCUS 2014 · Hardware competition</figcaption></figure></div>
</section>
