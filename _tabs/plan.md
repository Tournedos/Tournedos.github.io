---
layout: page
icon: fas fa-stream
order: 7
---

## *ACT 1: THE ERUPTION*
"How did Battle Royale explode onto YouTube's gaming landscape, and did the momentum persist?"

This act establishes the quantitative foundation: the sheer scale and speed of BR's rise, which games led, and whether the growth plateaued or continued.

| Priority | RQ ID | Research Question                                                              | Plot/Analysis                                                                                             | Data Required                                                       | Persistence Check                                          |
| -------- | ----- | ------------------------------------------------------------------------------ | --------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------- | ---------------------------------------------------------- |
| ⭐⭐⭐      | 1.1   | What was the growth trajectory of BR content vs. other genres?                 | Time series: weekly/monthly video count and view count by subgenre (normalized to 2016 baseline)          | metadata_single_game_identified (upload_date, subgenre, view_count) | Slope in 2019: still growing, plateau, or decline?         |
| ⭐⭐⭐      | 1.2   | Which BR game led the wave? What was the diffusion sequence?                   | Stacked area chart: Fortnite vs PUBG vs H1Z1 vs Apex over time; mark release dates                        | metadata_single_game_identified (game, upload_date)                 | Did early leaders (PUBG, H1Z1) fade as Fortnite dominated? |
| ⭐⭐⭐      | 1.3   | Did BR's rise coincide with overall gaming content growth, or was it zero-sum? | Total gaming uploads per week (all genres) overlaid with BR share                                         | metadata_gaming (upload_date) + subgenre labels                     | Did total pie grow, or just BR's slice?                    |
| ⭐⭐       | 1.4   | Did new gaming channels emerge specifically during BR rise?                    | Channel creation rate (join_date) over time; segment by whether channel ever posted BR                    | channels_gaming (join_date) + channel's genre history               | Did channel creation rate stay elevated post-2018?         |
| ⭐⭐       | 1.5   | Did BR content diversify over time (e.g., Fortnite Creative, tournaments)?     | Keyword frequency in titles/descriptions: "creative," "tournament," "competitive," "custom" for BR videos | metadata (title, description) filtered to BR                        | Did diversification increase through 2019?                 |
| ⭐        | 1.6   | Did BR videos have different "viral potential" (view distribution shape)?      | Compare view count distributions (log scale, Gini coefficient) for BR vs other genres                     | metadata (view_count) by subgenre                                   | Stable difference or convergence?                          |

*Key Visualizations for Act 1:*
•⁠  ⁠*"The Explosion"*: Normalized video volume by genre (2014–2019), BR release dates annotated
•⁠  ⁠*"Market Share Evolution"*: Stacked area of genre proportions over time
•⁠  ⁠*"Rising Tide?"*: Total gaming video count with BR share overlay

---

## *ACT 2: CREATOR RESPONSE*
"How did YouTube creators adapt to the BR phenomenon — and did those behaviors stick?"

This act focuses on supply-side dynamics: who made BR content, whether they pivoted from other genres, whether BR was a growth accelerator, and whether creators behaved differently (opportunism, formats, tactics).

