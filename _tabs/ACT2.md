---
layout: page
icon: fas fa-stream
order: 3
title: "ACT 2 — Creators Response"   # this is used in sidebar             # custom key Chirpy uses to hide top title
---

<!-- ====== Swiper CSS & JS ====== -->
<link rel="stylesheet" href="https://unpkg.com/swiper/swiper-bundle.min.css"/>
<script src="https://unpkg.com/swiper/swiper-bundle.min.js"></script>

<h1 style="color:#003c9e; font-size:3rem; font-weight:900; margin:0;">
  Creators response to the Battle royale's turnover
</h1>

<figure style="text-align: center;">
  <img src="/assets/img/img_2/apex_legend.jpg" width="600px" style="border-radius:24px; display: block; margin: 0 auto;">
  <figcaption style="color: #666666; font-style: italic; margin-top: 8px;">
    Promotional artwork from Apex Legends, one of the flagship titles of the Battle Royale genre.
  </figcaption>
</figure>

<h3 style="color:#4f6fd6; font-size:1.5rem; font-weight:500;">The Turning point</h3>
The year 2017 emerges as a clear turning point, coinciding with the rapid expansion of the Battle Royale genre following the release of Fortnite. Prior to 2017, creators predominantly transition toward the FPS genre. From 2017 onward, Battle Royale captures the majority of transitions that previously targeted FPS, suggesting a structural shift in genre dynamics. This observation motivates an explicit investigation into whether Battle Royale effectively absorbed transition flows from other genres.

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

<div class="question-box">
  <div class="question-box-title">Key Questions</div>
  <ul>
    <li>Did existing creators pivot to BR content ?</li>
    <li>Did posting BR videos accelerate channel growth ?</li>
    <li>Did BR introduce new video formats (length, frequency) ?</li>
  </ul>
</div>

<h2 style="color:#003c9e; font-size:2rem; font-weight:600;">(2.1) Did existing creators pivot to BR content ?</h2>
<h3 style="color:#4f6fd6; font-size:1.5rem; font-weight:500;">Approach 1 : Proportions Of Channels in each Genre Phase Over Time</h3>

<iframe
  src="/assets/plots/plots_2/genre_composition_interactive.html"
  style="width:100%; height:80vh; border:none;">
</iframe>

<h3 style="color:#4f6fd6; font-size:1.5rem; font-weight:500;">Interpretation</h3>

The proportion analysis shows strong **negative correlations** between Battle Royale’s market share and most other genres. The strongest association is observed with FPS (r = −0.972), followed by MMORPG and MOBA. Horror is the only genre that does not exhibit a significant correlation. Battle Royale grows from near zero to roughly 25% of genre-specific channels by 2019, the relative share of all other genres decreases accordingly.

These correlations must be interpreted with care. Genre proportions are zero-sum by construction: an increase in Battle Royale’s share necessarily implies a decrease in the combined share of other genres. As a result, a rapidly expanding genre will mechanically exhibit negative correlations with others, even in the absence of direct creator migration.

The proportion analysis therefore demonstrates that Battle Royale substantially reshaped the genre landscape in relative terms, but it does not explain the underlying mechanism. In particular, it cannot determine whether Battle Royale **drew creators away** from existing genres, **absorbed creators** who would otherwise have entered those genres, or expanded primarily by **attracting new creators**.To address this question, we next analyze direct inflows into the Battle Royale genre to identify the actual sources of its growth.

<h3 style="color:#4f6fd6; font-size:1.5rem; font-weight:500;">Approach 2 : Direct Inflows to Battle Royale</h3>

<iframe
  src="/assets/plots/plots_2/br_inflows_sankey.html"
  style="width:100%; height:70vh; border:none;">
</iframe>

<h3 style="color:#4f6fd6; font-size:1.5rem; font-weight:500;">Interpretation</h3>

The direct inflow analysis shows that FPS is by far the main source of Battle Royale creators, with 912 transitions, more than 2.5 times the second-largest contributor, Sandbox (358). Sports (301) and Single Player / Open World (205) follow, while traditionally competitive genres such as MOBA (46) and MMORPG (27) contribute relatively few creators.

This ranking is intuitive. Battle Royale shares core mechanics with shooters (aiming, weapons, movement), open-world or survival games (looting, map navigation), and sports titles (competitive multiplayer and seasonal dynamics). Creators from these genres therefore possess transferable skills and are likely to appeal to similar audiences.

The temporal breakdown follows the expected trajectory: limited inflows in 2015–2016, rapid growth in 2017, a pronounced peak in 2018 during the Fortnite boom, and a decline in 2019 as the genre matures (even taking into account the removed 2019 Q4). The composition of inflows remains stable over time, with FPS consistently dominating.

