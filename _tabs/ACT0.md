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

<h2 style="color:#003c9e; font-size:1.5rem; font-weight:900 !important;">
  What defines a Battle Royale game?
</h2>

In this project, we define Battle Royale (BR) games as a specific subgenre of online multiplayer games where a large number of players compete in the same match with a single objective: be the last player (or team) alive. Although implementations differ from game to game, most Battle Royale titles share a common set of mechanics:



<figure>
  <figcaption style="text-align: center;color: #666666; font-style: italic;">
  Core mechanisms of a battle royale game</figcaption>
  <img src="/assets/img/img_0/Scheme2.png" alt="Scheme" width="800px">
</figure>

From a content perspective, these characteristics make Battle Royale games extremely YouTube-friendly:  
they naturally generate clutch moments, comebacks, chaotic endgames, and highlight-worthy plays, which are ideal for short-form clips, montages, and high-intensity streams.

<h2 style="color:#003c9e; font-size:1.5rem; font-weight:900 !important;">
  A short historical background of the Battle Royale genre
</h2>

The idea behind Battle Royale in games predates the genre label itself. On the fiction side, many authors and films explored “last-person-standing” death games. A clear reference point in game journalism is Koushun Takami’s 1999 novel Battle Royale and its 2000 film adaptation, in which a group of students is forced to fight until only one survives. Several game journalists explicitly link the structure of modern Battle Royale games to this story template.

On the game design side, the genre evolved from mods for survival and sandbox games in the early 2010s. Key early experiments included:

- Community “Hunger Games” / Survival Games plugins for Minecraft around 2012.
- DayZ and later Arma 2 / Arma 3 survival mods.
- Brendan “PlayerUnknown” Greene’s Battle Royale mods, introducing large lobbies, random loot, and a shrinking safe zone on military-style maps.
- H1Z1: King of the Kill (2015), one of the first standalone shooters built fully around this format.

The modern Battle Royale “boom” occurred in the mid-to-late 2010s, with widely recognized milestones:

- 2017 — PlayerUnknown’s Battlegrounds (PUBG) brings the mod formula to a commercial Steam release, popularizing the now-standard loop: ~100 players drop from a plane, loot, and fight inside a shrinking circle.
- 2017 — Fortnite Battle Royale launches as a free mode, quickly reaching a wider audience than PUBG, helped by its accessibility, building mechanics, and cross-platform support.
- 2019–2020 — Apex Legends and Call of Duty: Warzone integrate Battle Royale into large existing franchises, attracting tens of millions of players within weeks, confirming BR as a mainstream competitive format. Of course we are not able to study the boom brought by Warzone since the dataset stops before it's official release.

In this project, we focus on the modern wave of Battle Royale titles (from H1Z1, PUBG, and Fortnite onwards) and study how their rise reshaped YouTube gaming content.


<h2 style="color:#003c9e; font-size:2rem; font-weight:900 !important;">
    Project guidelines and research questions
</h2>

Our goal is to tell a structured, data-driven story about how Battle Royale (BR) games enter and reshape YouTube gaming.
To do this, we organize the project into five main steps, each with its own guiding questions:

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

<div class="question-box" style="display:flex; gap:2rem;">
  <a href="/act1/" style="text-align:center; color: inherit; text-decoration: none;border-bottom:none;">
    <div style="font-size:2rem; font-weight:bold;">ACT 1</div>
    <div>THE ERUPTION</div>
    <small>“How did BR explode onto YouTube’s gaming landscape, and did the momentum persist?”</small>
  </a>
  <a href="/act2/" style="text-align:center; color: inherit; text-decoration: none;border-bottom:none;">
    <div style="font-size:2rem; font-weight:bold;">ACT 2</div>
    <div>CREATOR RESPONSE</div>
    <small>“How did YouTube creators adapt to the BR phenomenon, and did those behaviors stick?”</small>
  </a>
  <a href="/act3/" style="text-align:center; color: inherit; text-decoration: none;border-bottom:none;">
    <div style="font-size:2rem; font-weight:bold;">ACT 3</div>
    <div>AUDIENCE SHIFTS</div>
    <small>“Did viewers migrate to BR, and how did community dynamics change?”</small>
  </a>
</div>

<figure>
  <img src="/assets/img/img_0/Scheme1.png" alt="Scheme" width="600px">
  <figcaption style="text-align: center;color: #666666; font-style: italic;">Overview of Battle Royale emergence and impact, following the YouNiverse Timescale</figcaption>
</figure>


<h2 style="color:#003c9e; font-size:2rem; font-weight:900 !important;">
    Selecting our game panel from Twitch
</h2>

