---
layout: page
icon: fas fa-stream
order: 4
title: ACT 3 - Audience Shift
---

<style>
.plot-container {
  width: 100%;
  max-width: 1100px;
  margin: 2rem auto;
}
.plot-container iframe {
  width: 100%;
  height: 600px;
  border: none;
}

.plot-card {
  max-width: 1100px; 
  margin: 2rem auto;
  padding: 1.2rem 1.4rem;
  /*border-radius: 1rem;
  border: 1px solid rgba(0,0,0,0.15);*/
  background: #ffffff;
  /*box-shadow: 0 4px 14px rgba(0,0,0,0.08);*/
}
.plot-card iframe {
  width: 100%;
  height: 75vh;
}

html.dark .plot-card {
  border: 1px solid rgba(180,196,255,0.35);
  background: linear-gradient(135deg, #050814, #0c1024);
  box-shadow: 0 14px 30px rgba(0,0,0,0.4);
}

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


<div style="display: flex; align-items: center; gap: 2rem;">
  <h1 style="color:#003c9e; font-size:3rem; font-weight:700;">
    Audience Shifts: Did Viewers Migrate to Battle Royale, and How Did Communities Change?
  </h1>
  <img src="/assets/img/img_3/comment.png" alt="Scheme" style="width:850px; height:auto; border-radius:18px;">
</div>


Act 1 showed how Battle Royale (BR) reshaped the ecosystem of YouTube gaming.  
Act 2 uncovered how creators adapted to this new environment.  

Now comes the final layer of the puzzle: the viewers themselves.  
To what extent did BR attract new audiences, pull viewers away from other genres, or reshape engagement and community dynamics?

Battle Royale was not just a genre, it became a gravitational force. In this act, we study how attention, commenters, and sentiment migrated during the BR explosion.


<div class="question-box">
  <div class="question-box-title">Key Questions</div>
  <ul>
    <li>Did the Battle Royale genre steal audience from other gaming communities?</li>
    <li>Were BR commenters originally from other genres, or were they new to YouTube gaming?</li>
    <li>Did BR content trigger different engagement dynamics?</li>
    <li>Did BR introduce new video formats (length, frequency)?</li>
  </ul>
</div>

<blockquote style="font-style:italic; opacity:0.85;">
  Fun fact: preprocessing the full YouNiverse comments archive literally killed two of our computers.  
  Battle Royale wasn’t the only thing causing explosions in 2017.
</blockquote>


<!-- 3.1 — AUDIENCE STEALING EFFECT -->

<div style="display:flex; justify-content:center; margin:2rem 0;">
  <img 
    src="/assets/img/img_3/battle_comments.png" 
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

<h2 style="color:#003c9e; font-size:2rem; font-weight:600;">Did Battle Royale Steal Audience From Other Genres?</h2>

To determine whether BR captured viewers from existing communities, we track the movement of comment authors across genres.  
If BR rapidly accumulated commenters whose first interactions were in other genres (FPS, Sandbox, MOBA, etc.), this would indicate a redistribution of audience attention rather than the arrival of new people.

A first step is to determine whether newcomers to YouTube gaming disproportionately entered through BR.  
To do this, we identify the genre of each user's first-ever comment, and compare the distribution across genres.

Because comment timestamps are unavailable, we approximate comment timing by the upload date of the commented video.  This is a reasonable assumption: most comments are written shortly after publication, especially by active users.  While imperfect for low-activity accounts, the approximation holds at the large scale required for this analysis.


<!-- FIGURE: Entry points into the ecosystem -->
<div class="plot-card">
  <iframe
    src="/assets/plots/plots_3/plot_3_1.html"
    loading="lazy"
    title="Entry Points of New Commenters by Genre"
  ></iframe>
</div>


If BR acted as an entry gateway, we would expect BR to dominate first-user comments.  
If instead BR’s rise was mainly fueled by migration from other genres, the first comments would cluster around Sandbox, FPS, or MOBA.


---

<div style="display:flex; justify-content:center; margin:2rem 0;">
  <img 
    src="/assets/img/img_3/fortnite_detective.png" 
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

<h3 style="color:#4f6fd6; font-size:1.5rem; font-weight:500;">Following Users Across Genres</h3>


Beyond identifying entry points, we want to know whether BR had an addictive effect:  
Did users who commented a BR video first keep consuming BR content afterwards?

Conversely, did users who started in FPS or Sandbox stay loyal to their original genre, or did they gradually shift toward BR?

Tracking users across time reveals whether BR functioned as a sticky community or merely a temporary curiosity.


<!-- FIGURE: Migration flows -->
<div class="plot-card">
  <iframe
    src="/assets/plots/plots_3/plot_3_2.html"
    loading="lazy"
    title="Migration of Commenters Across Genres"
  ></iframe>
</div>


These flows allow us to quantify how much BR’s explosion resulted from internal migration versus external newcomers, a crucial distinction to understand the cultural impact of the genre.


<!-- 3.2 — MIGRATION OR NEW USERS? -->

<h2 style="color:#003c9e; font-size:2rem; font-weight:600;">Did Commenters Migrate to BR, or Were They New to YouTube Gaming?</h2>

*Coming soon: integration of your results.*  

This section will contrast:
- retained users from other genres
- new users entering through BR
- cross-genre drifters whose commenting history shifted

It will serve as a bridge toward engagement dynamics.


<!-- 3.3 — ENGAGEMENT DYNAMICS -->

<h2 style="color:#003c9e; font-size:2rem; font-weight:600;">Did Engagement Dynamics Differ for BR Content?</h2>

To evaluate whether BR fostered stronger audience engagement, we compute the likes-per-view ratio (LPV).  
This metric reflects how actively viewers interact with videos: passive viewers only watch, but engaged viewers watch + react.

If BR displays higher LPV values, it suggests that BR content cultivated a particularly enthusiastic and reactive audience.


<div class="plot-card">
  <iframe
    src="/assets/plots/plots_3/plot_3_3.html"
    loading="lazy"
    title="Plot 3.3 – Engagement by Genre"
  ></iframe>
</div>


Battle Royale clearly dominates the LPV distribution during 2017–2019.  
Viewers weren’t just watching—they were liking, consistently and intensely.  
Statistical testing confirms the difference: comparing BR to Sandbox (the second most engaging genre) through independent t-tests for 2018 and 2019 shows a significant gap in median engagement.


---

<h3 style="color:#4f6fd6; font-size:1.5rem; font-weight:500;">Are Video Formats Responsible for This Difference?</h3>

To determine whether BR’s high engagement stems from its content format rather than the genre itself, we examine:

- video duration
- upload frequency

If BR videos are significantly shorter, longer, or more frequent, these structural differences could explain engagement patterns.


<div class="plot-card">
  <iframe
    src="/assets/plots/plots_3/plot_3_4.html"
    loading="lazy"
    title="Video Duration Comparison Across Genres"
  ></iframe>
</div>


Long outliers (up to 100,000 seconds) appear in both BR and FPS—usually stream replays.  
Removing them reveals a tighter distribution: all major genres produce videos in the 8–16 minute range.

This strongly suggests that BR creators did not adopt a specific video format responsible for boosting engagement.  
Thus, the enthusiasm for BR content likely stems from the genre itself, not from fundamentally different production strategies.