However, absolute inflow counts alone do not resolve the cannibalization question. The large number of FPS-to-BR transitions could indicate substantial diversion of FPS creators, or alternatively reflect a small fraction of a very large FPS creator base. To distinguish between these possibilities, inflows must be interpreted relative to the size of each source genre and examined alongside transition correlations that capture whether BR growth coincided with reduced transitions into other genres.

<h3 style="color:#4f6fd6; font-size:1.5rem; font-weight:500;">Approach 3 : Transition Flow Correlations</h3>
Finally, we test whether quarterly transition flows TO Battle Royale correlate with flows TO other genres. A significant negative correlation would suggest competition for incoming creators. Before running the correlation analysis, we verified whether the data satisfied the standard assumptions of Pearson correlation.

<div style="width:100%; height:100vh;">
  <iframe
    src="/assets/plots/plots_2/phase_transition_matrix_slider.html"
    style="width:100%; height:100%; border:none;"
    scrolling="no">
  </iframe>
</div>

<h3 style="color:#4f6fd6; font-size:1.5rem; font-weight:500;">Interpretation</h3>

The transition flow analysis provides a different perspective from the raw inflow counts.

For FPS, despite being the largest absolute source of Battle Royale creators (912 transitions), there is no evidence of cannibalization. Quarterly inflows to Battle Royale are uncorrelated with inflows to FPS (r = 0.045, p = 0.85), and the confidence interval clearly includes zero. Periods of increased transition into Battle Royale therefore did not coincide with reduced transition into FPS, indicating that the two flows evolved independently.

MMORPG is the only genre showing a pattern consistent with potential cannibalization. It exhibits a moderate negative correlation with Battle Royale inflows (r = −0.420), with a confidence interval excluding zero. Quarters with higher Battle Royale inflows tend to correspond to lower MMORPG inflows. However, MMORPG contributes only 27 creators to Battle Royale overall, suggesting that this pattern may reflect a broader decline in MMORPG rather than direct competition with Battle Royale.

Several genres grew alongside Battle Royale. Fighting (r = 0.74), Nintendo (r = 0.58), and Sports (r = 0.54) all show significant positive correlations, with increased creator inflows occurring in the same quarters as Battle Royale expansion. Given the absence of shared core mechanics or obvious structural links with Battle Royale, these concurrent increases more likely reflect overall growth in gaming content rather than any direct relationship.

<h2 style="color:#003c9e; font-size:2rem; font-weight:600;">(2.2) Did posting BR videos accelerate channel growth ?</h2>
## **No answer for now**

<h2 style="color:#003c9e; font-size:2rem; font-weight:600;">(2.3) Did BR introduce new video formats (length, frequency) ?</h2>
## **No answer for now**

<h2 style="color:#003c9e; font-size:2rem; font-weight:600;">Synthesis: Battle Royale Carved Its Own Path</h2>

The three approaches yield complementary findings that together clarify how Battle Royale reshaped the gaming content landscape.

The Market Share approach established that BR's rise fundamentally altered the genre distribution. As BR grew from near-zero to ~25% of genre-specific channels, nearly all other genres declined in relative terms, with FPS showing the strongest inverse relationship (r = -0.97). However, proportions are zero-sum by construction, this tells us that the landscape changed, not how.

The Direct Inflows approach revealed that FPS was by far the largest source of BR creators (912 transitions), followed by Sandbox (358) and Sports (301). This makes mechanical sense given the gameplay overlap between shooters and Battle Royale. In absolute terms, BR clearly drew from the FPS creator pool.

The Transition Correlations approach provided a critical insight. Despite FPS being BR's primary feeder genre, quarterly flows into FPS showed no correlation with flows into BR (r = 0.045). Creators continued entering FPS at rates independent of BR's growth. MMORPG was the only genre showing a negative correlation, but since only 27 creators transitioned from this genre to BR, it suggest more of an independent decline rather than direct competition.


<h2 style="color:#003c9e; font-size:2rem; font-weight:600;">Conclusion</h2>
Battle Royale did not cannibalize other genres through competitive displacement. This apparent contradiction, especially with FPS that lost market share while its creator pipeline remained unaffected, resolves when we recognize that BR's growth was largely additive. BR attracted new creators and drew from existing pools without reducing the rate at which those pools replenished. The result was an expanded ecosystem in which BR claimed a large share, mechanically compressing other genres' relative presence without undermining their absolute vitality at the creator level.
