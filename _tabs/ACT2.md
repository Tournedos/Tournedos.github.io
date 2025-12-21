---
layout: page
icon: fas fa-stream
order: 3
title: "ACT 2 — Creators Response"   # this is used in sidebar             # custom key Chirpy uses to hide top title
permalink: /act2/
---

<!-- ====== Swiper CSS & JS ====== -->
<link rel="stylesheet" href="https://unpkg.com/swiper/swiper-bundle.min.css"/>
<script src="https://unpkg.com/swiper/swiper-bundle.min.js"></script>

<h1 style="color:#003c9e; font-size:3rem; font-weight:900; margin:0;">
  Creators response to the Battle royale's turnover
</h1>

<figure style="text-align: center;">
  <img src="/assets/img/img_2/apex_legend.jpg" width="600px" alt="Fortnite Season 1 Wallpaper"  style="border-radius:24px; display: block; margin: 0 auto;">
  <figcaption style="color: #666666; font-style: italic; margin-top: 8px;">
    Promotional artwork from Apex Legends, one of the flagship titles of the Battle Royale genre.
  </figcaption>
</figure>

<style>
  /* Remove underline from all links inside question-box */
  .question-box a {
    text-decoration: none !important; /* enforce removal */
    color: white;
    font-weight: bold;
    cursor: default; /* prevents hover underline effects */
  }
  .question-box {
    background: #0a4fffde;
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
    background: #003cbd;
    border-color: rgba(255,255,255,0.15);
    box-shadow: 0 8px 24px rgba(0,0,0,0.5);
  }
</style>

---

This section examines how YouTube gaming content creators responded to the Battle Royale (BR) phenomenon. While Act 1 established that BR emerged as a dominant force in uploads and views, the focus now shifts from content to creators, the individuals and channels who shape the platform’s ecosystem. The central question becomes: **how did content creators adapt their strategies in response to BR’s rise ?** Two competing hypotheses frame the inquiry:

*Pivoting :* Creators abandoned previous genres to specialise in BR (genre substitution).

*Diversifying :* Creators added BR while maintaining existing content (genre expansion).

---

<div class="question-box">
  <div class="question-box-title">Key Reflexions</div>
  <ul style="list-style-type:disc; padding-left:1.2rem;">
    <li>
      <a href="#q1" style="color:white; text-decoration:none; font-weight:bold;border-bottom:none;">Phase Transition Dynamics</a>:<br>
      <span style="font-weight:normal;">Tracking how creators moved between genres over time using rolling‑window phase detection</span>
    </li>
    <li>
      <a href="#q2" style="color:white; text-decoration:none; font-weight:bold;border-bottom:none;">Genre Cannibalisation Analysis</a>:<br>
      <span style="font-weight:normal;">Testing whether BR growth came at the expense of other genres or expanded the ecosystem</span>
    </li>
    <li>
      <a href="#q3" style="color:white; text-decoration:none; font-weight:bold;border-bottom:none;">Channel‑Level Profiling</a>:<br>
      <span style="font-weight:normal;">Examining upload strategies and growth patterns of BR creators</span>
    </li>
  </ul>
</div>

<h2 id="q1" style="color:#003c9e; font-size:2rem; font-weight:600;">
  Phase Transition Dynamics
</h2>

To understand **creator migration patterns**, we follow each channel’s main genre over time to detect when creators shift focus. In this section, we uncover patterns of migration, see whether Battle Royale stole attention from other genres, and examine how creators adapted to the new trend.

<div class="question-box">
  <div class="question-box-title">Key Questions for Phase Transition Dynamics</div>
  <ul>
    <li>
      <span style="color:white; text-decoration:none; border-bottom:none;">
        How did genre preferences evolve over time ?
      </span>
    </li>
    <li>
      <span style="color:white; text-decoration:none; border-bottom:none;">
        When did BR emerge as a significant destination ?
      </span>
    </li>
    <li>
      <span style="color:white; text-decoration:none; border-bottom:none;">
        Which genres served as sources for BR creators ?
      </span>
    </li>
  </ul>
</div>

By tracking these movements, we can reconstruct BR’s rise from the perspective of creators rather than aggregate views.

<h3 style="color:#4f6fd6; font-size:1.5rem; font-weight:500;">Phase Transition Heatmaps: Before vs After H1Z1</h3>

