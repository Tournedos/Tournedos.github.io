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

<h3 style="color:#4f6fd6; font-size:1.5rem; font-weight:500;">The Turning point</h3>
The year 2017 emerges as a clear turning point, coinciding with the rapid expansion of the Battle Royale genre following the release of Fortnite. Prior to 2017, creators predominantly transition toward the FPS genre. From 2017 onward, Battle Royale captures the majority of transitions that previously targeted FPS, suggesting a structural shift in genre dynamics. This observation motivates an explicit investigation into whether Battle Royale effectively absorbed transition flows from other genres. Throughout this Act, we will be answering the three following questions :

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

This section examines how YouTube gaming content creators responded to the Battle Royale (BR) phenomenon. While Act 1 established that BR emerged as a dominant force in uploads and views, the focus now shifts from content to creators—the individuals and channels who shape the platform’s ecosystem. The central question becomes: how did content creators adapt their strategies in response to BR’s rise? Two competing hypotheses frame the inquiry:

Pivoting: Creators abandoned previous genres to specialise in BR (genre substitution).

Diversifying: Creators added BR while maintaining existing content (genre expansion).

Our investigation proceeds in three parts: (1) phase transition dynamics, tracking how creators moved between genres over time using rolling‑window phase detection; (2) genre cannibalisation analysis, testing whether BR growth came at the expense of other genres or expanded the ecosystem; and (3) channel‑level profiling, examining upload strategies and growth patterns of BR creators.

---

<div class="question-box">
  <div class="question-box-title">Key Questions</div>
  <ul>
    <li>
      <a href="#q1" style="color:white; text-decoration:none;border-bottom:none;">
        Did existing creators pivot to BR content ?
      </a>
    </li>
    <li>
      <a href="#q2" style="color:white; text-decoration:noneborder-bottom:none;;">
        Did posting BR videos accelerate channel growth ?
      </a>
    </li>
    <li>
      <a href="#q3" style="color:white; text-decoration:none;border-bottom:none;">
        Did BR introduce new video formats (length, frequency) ?
      </a>
    </li>
  </ul>
</div>

<h2 id="q1" style="color:#003c9e; font-size:2rem; font-weight:600;">(2.1) Did existing creators pivot to BR content ?</h2>

<table style="width:100%; border-collapse: collapse; text-align: left; font-size:0.75rem;">
  <thead>
    <tr style="background-color:#003c9e; color:white;">
      <th style="padding:6px;">Approach</th>
      <th style="padding:6px;">Question</th>
      <th style="padding:6px;">Cannibalization Signal</th>
    </tr>
  </thead>
  <tbody>
    <tr style="background-color:#f0f0f0;">
      <td style="padding:6px;">
        <a href="#proportions" style="color:#003c9e; text-decoration:underline;">Genre proportions over time</a>
      </td>
      <td style="padding:6px;">What share of active channels are in each genre at time t?</td>
      <td style="padding:6px;">If BR rises while other genres fall, suggests displacement</td>
    </tr>
    <tr>
      <td style="padding:6px;">
        <a href="#direct-inflows" style="color:#003c9e; text-decoration:underline;">Direct inflows to BR</a>
      </td>
      <td style="padding:6px;">Which genres did BR creators come from?</td>
      <td style="padding:6px;">Shows exactly where BR pulled creators from</td>
    </tr>
    <tr style="background-color:#f0f0f0;">
      <td style="padding:6px;">
        <a href="#transition-correlations" style="color:#003c9e; text-decoration:underline;">Transition correlations</a>
      </td>
      <td style="padding:6px;">Do quarterly flows to genre X correlate with flows to BR?</td>
      <td style="padding:6px;">Negative correlation suggests competition for incoming creators</td>
    </tr>
  </tbody>
</table>

<h2 id="q2" style="color:#003c9e; font-size:2rem; font-weight:600;">
  (1) PHASE TRANSITION DYNAMICS ?
