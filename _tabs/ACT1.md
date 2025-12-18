---
layout: page
icon: fas fa-stream
order: 2
title: ACT 1 - The Eruption  # this is used in sidebar             # custom key Chirpy uses to hide top title
---

<style>
.plot-card {
  max-width: 1100px; 
  margin: 2rem auto;
  padding: 1.2rem 1.4rem;
  border-radius: 1rem;
  border: 1px solid rgba(0,0,0,0.15);
  background: #ffffff;
  box-shadow: 0 4px 14px rgba(0,0,0,0.08);
}

.plot-card iframe {
  width: 100%;
  height: 480px;       /* THIS is the key line */
}

html.dark .plot-card {
  border: 1px solid rgba(180,196,255,0.35);
  background: linear-gradient(135deg, #050814, #0c1024);
  box-shadow: 0 14px 30px rgba(0,0,0,0.4);
}
</style>

<style>
  .question-box {
    background: #0a4fffde;
    background: var(--qbox-bg, #0a4fffde);
    color: white;                          
    padding: 1.2rem 1.6rem;
    border-radius: 12px;
    margin: 1.8rem 0;
    border: 2px solid rgba(255, 255, 255, 0.1);
    box-shadow: 0 6px 18px rgba(0,0,0,0.18);
  }

  .question-box-title {
    font-weight: 800;
    font-size: 1.15rem;
    text-transform: uppercase;
    margin-bottom: 0.6rem;
    letter-spacing: 0.06em;
  }

  html[data-theme="dark"] .question-box {
    --qbox-bg: #003cbd;
    border-color: rgba(255,255,255,0.15);
    box-shadow: 0 8px 24px rgba(0,0,0,0.5);
  }
</style>


<div style="display: flex; align-items: center; gap: 3rem;">
  <h1 style="color:#003c9e; font-size:3rem; font-weight:900; margin:0;">
    The Eruption of Battle Royale
  </h1>

  <img 
    src="/assets/img/img_1/eruption1.png" 
    alt="Scheme" 
    style="width:800px; height:auto; border-radius:24px;
    "
  >
</div>

---

This first act documents how Battle Royale (BR) emerged and rapidly established itself as a core genre within YouTube gaming.  
Rather than assuming BR as an immediate success story, we reconstruct its rise step by step, focusing on *when*, *how fast*, and *at whose expense* this transformation occurred.

We address three main questions:

<div class="question-box">
  <div class="question-box-title">Key Questions</div>
  <ul>
    <li>How did BR uploads and views grow compared to other major gaming genres?</li>
    <li>Which Battle Royale games drove this explosion?</li>
    <li>Did BR expand YouTube gaming overall or primarily reshuffle attention?</li>
  </ul>
</div>


To keep the analysis readable, we focus on the top 7 gaming genres, which capture the vast majority of uploads and views during the period. Smaller genres are excluded as they do not affect the global dynamics and would only clutter the figures.

<div class = "plot-card">
  <iframe
    src="/assets/plots/plots_1/plot_1_1.html"
    loading="lazy"
  ></iframe>
</div>

<h3 style="color:#4f6fd6; font-size:1.5rem; font-weight:500;">Why do we keep only the Top-7 genres (by uploads)?</h3>

- A small number of genres dominate YouTube gaming uploads.  
- The remaining genres contribute extremely little and mostly add noise to time-series analysis.  
- Focusing on the Top-7 genres preserves the structure of the ecosystem while keeping the plots readable.  
- This ranking is stable both over the full period (2014–mid-2019) and within the 2017–2018 BR boom window.

<h3 style="color:#4f6fd6; font-size:1.5rem; font-weight:500;">Why is 2017–2018 our period of interest?</h3>

- The Battle Royale explosion occurs precisely between 2017 and 2018.  
- This boom is driven by the rapid rise of H1Z1, PUBG, and especially Fortnite.  
- Studying this window captures the disruptive impact of BR on YouTube gaming.  
- Confirming that the Top-7 genres remain stable in this period ensures that filtering does not distort the ecosystem’s dynamics.


---

<h2 style="color:#003c9e; font-size:2rem; font-weight:600;">
  Growth of Battle Royale vs other gaming genres
</h2>

We first examine how the volume of Battle Royale uploads and views evolved relative to other dominant gaming genres.  
The objective is not only to detect growth, but to compare rates and persistence: did BR merely spike or did it structurally alter the hierarchy of YouTube gaming?

<h3 style="color:#4f6fd6; font-size:1.5rem; font-weight:500;">Absolute evolution of uploads and views</h3>

Monthly time series show that Battle Royale was nearly absent from YouTube gaming before 2017. At that point, both uploads and views rise abruptly and at a pace unmatched by any other genre.  
By 2018–2019, BR reaches levels comparable to long-established giants such as FPS and Sandbox games, both in production and in audience attention.

Sandbox and FPS remain strong throughout the period, but neither displays a comparable acceleration. Other genres (MOBA, Single Player / Open World, Nintendo, Sports) grow gradually without major discontinuities.

<!-- FIGURE: Monthly uploads & views by genre (entire period / BR boom / BR era) -->
<div class = "plot-card">
  <iframe
    src="/assets/plots/plots_1/plot_1_2.html"
    loading="lazy"
  ></iframe>
</div>


---

<!--- <div style="display:flex; align-items:center; justify-content:space-between; gap:1.5rem; margin:2.5rem 0;">
  
  <h3 style="color:#003c9e; margin:0; font-size:1.7rem; font-weight:900;">
    Relative shares within the gaming ecosystem
  </h3>

  <img 
    src="/assets/img/cake2.png" 
    alt="Image"
    style="
      width:160px;
      height:auto;
      border-radius:14px;
      object-fit:cover;
      display:block;
      box-shadow:0 4px 12px rgba(0,0,0,0.2);
    "
  >

</div> --->

<h3 style="color:#4f6fd6; font-size:1.5rem; font-weight:500;">Relative shares within the gaming ecosystem</h3>

Looking at shares rather than absolute volumes clarifies how BR reshaped the upper layer of YouTube gaming.

Before 2017, FPS and Sandbox dominate uploads and views. During the BR boom, Battle Royale rapidly gains share—mostly at the expense of Sandbox in views and modestly at the expense of both Sandbox and FPS in uploads.  
Importantly, mid-tier genres remain remarkably stable, indicating that the disruption is concentrated at the top of the hierarchy.

By 2018–2019, BR occupies a persistent and large share of both uploads and views, confirming that the eruption is structural rather than transient.

<!-- FIGURE: Share of uploads & views by genre (stacked area plots) -->
<div class = "plot-card">
  <iframe
    src="/assets/plots/plots_1/plot_1_3.html"
    loading="lazy"
  ></iframe>
</div>


---

<div style="display:flex; justify-content:center; margin:2rem 0;">
  <img 
    src="/assets/img/img_1/fortnite_vs.jpeg" 
    alt="Image"
    style="
      width:90%;
      max-width:480px;
      height:auto;
      border-radius:18px;
      display:block;
      margin:auto;
    "
  >
</div>

<h3 style="color:#4f6fd6; font-size:1.5rem; font-weight:500;">Which genres were hit hardest?</h3>

Growth-rate comparisons across three phases—pre (BR, BR boom, and post-BR) show how exceptional BR’s rise was.

During the boom period, Battle Royale exhibits explosive growth in both uploads and views, while most other major genres experience stagnation or decline, particularly in views.  
After the boom, BR continues to grow in uploads and stabilizes at high view levels, while other genres fail to return to their pre-boom growth trajectories.

This strongly suggests that BR did not merely coexist with existing genres, but actively reallocated attention at the top of the ecosystem.

<!-- FIGURE: Growth rate bubbles (uploads vs views, three time periods) -->
<div class = "plot-card">
  <iframe
    src="/assets/plots/plots_1/plot_1_4.html"
    loading="lazy"
  ></iframe>
</div>


---

<div style="display:flex; justify-content:center; margin:2rem 0;">
  <img 
    src="/assets/img/img_1/crown.jpg" 
    alt="Image"
    style="
      width:60%;
      max-width:480px;
      height:auto;
      border-radius:18px;
      display:block;
      margin:auto;
    "
  >
</div>

<h2 style="color:#003c9e; font-size:2rem; font-weight:600;">
  Which Battle Royale games led the wave?
</h2>

The Battle Royale genre is not driven by a single title but by a sequence of releases that shaped its internal dynamics.  
We focus on four BR games present in the Twitch Top-50 panel: H1Z1, PUBG, Fortnite, and Apex Legends, and align their release dates with genre-level trends.

<h3 style="color:#4f6fd6; font-size:1.5rem; font-weight:500;">Temporal alignment with game launches</h3>

Superimposing BR game release dates on the genre-level time series reveals a clear pattern:
- H1Z1 appears early but remains marginal.
- PUBG’s launch in early 2017 coincides with the first visible inflection in BR uploads and views.
- Fortnite’s BR mode marks the start of the explosion.
- Apex Legends enters later, reinforcing but not redefining the existing balance.

<!-- FIGURE: BR uploads & views with annotated game release dates -->
<div class = "plot-card">
  <iframe
    src="/assets/plots/plots_1/plot_1_5.html"
    loading="lazy"
  ></iframe>
</div>


---

<h3 style="color:#4f6fd6; font-size:1.5rem; font-weight:500;">Which games dominate BR content?</h3>

To identify which games truly drive BR discussions, we track the frequency of game-name mentions in BR video metadata.

Fortnite overwhelmingly dominates the conversation from late 2017 onward, far exceeding PUBG, H1Z1 and Apex Legends.  
PUBG plays a crucial early role, while H1Z1 remains limited in scale and Apex Legends produces a visible but short-lived shock.

This confirms that the BR eruption is not only genre-driven, but largely Fortnite-driven.

<!-- FIGURE: Mentions of BR game names over time -->
<div class = "plot-card">
  <iframe
    src="/assets/plots/plots_1/plot_1_6.html"
    loading="lazy"
  ></iframe>
</div>


---

<h3 style="color:#4f6fd6; font-size:1.5rem; font-weight:500;">Internal balance within the Battle Royale genre</h3>

Relative share plots show a clear internal hierarchy:
- H1Z1 establishes the category.
- PUBG triggers the initial expansion.
- Fortnite rapidly captures the vast majority of attention.
- Apex Legends adds a late disturbance without altering the overall regime.

Fortnite emerges as the central engine of BR visibility on YouTube.

<!-- FIGURE: Share of BR game-name mentions -->
<div class = "plot-card">
  <iframe
    src="/assets/plots/plots_1/plot_1_7.html"
    loading="lazy"
  ></iframe>
</div>


---

<h2 style="color:#003c9e; font-size:2rem; font-weight:600;">
  Did Battle Royale grow YouTube gaming or reshuffle it?
</h2>

We now shift to a platform-wide perspective, comparing Battle Royale, non-BR gaming, and total gaming activity, normalized to a common 2016 baseline.

<h3 style="color:#4f6fd6; font-size:1.5rem; font-weight:500;">Overall growth effects</h3>

On the upload side, BR clearly expands the YouTube gaming pie. Non-BR uploads remain stable while BR adds a large and persistent layer of new production.

On the view side, the picture is more mixed. BR contributes to higher total viewership but this increase is accompanied by a visible decline in non-BR views, indicating partial attention reallocation.

<!-- FIGURE: Indexed uploads & views (BR vs non-BR vs total) -->
<div class = "plot-card">
  <iframe
    src="/assets/plots/plots_1/plot_1_8.html"
    loading="lazy"
  ></iframe>
</div>


---

<h3 style="color:#4f6fd6; font-size:1.5rem; font-weight:500;"> BR’s share of total gaming activity </h3>

Battle Royale remains a minority in uploads, stabilizing around 15–20% of total gaming production at its peak.  
In contrast, its share of views rises rapidly after 2017, reaching roughly 25–35% of all YouTube gaming views.

This asymmetry highlights a key result: BR does not dominate creator output but it strongly dominates audience attention.

<!-- FIGURE: Share of BR vs non-BR in uploads and views -->
<div class = "plot-card">
  <iframe
    src="/assets/plots/plots_1/plot_1_9.html"
    loading="lazy"
  ></iframe>
</div>


---

<h2 style="color:#003c9e; font-size:2rem; font-weight:600;">
  Synthesis
</h2>

Act 1 shows that Battle Royale represents a structural break in YouTube gaming.  
Arriving late, BR grows faster than any existing genre, stabilizes at high levels, and reshapes the top tier of the ecosystem.

At the game level, the eruption follows a clear sequence: H1Z1 initiates, PUBG accelerates and Fortnite establishes a lasting regime.  
At the ecosystem level, BR expands content production while simultaneously redirecting viewer attention.



---


<div style="display:flex; justify-content:center; margin:2rem 0;">
  <img 
    src="/assets/img/img_1/domination.png" 
    alt="Image"
    style="
      width:90%;
      max-width:480px;
      height:auto;
      border-radius:18px;
      display:block;
      margin:auto;
    "
  >
</div>