We compared how creators moved between genres before and after the release of H1Z1, the first major BR title. By counting and weighting these transitions, we get a sense of how the BR wave reshaped creators’ trajectories, even if the raw numbers aren’t shown here.


<h3 id="transition-correlations" style="color:#4f6fd6; font-size:1.5rem; font-weight:500;">Quarterly and Yearly Transition Dynamics</h3>

From 2015 to 2019 (quarter by quarter), we tracked how creators moved between genres each quarter. The interactive matrix lets you explore these flows over time.

<div style="width:100%; height:100vh;">
  <iframe
    src="/assets/plots/plots_2/phase_transition_matrix_slider.html"
    style="width:100%; height:100%; border:none;"
    scrolling="no">
  </iframe>
</div>

2017 marks a clear turning point. Before then, creators mostly transitioned toward FPS. With the 2017–2018 Fortnite boom, Battle Royale quickly became the main destination, taking over flows that once went to FPS. BR moved from niche curiosity to the typical first phase for new channels, hinting at a structural shift in the genre landscape.

*Note: The 2019 matrix appears visually flatter because it contains fewer total transitions due to the dataset's temporal boundary. The relative distribution patterns remain consistent.*

---


<h2 id="q2" style="color:#003c9e; font-size:2rem; font-weight:600;">
  Genre Cannibalisation Analysis
</h2>

Did Battle Royale grow by eating other genres, or did it expand the ecosystem? We define **cannibalization as a zero-sum shift**: BR gains at the cost of other genres, either by creators leaving them or by capturing the pool of new entrants. If true, rising BR shares should coincide with declining inflows or shrinking shares elsewhere. We examine this using three complementary approaches:


<div class="question-box">
  <div class="question-box-title">Key Questions for Genre Cannibalisation Analysis</div>
  <ul style="list-style-type:disc; padding-left:1.2rem;">
    <li>
      <span style="color:white; text-decoration:none; font-weight:bold;border-bottom:none;">Genre proportions over time</span>:<br>
      <span style="font-weight:normal;">How did the share of active channels in each genre evolve ?</span>
    </li>
    <li>
      <span style="color:white; text-decoration:none; font-weight:bold;border-bottom:none;">Direct inflows to BR</span>:<br>
      <span style="font-weight:normal;">Which genres did BR creators come from ?</span>
    </li>
    <li>
      <span style="color:white; text-decoration:none; font-weight:bold;border-bottom:none;">Transition correlations</span>:<br>
      <span style="font-weight:normal;">Do quarterly inflows to BR correlate (negatively) with inflows to other genres ?</span>
    </li>
  </ul>
</div>



Together, these perspectives build a comprehensive picture of whether BR’s rise was zero‑sum or additive.

<h3 style="color:#4f6fd6; font-size:1.5rem; font-weight:500;">Genre Market Share Over Time</h3>

We first examine how the distribution of channels across genres evolved over time. A channel is counted as "in" a genre during a quarter if its phase overlaps with that quarter. This stacked area chart shows the relative share of each genre (excluding *Genreless*) from 2015 to 2019.

<iframe
  src="/assets/plots/plots_2/genre_composition_interactive.html"
  style="width:100%; height:70vh; border:none;">
</iframe>

By 2019, Battle Royale has climbed from near zero to roughly 25 % of genre-specific channels, while Sandbox, FPS, and other top genres shrink in relative terms. Correlations reveal a **strong negative association between BR and other genres**, especially FPS (r ≈ −0.97). These proportions, however, are inherently zero-sum: the growth of one genre can mechanically reduce the relative shares of others even if no creators actually switch. The chart highlights BR’s rising prominence and its reshaping of the genre landscape, but to understand whether it truly **drew creators away**, we must next examine direct inflows.

<h3 style="color:#4f6fd6; font-size:1.5rem; font-weight:500;">Direct Inflows to Battle Royale</h3>

While market share charts show relative shifts, they do not reveal where Battle Royale’s growth came from. To uncover its sources, we count all transitions from each genre into BR between 2015 and 2019. These visualizations highlight which creator pools BR drew from most and how the **composition of inflows changed over time**.

<iframe
  src="/assets/plots/plots_2/br_inflows_sankey.html"
  style="width:100%; height:70vh; border:none;">
</iframe>

