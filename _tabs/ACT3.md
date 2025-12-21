---
layout: page
icon: fas fa-stream
order: 4
title: ACT 3 - Audience Shift
permalink: /act3/
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
  background: #ffffff;
}
.plot-card iframe {
  width: 100%;
  height: 80vh;
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

<style>
.slider {
  display: flex;
  overflow-x: auto;
  scroll-snap-type: x mandatory;
  scroll-behavior: smooth;
  width: 100%;
  max-width: 1100px;
  margin: 2rem auto;
}
.slider::-webkit-scrollbar { 
  display: none; 
}
.slide { 
  min-width: 100%; 
  scroll-snap-align: start; 
}
.slide iframe { 
  width: 100%; 
  height: 75vh; 
  border: none; 
}
.slider-dots {
  display: flex;
  justify-content: center;
  margin-top: 1rem;
  gap: 10px;
}
.slider-dot {
  width: 10px;
  height: 10px;
  border-radius: 50%;
  background: #c7d2f0;
  opacity: 0.6;
  transition: transform 0.2s ease, opacity 0.2s ease;
  display: inline-block;
}
.slider-dot:hover {
  opacity: 1;
  background: #657dccff;
  transform: scale(1.2);
}
</style>

<!-- HEADER + IMAGE -->
<div style="display: flex; align-items: center; gap: 2rem;">
  <h1 style="color:#003c9e; font-size:3rem; font-weight:700;">
    Audience Shifts:  
    Did Viewers Migrate to Battle Royale, and How Did Communities Change?
  </h1>
  <img src="/assets/img/img_3/comment.png"
       alt="Audience comments illustration"
       style="width:850px; height:auto; border-radius:18px;">
</div>

<p>
After analyzing how Battle Royale reshaped the YouTube gaming ecosystem in Acts 1 and 2,
we now focus on the viewers themselves.
The objective is to determine whether Battle Royale attracted a new population of active commenters,
or whether it pulled attention away from pre-existing gaming communities.
</p>

<div class="question-box">
  <div class="question-box-title">Key Questions</div>
  <ul>
    <li>
      <a href="#audience-steal" style="color:white; text-decoration:none; border-bottom:none;">
        Did the Battle Royale genre attract new viewers, or did it steal audience from existing gaming communities?
      </a>
    </li>
    <li>
      <a href="#commenter-origin" style="color:white; text-decoration:none; border-bottom:none;">
        Were Battle Royale commenters already active in other genres, or did they enter YouTube gaming through BR?
      </a>
    </li>
    <li>
      <a href="#engagement-dynamics" style="color:white; text-decoration:none; border-bottom:none;">
        Did Battle Royale content generate different engagement dynamics compared to other genres?
      </a>
    </li>
  </ul>
</div>

<blockquote style="font-style:italic; opacity:0.85;">
Preprocessing the full YouNiverse comments archive (77GB) pushed our machines to their limits.
Battle Royale isn't the only exploding thing, our laptops too...
</blockquote>

<!-- ================================================= -->
<!-- 3.1 -->
<h2 id="audience-steal" style="color:#003c9e; font-size:2rem; font-weight:600;">
(3.1) Were Battle Royale commenters new to YouTube gaming?
</h2>

<p>
To address this question, we analyze the genre associated with each author’s
<strong>first-ever gaming comment</strong>.
Because comment timestamps are unavailable, we approximate timing using the upload date
of the commented video.
This approximation is reliable for active users, who typically comment shortly after publication.
</p>

<h3 style="color:#4f6fd6; font-size:1.5rem; font-weight:500;">
  (3.1.1) Was the emergence of Battle Royal accompagnied by the emergence of a group of active users?
</h3>

<p>
By identifying entry genres, we assess whether the emergence of Battle Royale coincided
with the arrival of a new population of engaged commenters.
</p>

<!-- FIG 3.1.1 – Genre entry points -->
<div class="slider">
  <div id="plot1" class="slide"><iframe src="/assets/plots/plots_3/plot-3-1-2.html"></iframe></div>
  <div id="plot2" class="slide"><iframe src="/assets/plots/plots_3/plot-3-1-1.html"></iframe></div>
  <div id="plot3" class="slide"><iframe src="/assets/plots/plots_3/plot-3-1-3.html"></iframe></div>
</div>

<div class="slider-dots">
  <a href="#plot1" class="slider-dot"></a>
  <a href="#plot2" class="slider-dot"></a>
  <a href="#plot3" class="slider-dot"></a>
</div>

<p>
The <strong>Genre Entry Points</strong> plot highlights the genre through which commenters first entered the YouTube gaming ecosystem. This analysis allows us to assess whether the rise of Battle Royale coincided with the emergence of a new community of active users. Entering through Battle Royale suggests that the genre itself acted as a gateway into YouTube gaming, potentially triggering strong initial engagement.
</p>

<p>
For less active authors, Sandbox is the dominant entry point, which is expected given its long-standing presence in the ecosystem. Nevertheless, Battle Royale emerges as a major secondary entry genre, indicating that a substantial number of users became active through this newly emerging genre. As we move toward more active authors, Sandbox and FPS gradually gain importance as entry points, while Battle Royale becomes relatively less dominant.
</p>

<p>
This shift can be explained by differences in user seniority. Highly active commenters are more likely to have been present on YouTube gaming before the rise of Battle Royale and therefore could not have entered the ecosystem through it. Overall, these results confirm that while Battle Royale played a key role in attracting new users, older and more active users were more likely to have entered through earlier-established genres.
</p>

<p>
In conclusion, Battle Royale emerges as a <strong>major entry point</strong> into the YouTube gaming ecosystem. Across all user activity levels, it consistently ranks among the most common genres for first-ever gaming comments. This indicates that the rise of Battle Royale was not only a redistribution of existing audiences, but also coincided with the arrival of a new population of active commenters, reshaping the dynamics of YouTube gaming communities.
</p>


<!-- IMAGE DE TRANSITION -->
<div style="display:flex; justify-content:center; margin:2rem 0;">
  <img src="/assets/img/img_3/battle_comments.png"
       alt="Battle Royale investigation illustration"
       style="width:90%; max-width:480px; border-radius:18px;">
</div>

<!-- ================================================= -->
<h3 style="color:#4f6fd6; font-size:1.5rem; font-weight:500;">
  (3.1.2) Did Battle Royale make commenters stick to the genre?
</h3>

<p>
We now examine whether commenters remained loyal to the genre of their first comment,
or whether they diversified their interests over time.
This allows us to evaluate the “hook” effect of Battle Royale compared to other genres.
</p>

<!-- FIG 11 / 12 / 13 – Retention matrices -->
<div class="slider">
  <div id="plot4" class="slide"><iframe src="/assets/plots/plots_3/plot-3-2-1.html"></iframe></div>
  <div id="plot5" class="slide"><iframe src="/assets/plots/plots_3/plot-3-2-2.html"></iframe></div>
  <div id="plot6" class="slide"><iframe src="/assets/plots/plots_3/plot-3-2-3.html"></iframe></div>
</div>

<div class="slider-dots">
  <a href="#plot4" class="slider-dot"></a>
  <a href="#plot5" class="slider-dot"></a>
  <a href="#plot6" class="slider-dot"></a>
</div>

<p>
By focusing on the three main entry genres (Sandbox, Battle Royale, and FPS) we observe clear differences in how commenters’ interests evolve over time. Authors who entered through Sandbox mostly remained within that genre, although a noticeable fraction later engaged with Battle Royale content. Battle Royale stands out as the most retentive genre: users who entered through BR were the most likely to continue interacting primarily with BR videos, suggesting the formation of a particularly loyal community. In contrast, FPS shows weaker retention, with many commenters gradually shifting their activity toward Battle Royale. Overall, these patterns indicate that Battle Royale not only retained its own audience more effectively than other genres, but also attracted users from FPS, pointing to a broader shift of community interest toward Battle Royale content. 
</p>

<div class="slider">
  <div id="plot7" class="slide"><iframe src="/assets/plots/plots_3/plot-3-2-11.html"></iframe></div>
  <div id="plot8" class="slide"><iframe src="/assets/plots/plots_3/plot-3-2-22.html"></iframe></div>
  <div id="plot9" class="slide"><iframe src="/assets/plots/plots_3/plot-3-2-33.html"></iframe></div>
</div>

<div class="slider-dots">
  <a href="#plot7" class="slider-dot"></a>
  <a href="#plot8" class="slider-dot"></a>
  <a href="#plot9" class="slider-dot"></a>
</div>

<p>
When focusing on authors with a higher level of activity (those who commented between 10 and 20 times), we observe patterns similar to the previous group but more pronounced. Sandbox commenters remain largely within their original genre, yet an increasing share of their activity shifts toward Battle Royale. FPS shows an even stronger change: retention within the genre weakens further, while migration toward Battle Royale becomes more substantial. Battle Royale itself continues to display strong loyalty, with most commenters remaining engaged with BR content. Overall, these results reinforce the idea that as user activity increases, the shift of interest toward Battle Royale becomes clearer. This trend motivates us to examine the most active authors to confirm whether this pattern continues.
</p>

<div class="slider">
  <div id="plot10" class="slide"><iframe src="/assets/plots/plots_3/plot-3-2-111.html"></iframe></div>
  <div id="plot11" class="slide"><iframe src="/assets/plots/plots_3/plot-3-2-222.html"></iframe></div>
  <div id="plot12" class="slide"><iframe src="/assets/plots/plots_3/plot-3-2-333.html"></iframe></div>
</div>

<div class="slider-dots">
  <a href="#plot10" class="slider-dot"></a>
  <a href="#plot11" class="slider-dot"></a>
  <a href="#plot12" class="slider-dot"></a>
</div>

<p>
For the most active authors, the same trends become even more pronounced. Sandbox pioneers show a gradual decline in loyalty to their original genre, with a growing share of their activity shifting toward Battle Royale. The effect is even stronger for FPS pioneers: retention within FPS weakens further, and a large fraction of their subsequent engagement moves to other genres, most notably Battle Royale. This confirms a clear community shift away from FPS content among highly active users, with Battle Royale emerging as the primary destination for this redirected attention.
</p>

<p>
In summary, Battle Royale shows the strongest retention, with users more likely to remain engaged than in other genres. Sandbox and FPS exhibit weaker loyalty, with many commenters gradually shifting toward Battle Royale. This effect strengthens with user activity, highlighting Battle Royale’s ability to sustain <strong>long-term</strong> engagement and community loyalty.
</p>



<div style="display:flex; justify-content:center; margin:2rem 0;">
  <img src="/assets/img/img_3/fortnite_detective.png"
       alt="Battle Royale investigation illustration"
       style="width:90%; max-width:480px; border-radius:18px;">
</div>

<!-- ================================================= -->
<!-- 3.2 -->
<h2 id="commenter-origin" style="color:#003c9e; font-size:2rem; font-weight:600;">
  (3.2) From which communities did Battle Royale commenters migrate?
</h2>

<p>
To isolate migration effects, we focus on users who commented on Battle Royale content
but did <strong>not</strong> enter the YouTube gaming ecosystem through this genre.
This allows us to identify from which pre-existing communities Battle Royale drew its audience.
</p>

<!-- FIG 14 – Sankey diagram -->
<div class="slider">
  <div id="plot13" class="slide"><iframe src="/assets/plots/plots_3/plot-3-3-1.html"></iframe></div>
  <div id="plot14" class="slide"><iframe src="/assets/plots/plots_3/plot-3-3-2.html"></iframe></div>
  <div id="plot15" class="slide"><iframe src="/assets/plots/plots_3/plot-3-3-3.html"></iframe></div>
</div>

<div class="slider-dots">
  <a href="#plot13" class="slider-dot"></a>
  <a href="#plot14" class="slider-dot"></a>
  <a href="#plot15" class="slider-dot"></a>
</div>

<p>
The Sankey diagrams illustrate how YouTube gaming commenters migrated toward Battle Royale content. Each flow represents users who initially engaged with one genre before later commenting on at least one Battle Royale video. The diagrams reveal that most Battle Royale commenters did not emerge in isolation, but rather transitioned from other established gaming communities.
</p>

<p>
The largest sources of migration come from Sandbox and FPS, confirming patterns observed earlier in the analysis. These genres act as the main reservoirs of users who later engage with Battle Royale. At the same time, the presence of smaller flows from a wide range of other genres (such as Single Player / Open World, Sports, MOBA, and Nintendo) shows that Battle Royale attracted users with diverse gaming interests. This highlights Battle Royale’s role not only as a dominant genre, but also as a cross-genre hub capable of unifying audiences from across the YouTube gaming ecosystem.
</p>

<!-- ================================================= -->
<h3 style="color:#4f6fd6; font-size:1.5rem; font-weight:500;">
  (3.2.2) How did this migration evolve over time?
</h3>

<p>
We now analyze how this redistribution of attention unfolded over time.
By tracking FPS and Sandbox pioneers, we measure how the share of their comments
devoted to Battle Royale evolved during the BR boom.
</p>

<!-- FIG 15 / 16 – Migration over time -->
<div class="slider">
  <div id="plot16" class="slide"><iframe src="/assets/plots/plots_3/plot-3-4-1.html"></iframe></div>
  <div id="plot17" class="slide"><iframe src="/assets/plots/plots_3/plot-3-4-2.html"></iframe></div>
</div>

<div class="slider-dots">
  <a href="#plot16" class="slider-dot"></a>
  <a href="#plot17" class="slider-dot"></a>
</div>

<p>
Once again, FPS appears to be strongly impacted by the emergence of Battle Royale. As Battle Royale content gains momentum, a growing share of comments originally directed at FPS videos progressively shifts toward BR, following the same temporal pattern identified in Act 1. This shift peaks during the core years of the Battle Royale boom and then slightly recedes, indicating that part of the FPS audience redirected its attention rather than fully abandoning the genre.
</p>

<p>
The pattern differs somewhat for Sandbox content. Although commenters also begin to engage more with Battle Royale during the same period, the shift is weaker and stabilizes over time. This suggests a more moderate migration compared to FPS, but one that persists in the long run, as users do not fully return to Sandbox after engaging with Battle Royale. We now examine whether these trends remain consistent when focusing on a more active group of authors.
</p>

<div class="slider">
  <div id="plot18" class="slide"><iframe src="/assets/plots/plots_3/plot-3-4-3.html"></iframe></div>
  <div id="plot19" class="slide"><iframe src="/assets/plots/plots_3/plot-3-4-4.html"></iframe></div>
</div>

<div class="slider-dots">
  <a href="#plot18" class="slider-dot"></a>
  <a href="#plot19" class="slider-dot"></a>
</div>

<p>
For the second group of authors, the overall temporal pattern remains similar, with a clear rise in Battle Royale engagement during the emergence of the genre and a peak during its core expansion phase. However, the shift toward Battle Royale is noticeably stronger than for less active users. This supports the idea that authors with higher activity levels are more likely to experience and reflect major genre transitions over time, particularly the rise of Battle Royale.
</p>

<p>
A comparable pattern is observed for Sandbox pioneers, where the redirection of comments toward Battle Royale is more pronounced than in the previous group but stabilizes once the genre becomes established. To further test whether user activity consistently amplifies this effect, we now examine the most active group of authors.
</p>

<div class="slider">
  <div id="plot20" class="slide"><iframe src="/assets/plots/plots_3/plot-3-4-5.html"></iframe></div>
  <div id="plot21" class="slide"><iframe src="/assets/plots/plots_3/plot-3-4-6.html"></iframe></div>
</div>

<div class="slider-dots">
  <a href="#plot20" class="slider-dot"></a>
  <a href="#plot21" class="slider-dot"></a>
</div>

<p>
The last group of authors confirms the hypothesis formulated earlier: the more active the users, the stronger the shift toward Battle Royale. Among these highly engaged commenters, Battle Royale captures a substantial share of attention, particularly from FPS pioneers. This supports the idea that long-term, active users are more likely to span multiple phases of the gaming ecosystem, encompassing both the rise of FPS and the later emergence of Battle Royale.
</p>

<p>
A similar dynamic is observed for Sandbox content. Although the redirection of attention toward Battle Royale is stronger than for less active users, it stabilizes once the genre becomes established. Overall, this temporal analysis shows that Battle Royale did not simply attract new users, but actively redirected engagement from pre-existing communities, with this effect being most pronounced among the most active commenters.
</p>

<!-- ================================================= -->
<!-- 3.3 -->
<h2 id="engagement-dynamics" style="color:#003c9e; font-size:2rem; font-weight:600;">
  (3.3) Did engagement dynamics differ for Battle Royale content?
</h2>

<p>
To quantify engagement intensity, we analyze the likes-per-view ratio (LPV),
which reflects how often viewers actively react to content rather than passively consuming it.
</p>

<!-- FIG 17 – Engagement comparison -->
<div class="plot-card">
  <iframe src="/assets/plots/plots_3/plot-3-5.html"></iframe>
</div>

<p>
Battle Royale consistently exhibits the highest LPV during 2017–2019.
Statistical tests confirm that this difference is significant
when compared to Sandbox, the second most engaging genre.
</p>


<h2 id="audience-steal" style="color:#003c9e; font-size:2rem; font-weight:600;">
  (3.4) Synthesis: Viewers dynamics
</h2>

<p>
Our analysis confirms that the Battle Royale (BR) explosion was not merely a surge in content production, but a deep transformation of viewer dynamics within the YouTube gaming ecosystem. This shift can be summarized along three main dimensions.
</p>

<p>
<strong>A gateway for new audiences</strong> Battle Royale emerged as a major entry point into YouTube gaming, attracting a substantial share of new active commenters. This effect is particularly visible among less active and newer users, suggesting that BR successfully brought fresh audiences into the ecosystem rather than simply recycling existing ones. While some migration from Sandbox and FPS communities is observed, this pattern largely reflects the natural evolution of long-term users toward emerging genres.
</p>

<p>
<strong>Strong retention and hook effect</strong> Battle Royale displays the highest retention among all genres. Users who first engaged with BR content were more likely to remain loyal to the genre over time, while established genres (especially FPS) experienced a noticeable loss of active commenters toward BR. This highlights BR’s exceptional ability to capture and sustain audience attention.
</p>

<p>
<strong>Higher engagement intensity</strong> Beyond audience size, Battle Royale content generated stronger engagement, with viewers reacting more actively than in other genres. This suggests that BR did not only attract viewers, but fostered higher enthusiasm and involvement within its community.
</p>

<p>
<strong>Final verdict</strong> The Battle Royale era marked a turning point for YouTube gaming. It expanded the ecosystem by attracting new users, redirected engagement from established communities, and built a highly loyal and engaged audience, reshaping viewer behavior at a platform-wide scale.
</p>