</h2>

To understand creator migration patterns, we use a rolling‑window phase detection algorithm that assigns each channel to a primary genre at any point in time. A phase represents a contiguous period during which a channel predominantly uploads content in a single genre; transitions between phases mark moments when creators shift their content focus. This section analyzes those transitions to address three questions:

**How did genre preferences evolve over time?**

**When did BR emerge as a significant destination?**

**Which genres served as sources for BR creators?**

By tracking these movements, we can reconstruct BR’s rise from the perspective of creators rather than aggregate views.

<h3 style="color:#4f6fd6; font-size:1.5rem; font-weight:500;">(1.1) Phase Transition Heatmaps: Before vs After H1Z1*</h3>

To visualize how creators shifted between genres, we construct transition matrices that count how often channels move from one genre phase (row) to another (column). We split the analysis at 15 January 2015, the release of H1Z1, the first major standalone BR title, to compare patterns before and after BR’s arrival. Two versions of each matrix are presented:

**Absolute counts**: raw numbers of transitions.

**Duration‑weighted counts**: normalized by how long creators stayed in the target phase, giving more weight to sustained commitments.

These heatmaps provide a baseline for detecting structural changes in creator trajectories.

<h3 id="transition-correlations" style="color:#4f6fd6; font-size:1.5rem; font-weight:500;">(1.2) Quarterly and Yearly Transition Dynamics</h3>

To track how migration patterns evolved, we build transition matrices for each quarter from 2015 to 2019. Examining these quarter‑by‑quarter flows allows us to pinpoint when BR became a dominant destination and to contextualize it within annual trends. This granular view reveals not only the overall volume of genre switching but also shifts in creator preferences over time.

<div style="width:100%; height:100vh;">
  <iframe
    src="/assets/plots/plots_2/phase_transition_matrix_slider.html"
    style="width:100%; height:100%; border:none;"
    scrolling="no">
  </iframe>
</div>

**Interpretation: Year-by-Year Transition Dynamics**

The year 2017 emerges as a clear turning point. Prior to 2017, creators transitioning between genres mostly moved toward the long‑established First‑Person Shooter (FPS) category. Starting in 2017 and accelerating with the 2017–2018 Fortnite boom, Battle Royale captures the majority of transitions that previously targeted FPS. This shift signals a structural change in the genre landscape: BR moves from peripheral curiosity to primary destination, eventually becoming the typical first phase for new channels as we will see later. The observation motivates a more rigorous test of whether BR absorbed flows from other genres or merely coincided with overall growth.

*Note: The 2019 matrix appears visually flatter because it contains fewer total transitions due to the dataset's temporal boundary. The relative distribution patterns remain consistent.*

---


<h2 id="q2" style="color:#003c9e; font-size:2rem; font-weight:600;">
  (2) TESTING FOR GENRE CANNIBALIZATION?
</h2>

A central question is whether BR’s explosive growth came at the expense of other genres. In this context, we define cannibalization as a zero-sum reallocation of creators, whereby increased entry into Battle Royale would be associated with reduced entry into other genres, either because creators actively switch away from them or because BR absorbs a fixed pool of incoming creators that would otherwise have entered elsewhere. Under cannibalization, BR growth should therefore coincide with declining inflows or shrinking shares in competing genres, beyond what would be expected from overall ecosystem growth. We examine this using three complementary approaches:

**1. Genre proportions over time**: How did the share of active channels in each genre evolve? If BR rises while others fall, displacement is suggested.

**2. Direct inflows to BR**: Which genres did BR creators come from? This identifies the actual sources of BR growth.

**3. Transition correlations**: Do quarterly inflows to BR correlate (negatively) with inflows to other genres? A negative correlation would signal competition for incoming creators.

Together, these perspectives build a comprehensive picture of whether BR’s rise was zero‑sum or additive.