<iframe
  src="/assets/plots/plots_2/first_phases_by_quarter.html"
  style="width:100%; height:70vh; border:none;">
</iframe>

Direct inflow analysis confirms that **FPS channels fed most of BR’s growth**, with 912 transitions—more than twice that of the next contributor, Sandbox. Sports and Single Player/Open World follow, while MOBA and MMORPG contribute relatively few. This pattern aligns with mechanical overlap: BR shares shooting, looting, map navigation, and competitive mechanics with these genres, making the transitions natural.

Temporally, inflows are low in 2015–2016, surge in 2017, peak during the 2018 Fortnite boom, and taper as BR matures in 2019. By early 2018, BR overtakes FPS and Sandbox as the dominant first phase for new channels. Yet, raw counts alone cannot prove cannibalization, large FPS→BR flows might simply reflect FPS’s overall size. To clarify, we next examine correlations between BR inflows and inflows to other genres.

---

<h3 style="color:#4f6fd6; font-size:1.5rem; font-weight:500;">Transition Flow Correlations</h3>

<div style="display:flex; align-items:flex-start; gap:1.5rem; margin:2rem 0;">
  <div style="flex:1;">
    <p>To test for competition between genres, we compute Pearson correlations between quarterly inflows to BR and inflows to other genres, as visualized in the correlation matrix slider above.</p>
    
    <p>Despite FPS being BR’s largest feeder, its quarterly inflows remain stable as BR grows (r≈0.045, p≈0.85). MMORPG shows a weak negative trend (r≈−0.42), but this reflects broader declines rather than direct competition. Other genres such as Fighting, Nintendo, and Sports even rise alongside BR. Overall, BR’s expansion <strong>did not cannibalise other genres but coexisted</strong> with healthy inflows across the platform.</p>
  </div>
  
  <div style="flex:0 0 50%; max-width:300px;">
    <img src="/assets/img/img_2/battlebus.png" 
         alt="Battle Royale investigation illustration" 
         style="width:100%; border-radius:18px;">
  </div>
</div>

---

<h3 style="color:#4f6fd6; font-size:1.5rem; font-weight:500;">Battle Royale Carved Its Own Path</h3>

Combining these perspectives clarifies BR’s impact on the gaming landscape. Market share shows BR rising to ~25 % by 2019, **compressing other genres’ relative shares**. Direct inflows highlight **FPS as the main source** (912 transitions), followed by Sandbox and Sports. Yet correlation tests indicate that BR’s growth did not suppress inflows to other genres. Instead, it attracted new creators while drawing from existing ones, expanding the ecosystem without cannibalising others.


<h2 id="q3" style="color:#003c9e; font-size:2rem; font-weight:600;">
  Channel-Level Profiling
</h2>

To understand how Battle Royale participation shapes creator behaviour, we adopt two **complementary analytical designs**. These approaches allow us to examine differences both across the entire population of channels and within each creator’s own history, isolating the effect of BR phases from baseline channel characteristics.

<div class="question-box">
  <div class="question-box-title">Complementary Analytical Designs</div>
  <ul style="list-style-type:disc; padding-left:1.2rem;">
    <li>
      <span style="color:white; text-decoration:none; font-weight:bold;border-bottom:none;">Pooled analyses</span>:<br>
      <span style="font-weight:normal;">Compare BR phases against non‑BR phases across all channels to capture population‑level differences.</span>
    </li>
    <li>
      <span  style="color:white; text-decoration:none; font-weight:bold;border-bottom:none;">Within‑channel (paired) analyses</span>:<br>
      <span style="font-weight:normal;">Contrast each creator’s behaviour during BR phases with their own behaviour in other phases to control for stable channel characteristics.</span>
    </li>
  </ul>
</div>

This dual approach separates selection effects (e.g., prolific uploaders may choose BR) from behavioural changes induced by the genre itself.

<h3 style="color:#4f6fd6; font-size:1.5rem; font-weight:500;">Channel Growth Analysis</h3>

To test whether Battle Royale accelerates channel growth, we compare **subscriber growth per day** and **growth rate per day across BR and non‑BR phases**. Analyses consider all channels, contrasting creators who ever produced BR content with those who did not, and paired channels, comparing each creator’s BR phases to their own non‑BR phases. Right‑skewed distributions and outliers are addressed using both non‑parametric *(Mann–Whitney U, Wilcoxon signed‑rank)* and parametric *(Welch’s and paired t‑tests)* tests, ensuring results are robust to distributional assumptions.