To decide which games actually matter in our analysis, we start from Twitch rather than YouTube. We use the public Kaggle dataset “Top games on Twitch 2016–2023” by Kartik Kirsh, which lists the monthly top 200 games on Twitch together with hours watched, hours streamed and average viewers [Twitch Dataset](https://www.kaggle.com/datasets/rankirsh/evolution-of-top-games-on-twitch).

From this dataset we build our game panel in four main steps:

<h2 style="color:#003c9e; font-size:1.5rem; font-weight:900 !important;">
    Time window and cleaning
</h2>
<h3 style="color:#003c9e;"> Time window and cleaning</h3>

- We keep only the years 2016–2019, which cover the main rise of modern Battle Royale titles.  
- We drop non-game categories (e.g. Just Chatting, Special Events, Creative, Poker), so that we only track actual video games.


<h3 style="color:#003c9e;"> Aggregate popularity per licence</h3>

- For each game, we sum hours watched over all months in 2016–2019.  
- We then merge yearly releases into a single licence (e.g. all FIFA entries → FIFA, all Call of Duty entries → Call of Duty) and recompute total hours watched per licence.


<h3 style="color:#003c9e;"> Top-50 core panel</h3>

- We rank licences by total hours watched and keep the top 50.  
- These 50 licences form our core panel of games that actually structure Twitch viewership during the Battle Royale era.

<h3 style="color:#003c9e;"> Manual genre annotation</h3>


- Each licence is manually mapped to one of our high-level genres:  
  Battle Royale, FPS, MOBA, Sports, Sandbox, MMORPG, Strategy, Single Player / Open World, Nintendo, Card / CCG, Fighting, Horror.  
- The result is stored in `data/filtered/twitch/games_selected.csv`.

Within this panel, licences annotated as Battle Royale (e.g. H1Z1 / Z1: Battle Royale, PLAYERUNKNOWN’S BATTLEGROUNDS, Fortnite, Apex Legends) form our BR game set, which we will later try to trace on YouTube using genre classification.

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

<h2 style="color:#003c9e; font-size:2.0rem; margin-top:2rem;">From YouTube metadata to clean game-genre panels</h2>

So far, we have defined our 12 game genres and built a Twitch-based top-50 game panel. We now need to find the corresponding videos on YouTube and keep only those that clearly belong to one genre.

We rely on the YouNiverse dataset and use only its English gaming subset:

- `yt_metadata_en`: video-level metadata (title, description, tags, upload date, views…)
- `df_channels_en` and `df_timeseries_en`: to filter channels labelled as Gaming
- num_comments` / `num_comments_authors`: comment activity

After restricting to gaming videos, we obtain about 13.7 million YouTube gaming videos. From there, our pipeline has three main steps.

<h3 style="color:#003c9e;">Step 1 : Building a high-precision reference set (single-game videos)</h3>

To train genre classifiers without manual labeling, we first construct a reference dataset of single-game videos:

- We merge each video’s title, description and tags into a single searchable string.
- We scan this text with a master regex containing all known variants of the top-50 games  
  (e.g. pubg | playerunknown's battlegrounds | gta v | gta 5 | grand theft auto v).
- Using a synonyms dictionary, every match is mapped back to a canonical game name, which is then mapped to exactly one of our 12 genres.
- We only keep videos that mention exactly one tracked game:
  - videos with no game mention are dropped;
  - videos mentioning several games (even within the same genre) are also removed, to avoid ambiguous labels.

This conservative filtering yields a very clean reference set of around 3.8M videos (≈28% of the 13.7M gaming videos). Each of these videos is then given a subgenre label based on the detected game.

<h3 style="color:#003c9e;">Step 2 : Training genre classifiers on metadata</h3>

From this single-game reference set, we train one binary classifier per genre (12 models in total):

- Positive class: videos whose detected game belongs to that genre.
- Negative class: videos from all other genres.
- To keep training balanced and efficient, we downsample to at most 50k positives + 50k negatives per genre.

Each model combines two types of features:

- TF-IDF representations of cleaned title, description and tags.
- Genre-specific vocabulary scores, built from curated dictionaries of key terms, game names and typical expressions.

A logistic regression classifier is trained on the resulting feature matrix. Internal validation shows that this hybrid representation systematically outperforms TF-IDF or vocabulary scores alone.

<h3 style="color:#003c9e;">Step 3 : Classifying the full YouTube gaming set and enforcing a single-genre rule</h3>

We apply the 12 trained classifiers to all 13.7M gaming videos.  
A video is considered classified if at least one model predicts it as positive, which yields about 6.6M classified videos (≈48%).

To obtain disjoint panels:

- For each video, we count how many genres predicted it as positive.
- We keep videos with exactly one positive genre label and store them in single_genre_videos.csv.
- Videos with two or more positive labels are stored in multi_genre_videos.csv and excluded from the main analysis.

After this filtering step, we obtain 12 clean, non-overlapping YouTube genre panels. These panels form the basis for all subsequent analyses on how the rise of Battle Royale reshapes the broader gaming ecosystem on YouTube.

<h3 style="color:#003c9e;">Step 4 : Detecting channel-level genre phases over time</h3>

Rather than assigning a fixed genre to each channel, we model how creators’ focus evolves over time by detecting
genre phases. This approach captures specialization, diversification, and genre pivoting
(e.g. FPS → Battle Royale), which cannot be inferred from individual videos alone.

For each video upload, we apply the following procedure:

- Consider the last 21 videos uploaded by the channel
- Compute the genre distribution within this rolling window
- If one genre exceeds 50%, assign the channel to that genre’s phase
- Otherwise, label the channel as genreless (diverse or experimental content)

Phase boundaries are stored as
<code>(channel_id, genre, start_date, end_date, video_count)</code>.

We tested window sizes of 11, 21, and 31 videos. A window of 21 videos provides the best balance:

- filters out short-lived experiments
- captures sustained genre commitment
- detects early Battle Royale adoption without excessive noise

The resulting file (<code>all_channel_phases.csv</code>) contains a complete timeline of genre phases per channel
and forms the basis for all subsequent analyses of creator behavior.