<h3 style="color:#4f6fd6; font-size:1.5rem; font-weight:500;">(2.1) Genre Market Share Over Time</h3>

We first examine how the distribution of channels across genres evolved over time. A channel is counted as "in" a genre during a quarter if its phase overlaps with that quarter. This stacked area chart shows the relative share of each genre (excluding *Genreless*) from 2015 to 2019.

<iframe
  src="/assets/plots/plots_2/br_inflows_sankey.html"
  style="width:100%; height:70vh; border:none;">
</iframe>

**Interpretation: Genre Market Share in Releases Over Time**

The stacked area charts reveal BR climbing from obscurity to roughly 25 % of genre‑specific channels by 2019, while the relative shares of Sandbox, FPS and other top genres decline. Correlation analysis shows strong negative associations between BR’s share and most other genres, especially FPS (r ≈ −0.97). However, these figures must be interpreted with caution: genre proportions are zero‑sum by construction. A rapidly expanding genre will mechanically show negative correlations with others, even without direct migration. The market share approach thus demonstrates that BR reshaped the landscape in relative terms but cannot determine whether it drew creators away from established genres or attracted new entrants. To resolve this ambiguity, we turn to direct inflows.

<h3 style="color:#4f6fd6; font-size:1.5rem; font-weight:500;">(2.2) Direct Inflows to Battle Royale</h3>

While market share charts highlight relative changes, they do not identify where BR’s growth came from. We therefore count all transitions from each genre into BR. We tally absolute counts across 2015–2019 and break them down by year, plotting both total inflows and proportions by year. These visualisations reveal which creator pools BR tapped most heavily and how the composition of inflows evolved over time.

<iframe
  src="/assets/plots/plots_2/first_phases_by_quarter.html"
  style="width:100%; height:70vh; border:none;">
</iframe>

** Interpretation: Source Genres for Battle Royale Creators ** 

Direct inflow analysis shows that FPS is by far the main source of BR creators, contributing 912 transitions, more than twice the second‑largest contributor, Sandbox (358). Sports (301) and Single Player/Open World (205) follow, while MOBA (46) and MMORPG (27) contribute relatively few. This ranking aligns with mechanical overlap: BR shares core mechanics with shooters (aiming, weapons, movement), open‑world survival games (looting, map navigation) and sports titles (competitive multiplayer, seasons), making the transition natural. Temporal patterns reinforce this narrative: inflows are minimal in 2015–2016, grow rapidly in 2017, peak during the Fortnite boom in 2018, and decline as the genre matures in 2019. Notably, by 2018 Q1 BR becomes the dominant first detected phase for new channels, overtaking FPS and Sandbox. However, absolute counts alone do not resolve cannibalisation: the large FPS→BR flow could reflect simply that FPS is a huge pool. To disentangle these possibilities, we examine correlations between BR inflows and inflows to other genres.

---

<h3 style="color:#4f6fd6; font-size:1.5rem; font-weight:500;">(2.3) Transition Flow Correlations</h3>

Absolute counts can be misleading if a large donor genre simply dominates the landscape. To test for true competition, we compute Pearson correlations between quarterly inflows to BR and inflows to each other genre. A significant negative correlation would indicate that quarters with high BR inflow coincide with low inflows elsewhere, evidence of cannibalisation. We also conduct diagnostic checks (normality, heteroscedasticity, autocorrelation) to ensure correlation results are not artefacts of time‑series properties.

Do Battle Royale inflows displace other genres?

To test for cannibalisation, we examine whether quarters with high inflows into Battle Royale coincide with reduced inflows into other genres. If BR were diverting creators, we would expect negative correlations between BR inflows and inflows elsewhere.

This is not what we observe. Despite FPS being the largest source of BR creators, quarterly inflows into FPS are uncorrelated with inflows into BR. Creators continue to enter FPS at stable rates throughout the BR expansion. Other major genres show similar independence.

