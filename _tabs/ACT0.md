---
# the default layout is 'page'
layout: page
icon: fas fa-stream
order: 1
title: "ACT 0 - Introduction"
---
<div style="display: flex; align-items: center; gap: 2rem;">
  <h2 style="color:#003c9e; font-size:3rem; font-weight:900; margin:0;">
    Pre-Battle Royale context
  </h2>
  <img src="/assets/img/img_0/victoryroyale.png" alt="Scheme" style="width:800px; height:auto;">
</div>

---
Between 2016 and 2019, Battle Royale reshaped online gaming culture. What began as a niche format rapidly became a dominant genre, triggering massive shifts in creator strategies, audience attention, and platform dynamics.
This study leverages the **YouNiverse dataset** (~32M gaming videos, 137k channels) to quantify how Battle Royale reshaped YouTube's gaming landscape. We develop a hybrid classification system combining TF-IDF vectorization and domain-specific dictionaries to label videos across 12 gaming genres, then apply rolling-window phase detection to track creator specialization over time.

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

---

Our findings reveal Battle Royale not as a transient trend but as a structural transformation in gaming content production, triggering unprecedented creator migration and audience reallocation.


<h2 style="color:#003c9e; font-size:2rem; font-weight:900 !important;">
  The Rise of Battle Royale: Impact on YouTube's Gaming Landscape
</h2>

<h2 style="color:#003c9e; font-size:1.5rem; font-weight:900 !important;">
  What defines a Battle Royale game?
</h2>

In this project, we define Battle Royale (BR) games as a specific subgenre of online multiplayer games where a large number of players compete in the same match with a single objective: be the last player (or team) alive. Although implementations differ from game to game, most Battle Royale titles share a common set of mechanics:

<figure>
  <figcaption style="text-align: center;color: #666666; font-style: italic;">
  Core mechanisms of a battle royale game</figcaption>
  <img src="/assets/img/img_0/Scheme2.png" alt="Scheme" width="800px">
</figure>

These characteristics make Battle Royale games exceptionally well-suited for streaming and YouTube content. The format naturally generates clutch moments, comebacks, and chaotic endgames—ideal for highlights, montages, and high-intensity streams.

Importantly, this combination of mechanics allows Battle Royale games to be unambiguously identified as a distinct genre, even relative to their closest parent genre, First-Person Shooters (FPS). While BR titles often inherit core FPS mechanics such as aiming and weapon handling, features like permanent elimination, large player counts, and match-wide survival dynamics fundamentally differentiate Battle Royale from traditional FPS formats based on rounds, respawns, and team score objectives.






<h2 style="color:#003c9e; font-size:1.5rem; font-weight:900 !important;">
  Historical Context : The Battle Royale Timeline
</h2>

<h3 style="color:#003c9e;"> From Community Experiments to Genre Shock</h3>

Battle Royale did not originate from top-down studio design. It emerged from grassroots experimentation, where players repurposed existing games to explore a simple but powerful idea: survival as the sole win condition.

<figure>
  <img src="/assets/img/img_0/Scheme1.png" alt="Scheme" width="600px">
  <figcaption style="text-align: center;color: #666666; font-style: italic;">Overview of Battle Royale emergence and impact, following the YouNiverse Timescale</figcaption>
</figure>

<h3 style="color:#003c9e;"> Pre-History: Community Mods (2012–2015)</h3>

Early Battle Royale mechanics appeared in marginal spaces of the gaming ecosystem. Minecraft “Hunger Games” servers introduced large-scale survival competition, while Brendan Greene’s **Battle Royale** mod for **DayZ** formalized the last-player-standing loop within a military simulator. With **H1Z1: King of the Kill**, the format reached Steam Early Access, but remained confined to niche survival communities.

At this stage, Battle Royale existed as a design prototype rather than a mainstream genre.

<h3 style="color:#003c9e;"> The Breakthrough (2016–2017)</h3>

