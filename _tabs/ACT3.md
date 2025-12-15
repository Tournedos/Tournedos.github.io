---
layout: page
icon: fas fa-stream
order: 4
title : ACT 3 - Audience shift
---
<style>
.plot-container {
  width: 100%;
  max-width: 1100px;   /* control horizontal size */
  margin: 2rem auto;
}
.plot-container iframe {
  width: 100%;
  height: 600px;       /* THIS is the key line */
  border: none;
}
</style>

<h1 style="color:#003c9e; font-size:3rem; font-weight:700;">Page title</h1>
<h2 style="color:#003c9e; font-size:2rem; font-weight:600;">Section title</h2>
<h3 style="color:#4f6fd6; font-size:1.5rem; font-weight:500;">Subsection title</h3>

<div style="display: flex; align-items: center; gap: 2rem;">
  <h1 style="color:#003c9e; font-size:3rem; font-weight:600;">
  Viewers migration to Battle Royale content & Community Dynamics changes
  </h1>
  <img src="/assets/img/img_3/comment.png" alt="Scheme" style="width:1000px; height:auto;">
</div>

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
**idee blague : preprocessing killed our computer, 2 computers.**
Why should you trust us? Why us and not some random “data guru” on YouTube? Because we didn’t just skim the surface—we went deep into the comments. The YouNiverse dataset isn’t only videos and channels; it contains billions of actual user comments. Handling it was a challenge: decompressing the full comments archive on a single machine took 45 hours of non-stop CPU grinding. It’s messy, it’s massive, but it’s real. That’s why our insights on engagement, community migration, and audience behavior are solid—because we saw what people actually said, not just the metadata.


**introduction of ACT3**
Now that we have analyzed how the emergence of Battle Royale impacted the gaming ecosystem of YouTube and how the creators of content reacted, we're going to focus on what happened at the viewers level. The goal is to observe whether Battle Royale genre stole aucience from other genres, or even if commenters migrated from other gaming communitites to the Battle Royale genre. In addition to that, we can ask whether the engagement dynamic of the Battle Royale community differs from other genres, and which factors influence this shift in which type of content the viewers want to consumme. In addition, it will be interesting to see if the communities of the Battle Royale games show different behaviors compared to the other genres, like more positivity/happy or more toxicity/hate.

<div class="question-box">
  <div class="question-box-title">Key Questions</div>
  <ul>
    <li>Did Battle Royale genre steal audience from other genres ?</li>
    <li>Did commenters migrate from other gaming communities to the Battle Royal genre ? Or were Battle Royale commenters new to YouTube gaming ?</li>
    <li>Did engagement dynamics differ for BR content?</li>
    <li>Did BR introduce new video formats (length, frequency) ?</li>
  </ul>
</div>

<h2 style="color:#003c9e; font-size:2rem; font-weight:600;">3.1 - Did Battle Royale genre steal audience from other genres ?</h2>
<h2 style="color:#003c9e; font-size:2rem; font-weight:600;">3.2 - Did commenters migrate from other gaming communities to the Battle Royal genre ? Or were Battle Royale commenters new to YouTube gaming ?</h2>

<h2 style="color:#003c9e; font-size:2rem; font-weight:600;">3.3 Did engagement dynamics differ for BR content?</h2>
<div class="plot-container">
Now we focus on engagement dynamics in Battle Royale content. To do this, we analyze the ratio of likes per view (LPV), which reflects how actively viewers respond to videos. Viewers who like content consistently can be considered more engaged than those who only watch.

  <iframe
    src="/assets/plots/plots_3/plot_3_3.html"
    loading="lazy"
    title="Plot 01 – Engagement by Genre"
  ></iframe>
</div>

Battle Royale clearly leads in audience engagement. From 2017 to 2019, its median likes per view far outpace all other subgenres. This means viewers aren’t just watching—they’re actively hitting the like button. We double-checked statistically, and yes, the difference is significant. In short: BR videos attract both eyes and clicks, explaining why creators raced to produce more of this content.


<h2 style="color:#003c9e; font-size:2rem; font-weight:600;">3.4 Did BR introduce new video formats (length, frequency) ?</h2>

Now that we have observed that the viewers were more enthusiastic for Battle Royal content than for the content of other genres, we can go further into the analysis. This enthusiasm can potentially be due to other factors than the genre itself. By that we mean that the way the Battle Royale videos are produced may differ from the other genres which could be the cause of the enthusiasm and not only the genre itself. Potential factors that we will explore are the duration or the frequency at which the creators upload videos.

est-ce que la duration of videos is significantly different -> box plot

est-ce que la fréquence à laquelle ils upload significantly different -> box plot

if not different -> think that the genre is attractive

if different -> what is different -> could be a factor that influence the enthusiasm

to define whether the enthusiasm comes from the genre only or whe