| Priority | RQ ID | Research Question                                                              | Plot/Analysis                                                                                                                                        | Data Required                                                       | Persistence Check                                       |
| -------- | ----- | ------------------------------------------------------------------------------ | ---------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------- | ------------------------------------------------------- |
| ⭐⭐⭐      | 2.1   | Did posting BR videos accelerate channel growth?                               | Difference-in-differences: compare delta_subs trajectories for channels before/after first BR video vs. matched controls who never posted BR         | timeseries_gaming + first BR upload date per channel                | Did growth advantage persist 6–12 months post-first-BR? |
| ⭐⭐⭐      | 2.2   | Did existing creators pivot to BR content?                                     | Identify pre-2017 channels; track their genre composition over time; quantify pivot rate                                                             | metadata_single_game_identified (channel_id, subgenre, upload_date) | Did pivoters stay in BR through 2019 or return?         |
| ⭐⭐⭐      | 2.3   | Were BR-focused creators more "opportunistic"? *(Henry)*                       | Compare metrics: (a) upload frequency / subscriber ratio, (b) posting consistency (variance), (c) tag count per video, (d) genre diversity over time | timeseries (activity, videos, subs) + metadata (tags)               | Did opportunistic behavior decrease as BR matured?      |
| ⭐⭐       | 2.4   | Did creators abuse BR tags for visibility (tag-stuffing)?                      | Compare: videos with BR game name in tags vs. videos classified as BR by your model; ratio over time                                                 | tags field vs. classifier labels                                    | Did tag abuse decline as genre saturated?               |
| ⭐⭐       | 2.5   | Did BR introduce new video formats (length, frequency)?                        | Compare distributions: video duration, inter-upload intervals for BR vs. other genres                                                                | metadata (duration, upload_date) by channel and subgenre            | Did other genres converge toward BR patterns?           |
| ⭐⭐       | 2.6   | Did BR accelerate shift from "pure gameplay" to "challenge/narrative" formats? | Keyword prevalence in titles: "challenge," "no [X]," "only [Y]," "win with," "funny moments" — BR vs. others                                         | metadata (title) by subgenre                                        | Did challenge format spread to non-BR?                  |
| ⭐⭐       | 2.7   | Did traditional games adopt BR modes, and did it boost their content?          | Track COD videos mentioning "blackout" (Oct 2018+); compare COD channel metrics pre/post Blackout                                                    | tags/description keyword search + timeseries                        | Did Blackout boost sustain through 2019?                |
| ⭐        | 2.8   | Did Fortnite's Creator Code program drive content volume?                      | Frequency of "creator code," "support-a-creator," "use code" in Fortnite video descriptions over time                                                | description field, Fortnite videos only                             | Sustained or one-time spike?                            |
| ⭐        | 2.9   | Did channel "genre purity" predict success during BR era?                      | Compare growth trajectories: specialists (>80% one genre) vs. generalists; segment by whether they included BR                                       | channel genre composition + timeseries                              | Which strategy won long-term?                           |

*Key Visualizations for Act 2:*
•⁠  ⁠*"The Pivot"*: Sankey diagram of creator genre migration (pre-BR primary genre → post-BR primary genre)
•⁠  ⁠*"Growth Accelerator?"*: Diff-in-diff plot showing subscriber trajectories for BR-adopters vs. controls
•⁠  ⁠*"Opportunism Index"*: Distribution comparison of upload frequency/subscriber ratio by genre focus
•⁠  ⁠*"Format Evolution"*: Video duration distributions over time, faceted by genre

---

## *ACT 3: AUDIENCE SHIFTS*
"Did viewers migrate to BR, and how did community dynamics change?"

This act focuses on demand-side dynamics: where viewers came from, whether they abandoned other genres, how engagement patterns differed, and whether communities restructured.

| Priority | RQ ID | Research Question                                                             | Plot/Analysis                                                                                                                                             | Data Required                                                                         | Persistence Check                                           |
| -------- | ----- | ----------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------- | ----------------------------------------------------------- |
| ⭐⭐⭐      | 3.1   | Did BR steal audience from other genres?                                      | Cross-genre view share over time; correlation analysis between BR rise and other genres' delta_views                                                      | timeseries_gaming (delta_views) aggregated by subgenre                                | Did "victim" genres recover in 2019?                        |
| ⭐⭐⭐      | 3.2   | Did commenters migrate from other gaming communities to BR?                   | Track anonymized author IDs: identify users who commented on non-BR gaming pre-2017, then appeared on BR videos post-2017                                 | youtube_comments (author, video_id) + video genre labels                              | Did migrants stay in BR or return to original communities?  |
| ⭐⭐⭐      | 3.3   | Were BR commenters new to YouTube gaming, or existing gamers?                 | Classify commenters: (a) "BR-native" (first comment on BR), (b) "migrant" (prior non-BR history), (c) "tourist" (commented on BR but primarily elsewhere) | youtube_comments + chronological first-comment analysis                               | Did BR-native proportion stay high or did community mature? |
| ⭐⭐       | 3.4   | Did engagement dynamics differ for BR content?                                | Compare by genre: like/dislike ratio, comments per view, unique_authors per video, likes per comment                                                      | metadata (like_count, dislike_count, view_count) + num_comments, num_comments_authors | Did BR engagement patterns persist or normalize?            |
| ⭐⭐       | 3.5   | Did BR's "highlight moment" nature favor short-form, high-engagement content? | Correlation: video duration vs. engagement metrics (views, likes, comments) — compare slopes for BR vs. others                                            | metadata (duration, view_count, like_count) + num_comments                            | Stable pattern or convergence?                              |
| ⭐⭐       | 3.6   | Did specific genres suffer disproportionately from BR's rise?                 | Per-genre analysis: FPS, MOBA, Sandbox — growth rate pre-BR (2015–2016) vs. during-BR (2017–2018) vs. post-peak (2019)                                    | timeseries by subgenre                                                                | Which genres recovered vs. structurally declined?           |
| ⭐        | 3.7   | Did BR foster different community dynamics (toxicity/positivity)?             | Compare like/dislike ratios on videos; comment likes distribution                                                                                         | metadata (like_count, dislike_count) + youtube_comments (likes)                       | Stable community character or evolution?                    |
| ⭐        | 3.8   | Did BR impact Nintendo gaming content viewership?                             | Volume and engagement trends for Nintendo subgenre (Smash Bros, Zelda) during BR era                                                                      | metadata + timeseries filtered to Nintendo                                            | Recovery or sustained impact?                               |