<iframe
  src="/assets/plots/plots_2/growth_per_day_comparison.html"
  style="width:100%; height:100vh; border:none;">
</iframe>

Across both pooled and paired analyses, channels experience faster subscriber growth during Battle Royale phases than in other genres. This holds even when controlling for channel-specific effects, confirming that BR offered a genuine growth advantage rather than merely reflecting a fleeting trend. The genre’s **rapid audience expansion** translated into **measurable benefits for individual creators**.


<h3 style="color:#4f6fd6; font-size:1.5rem; font-weight:500;">Upload Frequency Analysis</h3>

Next, we ask whether BR creators **upload content at different rates than creators in other genres**. Using the same pooled and paired designs, we calculate videos per day for each channel and compare BR versus non‑BR phases. Non‑parametric tests (*Mann–Whitney U, Wilcoxon signed‑rank*) are again employed due to skewed distributions, with parametric tests included for robustness.

<iframe src="/assets/plots/plots_2/upload_freq_per_subscriber.html"
        style="width:100%; height:100vh; border:none;"></iframe>

BR channels post more frequently than other creators on average (pooled analysis, p < 0.001), suggesting that prolific uploaders were more likely to adopt the genre. However, within‑channel comparisons reveal **no significant change in posting rate** when switching to BR. In other words, adopting BR does not make creators post more often; instead, channels that already upload frequently are the ones joining BR.

Looking at uploads relative to audience size (videos per subscriber) adds another layer: BR creators rank among the lowest, showing that adoption was driven by **audience opportunity** rather than extra effort or intrinsic motivation. Battle Royale rewarded channels with existing momentum, not higher relative output.

<h3 style="color:#4f6fd6; font-size:1.5rem; font-weight:500;">Phase Duration by Genre</h3>

If BR primarily **attracted opportunists** rather than committed creators, we would expect BR phases to be shorter. To test this, we compare the duration of BR phases to phases in other genres using both pooled and paired analyses. Phase duration is measured as the number of days a channel remains in a single genre phase.

<iframe
  src="/assets/plots/plots_2/phase_duration_distribution.html"
  style="width:100%; height:100vh; border:none;">
</iframe>

Battle Royale phases are significantly shorter than phases in other genres. This holds both in the all‑channels comparison and within‑channel analysis, indicating that the effect is not driven by differences between creators. On average, creators spend less time in BR phases, suggesting that BR content is more experimental: **many try it, but fewer stick with it**. Other genres tend to foster longer‑lasting engagement, highlighting BR’s transient nature.


<h3 style="color:#4f6fd6; font-size:1.5rem; font-weight:500;">Genre Adoption and Willingness to Experiment</h3>

Finally, we examine how many channels **tried each genre** at least once. This highlights BR’s reach and experimental appeal compared with other categories, focusing on how many creators sampled it rather than how long they stayed.

<iframe
  src="/assets/plots/plots_2/genre_adoption_rates.html"
  style="width:100%; height:70vh; border:none;">
</iframe>

Adoption patterns highlight BR’s broad appeal. While FPS still tops with 20 % of channels entering at least once, BR follows closely at 16.1 %, impressive given its late arrival. Sandbox (13.2 %) and Single Player/Open World (11.1 %) show moderate experimentation, whereas MOBA, Sports, MMORPG, and Strategy remain under 6 %. Coupled with shorter phase durations, these results paint BR as a genre many creators tried but few fully committed to—a **high-attraction, low-commitment genre**.


<h2 style="color:#003c9e; font-size:2rem; font-weight:600;">
  Creator Response: General Synthesis
</h2>

Across Act 2, Battle Royale reshaped creator behaviour **without cannibalising other genres**. After 2017, BR transitions surge, surpassing FPS and becoming the typical first phase for new channels. Correlations confirm that inflows to FPS and others remain stable, showing BR **expanded the ecosystem rather than displaced it**. At the channel level, BR phases deliver a growth premium but are ****shorter** and **do not boost upload intensity**. High adoption coupled with **brief engagement frames** BR as a catalyst: widely tried, quickly rewarding, but rarely a long-term home. In short, BR opened new pathways, encouraged diversification, and offered creators a surge of opportunity without eroding existing foundations.