Some genres—such as Sports, Nintendo, and Fighting—display positive correlations, indicating that their inflows increased in the same periods as BR growth. This suggests that BR’s rise coincided with a broader expansion of creator activity rather than competitive displacement.

Overall, we find no evidence that Battle Royale cannibalised creator inflows from other genres. Instead, BR appears to have emerged alongside sustained growth across the gaming ecosystem.




## **Synthesis: Battle Royale Carved Its Own Path**

Combining these perspectives clarifies how BR reshaped the gaming content landscape. Market share analysis shows BR skyrocketing to ~25 % share by 2019, mechanically compressing other genres’ relative presence. Direct inflows reveal that FPS supplied the bulk of BR creators (912), followed by Sandbox and Sports. Yet correlation tests demonstrate that BR’s growth did not suppress inflows into these genres. Instead, BR attracted new creators and drew from existing pools without diminishing their replenishment, producing an expanded ecosystem where BR claimed a large slice but did not cannibalise others.


<h2 id="q2" style="color:#003c9e; font-size:2rem; font-weight:600;">
  (3) — CHANNEL-LEVEL PROFILING ?
</h2>

Having established the macro‑level dynamics of genre transitions, we now turn to the channel level to examine how BR participation relates to individual creator behaviour and outcomes. We profile BR creators with a focus on content strategies and growth patterns, using two complementary analytical designs:

**Pooled analyses**: Compare BR phases against non‑BR phases across all channels to capture population‑level differences.

**Within‑channel (paired) analyses**: Contrast each creator’s behaviour during BR phases with their own behaviour in other phases to control for stable channel characteristics.

This dual approach separates selection effects (e.g., prolific uploaders may choose BR) from behavioural changes induced by the genre itself.


<h3 style="color:#4f6fd6; font-size:1.5rem; font-weight:500;">(3.1) Channel Growth Analysis</h3>

The core test of BR’s value proposition to creators is whether it accelerates channel growth. We measure subscriber growth per day and growth rate per day, comparing BR phases against non‑BR phases in two ways:

All channels: Compare mean growth among creators who ever produced BR content versus those who did not.

Paired channels: For creators with both BR and other content, compare growth during BR phases to growth during their own non‑BR phases.

To handle right‑skewed distributions and potential outliers, we report both non‑parametric tests (Mann–Whitney U for unpaired comparisons, Wilcoxon signed‑rank for paired) and parametric tests (Welch’s and paired t‑tests) as robustness checks. This ensures that significance is not driven by distributional assumptions.

<iframe
  src="/assets/plots/plots_2/growth_per_day_comparison.html"
  style="width:100%; height:100vh; border:none;">
</iframe>

**Interpretation: Battle Royale Growth Advantage**

Across both pooled and paired analyses, Battle Royale phases are associated with significantly faster subscriber growth. Channels grow more quickly during BR phases than during phases in other genres, even when controlling for channel‑specific effects. This finding confirms that BR represented a genuine growth opportunity, not just a trend creators followed blindly. The genre’s rapid audience expansion translated into tangible benefits for individual channels.


<h3 style="color:#4f6fd6; font-size:1.5rem; font-weight:500;">(3.2) Upload Frequency Analysis</h3>

Next, we ask whether BR creators upload content at different rates than creators in other genres. Using the same pooled and paired designs, we calculate videos per day for each channel and compare BR versus non‑BR phases. Non‑parametric tests (Mann–Whitney U, Wilcoxon signed‑rank) are again employed due to skewed distributions, with parametric tests included for robustness.

<iframe src="/assets/plots/plots_2/upload_freq_per_subscriber.html"
        style="width:100%; height:100vh; border:none;"></iframe>

### Interpretation: Upload Frequency