The transition from niche to mass adoption occurred abruptly.  
In early 2017, **PUBG** launched as a standalone title and rapidly became one of the most played and most watched games on Twitch, propelled by influencer visibility. Later that year, **Fortnite Battle Royale** removed remaining barriers through free-to-play access, cross-platform support, and a more expressive, streamer-friendly design. By early 2018, Fortnite had overtaken PUBG in viewership, marking Battle Royale’s full entry into popular culture.

This period represents a structural break: Battle Royale was no longer an experiment, but a dominant competitive format.


<h3 style="color:#003c9e;"> Genre Consolidation (2018–2019)</h3>

Following this success, Battle Royale entered a phase of consolidation. Established franchises integrated BR modes, while new titles such as **Apex Legends** refined the formula with hero abilities and fast-paced team play. By mid-2019, Battle Royale had stabilized as a core pillar of multiplayer gaming, alongside MOBAs and traditional FPS.

Innovation slowed, but adoption widened.


<h3 style="color:#003c9e;"> Why YouTube Matters</h3>

If Twitch captured the live explosion of Battle Royale, YouTube recorded its long-term effects. Tutorials, highlights, montages, and edited streams accumulated over time, reflecting sustained creator strategies rather than ephemeral hype. YouTube therefore provides a privileged lens on durable content production, specialization, and audience reallocation.

<h3 style="color:#003c9e;"> Research Positioning</h3>

This project asks a simple question: **how did the 2016–2019 Battle Royale wave reshape YouTube’s gaming ecosystem?**

We approach Battle Royale not as a single event, but as a shock to an existing equilibrium—one that forced creators and viewers to redistribute attention, effort, and engagement across genres.







<h2 style="color:#003c9e; font-size:2rem; font-weight:900 !important;">
    Research Framework
</h2>

<div class="question-box" style="display:flex; gap:2rem;">
  <a href="/act1/" style="text-align:center; color: inherit; text-decoration: none;border-bottom:none;">
    <div style="font-size:2rem; font-weight:bold;">ACT 1</div>
    <div>THE ERUPTION</div>
    <small>“When and how did Battle Royale emerge on YouTube ?”</small>
  </a>
  <a href="/act2/" style="text-align:center; color: inherit; text-decoration: none;border-bottom:none;">
    <div style="font-size:2rem; font-weight:bold;">ACT 2</div>
    <div>CREATOR RESPONSE</div>
    <small>“How did creators adapt to Battle Royale's expansion ?”</small>
  </a>
  <a href="/act3/" style="text-align:center; color: inherit; text-decoration: none;border-bottom:none;">
    <div style="font-size:2rem; font-weight:bold;">ACT 3</div>
    <div>AUDIENCE SHIFTS</div>
    <small>“How did audiences respond to this Youtube Perturbation ?”</small>
  </a>
</div>



<h3 style="color:#003c9e; font-size:2rem; font-weight:900 !important;">
    Game Selection: Building a Representative Panel
</h3>

Rather than manually selecting games, we use **Twitch viewership data** to identify which titles actually mattered during the BR era. We use the Kaggle dataset "Top games on Twitch 2016–2023" (Kartik Kirsh), which tracks monthly hours watched, hours streamed, and average viewers for the top 200 games.

<h3 style="color:#003c9e;"> Selection Process</h3>