*Key Visualizations for Act 3:*
•⁠  ⁠*"Audience Theft"*: Genre view share over time (stacked area, 100% normalized)
•⁠  ⁠*"Commenter Migration"*: Alluvial/flow diagram showing commenter movement between genre communities
•⁠  ⁠*"The Victims"*: Small multiples showing growth trajectories for each non-BR genre, with BR overlay for reference
•⁠  ⁠*"Engagement Fingerprint"*: Radar chart comparing engagement metrics (like ratio, comment rate, etc.) by genre

---

## *Summary: Consolidated Research Questions*

| Act             | # of RQs | High Priority (⭐⭐⭐) | Medium (⭐⭐) | Lower (⭐) |
| --------------- | -------- | ------------------- | ----------- | --------- |
| Act 1: Eruption | 6        | 3                   | 2           | 1         |
| Act 2: Creators | 9        | 3                   | 5           | 1         |
| Act 3: Audience | 8        | 3                   | 4           | 1         |
| *Total*         | *23*     | *9*                 | *11*        | *3*       |

---

## *Recommended Execution Order*

### *Phase 1: Foundation (Do First — Establishes the Story)*
 1.⁠ ⁠*RQ 1.1* — BR growth trajectory (the headline)
 2.⁠ ⁠*RQ 1.2* — Game-level breakdown (Fortnite vs PUBG narrative)
 3.⁠ ⁠*RQ 3.1* — Audience theft (the tension/stakes)
 4.⁠ ⁠*RQ 1.3* — Zero-sum vs. rising tide (contextualizes 3.1)

### *Phase 2: Creator Deep-Dive*
 5.⁠ ⁠*RQ 2.2* — Creator pivots (human angle)
 6.⁠ ⁠*RQ 2.1* — BR as growth accelerator (incentive structure)
 7.⁠ ⁠*RQ 2.3* — Opportunism analysis *(Henry's focus)*
 8.⁠ ⁠*RQ 2.5* — Format changes

### *Phase 3: Audience Deep-Dive*
 9.⁠ ⁠*RQ 3.2* — Commenter migration (requires heavy data processing)
10.⁠ ⁠*RQ 3.3* — BR-native vs. migrant commenters
11.⁠ ⁠*RQ 3.6* — Genre-specific victim analysis

### *Phase 4: Polish & Nuance*
12.⁠ ⁠Remaining RQs as time permits, prioritizing those with clearest findings from earlier phases

---

## *Persistence Framing (for Write-Up)*

For each major finding, explicitly state one of:

| Pattern                  | Interpretation                                 | Example                                                               |
| ------------------------ | ---------------------------------------------- | --------------------------------------------------------------------- |
| *Continued acceleration* | BR's impact was still intensifying at data end | "BR video volume was still growing 15% MoM in Sept 2019"              |
| *Sustained plateau*      | Change appears structural, no reversion        | "FPS viewership share stabilized at ~60% of pre-BR levels"            |
| *Signs of reversion*     | Impact may have been transient                 | "Pivoted creators began returning to original genres in mid-2019"     |
| *Insufficient data*      | Cannot distinguish inertia from permanence     | "12 months post-peak is insufficient to assess long-term equilibrium" |