The results reveal a nuanced pattern. In the pooled analysis, BR channels upload more frequently on average than non‑BR channels (p < 0.001), suggesting that prolific uploaders gravitated toward BR. However, within‑channel comparisons show no significant difference in upload rate between BR and non‑BR phases. In other words, switching to BR does not systematically change how often a channel posts; rather, channels that already upload frequently are more likely to adopt BR. To probe motivation further, we examine upload frequency per subscriber, a ratio capturing content output relative to audience size. Surprisingly, BR creators have among the lowest upload frequencies per subscriber. Contrary to the hypothesis that Battle Royale creators were more “passionate” or intrinsically motivated, the release frequency–to–subscriber ratio shows no systematic increase during BR phases. Creators did not upload more aggressively independent of their success, suggesting that BR adoption was driven by opportunity and audience response rather than exceptional determination.


<h3 style="color:#4f6fd6; font-size:1.5rem; font-weight:500;">(3.3) Phase Duration by Genre</h3>

If BR primarily attracted opportunists rather than committed creators, we would expect BR phases to be shorter. To test this, we compare the duration of BR phases to phases in other genres using both pooled and paired analyses. Phase duration is measured as the number of days a channel remains in a single genre phase.

<iframe
  src="/assets/plots/plots_2/phase_duration_distribution.html"
  style="width:100%; height:100vh; border:none;">
</iframe>

**Interpretation: Phase Duration in Battle Royale Content**

Battle Royale phases are significantly shorter than phases in other genres. This holds both in the all‑channels comparison and within‑channel analysis, indicating that the effect is not driven by differences between creators. On average, creators spend less time in BR phases, demonstrating that BR engagement is intrinsically more transient. Many creators experiment with BR content but do not sustain it, whereas other genres see longer‑lasting engagement. BR thus appears as a genre that creators are more likely to try but less likely to commit to.


<h3 style="color:#4f6fd6; font-size:1.5rem; font-weight:500;">(3.4) Genre Adoption and Willingness to Experiment</h3>

Finally, we examine how many channels tried each genre at least once. By calculating the proportion of channels that entered a phase in each genre, we can gauge BR’s reach relative to other categories. This analysis focuses on adoption rather than duration, showing how widely each genre was experimented with.

<iframe
  src="/assets/plots/plots_2/genre_adoption_rates.html"
  style="width:100%; height:70vh; border:none;">
</iframe>

**Interpretation: Genre Adoption and Willingness to Experiment**

The adoption chart reveals two key insights. First, FPS remains the most broadly adopted genre: 20 % of all channels enter an FPS phase at least once. Second, Battle Royale follows closely at 16.1 %, a remarkably high adoption rate given its later emergence. This shows that BR was not a niche specialisation but a genre that a large fraction of creators actively experimented with during its rise. Sandbox (13.2 %) and Single Player/Open World (11.1 %) show moderate adoption, while MOBA, Sports, MMORPG and Strategy remain below 6 %. Together with the shorter phase durations, these results reinforce the view of BR as a high‑attraction, low‑commitment genre: many creators tried it, but fewer sustained long‑term engagement compared to more traditional genres.


<h2 id="q2" style="color:#003c9e; font-size:2rem; font-weight:600;">
  (4) Creator Response: General Synthesis
</h2>

Across Act 2, the evidence shows that Battle Royale transformed creator behaviour without cannibalising established genres. Structural analyses reveal that BR transitions surge after 2017, overtaking FPS as the main destination and even becoming the typical first phase for new channels. Yet correlation tests confirm that inflows to FPS and other genres remain stable, indicating that BR’s rise expanded the ecosystem rather than displacing existing creator pipelines. Channel‑level profiling demonstrates that BR phases deliver a clear growth premium but are shorter and not accompanied by increased upload intensity. High adoption rates combined with brief engagement suggest that BR functioned as a catalyst: a genre that creators were eager to sample and that rewarded them quickly, but that few adopted as a long‑term home. Thus, BR reshaped YouTube gaming at the creator level by opening new pathways and encouraging diversification, offering a surge of opportunity that did not necessarily erode its foundations.