<div class="question-box">
  <div class="question-box-title">Key Reflexions</div>
  <ul style="list-style-type:disc; padding-left:1.2rem;">
    <li>
      <a href="#q1" style="color:white; text-decoration:none; font-weight:bold;border-bottom:none;">1. Time Window</a>:<br>
      <span style="font-weight:normal;">Restrict to 2016–2019 (the core BR emergence period)</span>
    </li>
    <li>
      <a href="#q2" style="color:white; text-decoration:none; font-weight:bold;border-bottom:none;">2. Category Filtering</a>:<br>
      <span style="font-weight:normal;">Remove non-game categories (Just Chatting, Creative, etc.)</span>
    </li>
    <li>
      <a href="#q3" style="color:white; text-decoration:none; font-weight:bold;border-bottom:none;">3. License Aggregation</a>:<br>
      <span style="font-weight:normal;">Merge annual releases into unified franchises (all FIFA entries → `FIFA`, all Call of Duty entries → `Call of Duty`)</span>
    </li>
    <li>
      <a href="#q3" style="color:white; text-decoration:none; font-weight:bold;border-bottom:none;">4. Top 50 Panel</a>:<br>
      <span style="font-weight:normal;">Rank by total hours watched and select the 50 most-viewed licenses</span>
    </li>
    <li>
      <a href="#q3" style="color:white; text-decoration:none; font-weight:bold;border-bottom:none;">5. Genre Annotation</a>:<br>
      <span style="font-weight:normal;">Manually assign each license to one of 12 high-level genres</span>
    </li>
  </ul>
</div>
This approach ensures our game panel reflects actual platform dynamics rather than researcher intuition.

<h3 style="color:#003c9e; font-size:2rem; font-weight:900 !important;">
    Data Source: YouNiverse Dataset
</h3>

**YouNiverse** is a large-scale YouTube dataset curated by EPFL, designed for research on content dynamics, creator behavior, and platform evolution.

<b>Dataset Specifications</b>
<table>
  <tr>
    <th>Dimension</th>
    <th>Full Dataset</th>
    <th>Gaming Subset (This Study)</th>
  </tr>
  <tr>
    <td>Videos</td>
    <td>~73M</td>
    <td>~32M</td>
  </tr>
  <tr>
    <td>Channels</td>
    <td>~137k</td>
    <td>~84k</td>
  </tr>
  <tr>
    <td>Time Period</td>
    <td>2005–2019</td>
    <td>2014–2019 (filtered)</td>
  </tr>
  <tr>
    <td>Metadata</td>
    <td>Title, description, tags, category, upload_date</td>
    <td>Same</td>
  </tr>
  <tr>
    <td>Timeseries</td>
    <td>Views, likes, dislikes, comments (daily/weekly)</td>
    <td>Same</td>
  </tr>
  <tr>
    <td>Comments</td>
    <td>~8.6B</td>
    <td>Subset analyzed</td>
  </tr>
</table>

<h3 style="color:#003c9e; font-size:2rem; font-weight:900 !important;">
    Selecting our game panel from Twitch
</h3>

To decide which games actually matter in our analysis, we start from Twitch rather than YouTube. We use the public Kaggle dataset “Top games on Twitch 2016–2023” by Kartik Kirsh, which lists the monthly top 200 games on Twitch together with hours watched, hours streamed and average viewers [Twitch Dataset](https://www.kaggle.com/datasets/rankirsh/evolution-of-top-games-on-twitch).

<figure>
  <img src="/assets/img/img_0/twitch1.png" alt="Scheme" width="20000px">
  <figcaption style="color: #666666; font-style: italic;">
    Top 50 games from Twitch dataset
  </figcaption>
</figure>

**Which games dominate Twitch in our panel?**

League of Legends is clearly the most watched game on Twitch during this period. Following it, Fortnite, Dota 2, and CS:GO form the next tier, showing that MOBAs and FPS titles remain the backbone of Twitch from 2016 to 2019. Battle Royale games already occupy a central role, Fortnite ranks second overall and PUBG sits among the top tier alongside long-established games like Hearthstone, Overwatch, and World of Warcraft

Other games in the top 50 include enduring esports titles such as Rocket League, Smash Bros., and Rainbow Six Siege, which maintain strong and persistent positions. Annual sports franchises like FIFA and NBA 2K appear regularly, reflecting yearly releases and competitive cycles. Large sandbox and open-world games such as Minecraft, GTA V, ARK, DayZ, and RDR2 also sustain high watch time due to their versatile gameplay and persistent communities.

Overall, this panel highlights the core structure of Twitch during these years, MOBAs, FPS, evergreen sandboxes, and major esports, while showing how Battle Royale titles quickly reached top-tier attention, competing with long-standing favorites.



