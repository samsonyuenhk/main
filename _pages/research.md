---
layout: archive
title: "Research"
permalink: /research/
author_profile: true
---

<style>
/* ---------- Research page styling ----------
   NOTE: no font-family is declared anywhere in this file.
   All type inherits from the site theme.                 */

.page__content h2 {
  margin-top: 2.2em;
  padding-bottom: 0.3em;
  border-bottom: 2px solid #e8e8e8;
}
.page__content h3 {
  margin-top: 1.8em;
  margin-bottom: 0.6em;
}

/* Section jump links */
.section-nav {
  margin: 1.2em 0 2em;
  padding: 0.9em 1.1em;
  background: #fafafa;
  border: 1px solid #ececec;
  border-radius: 6px;
  line-height: 2;
}
.section-nav a {
  display: inline-block;
  margin-right: 1.2em;
  text-decoration: none;
  border-bottom: 1px dotted #bbb;
}
.section-nav a:hover { border-bottom-style: solid; }

/* Research-field directory under Journal Articles */
.field-nav {
  margin: 0.9em 0 1.8em;
  padding: 0;
  list-style: none;
  display: flex;
  flex-wrap: wrap;
  gap: 0.5em;
}
.field-nav li { margin: 0; }
.field-nav a {
  display: inline-block;
  padding: 5px 13px;
  border: 1px solid #dcdcdc;
  border-radius: 999px;
  background: #fafafa;
  color: #3d3d3d !important;
  text-decoration: none !important;
  line-height: 1.4;
}
.field-nav a:hover { background: #eef3f8; border-color: #a9c2d8; }
.field-nav .count { color: #999; font-size: 0.9em; margin-left: 4px; }

/* Highlight the field you just jumped to */
.page__content h3:target {
  background: #fffbe8;
  box-shadow: -8px 0 0 #fffbe8, 8px 0 0 #fffbe8;
}

/* Publication list */
.pub-list { list-style: none; padding-left: 0; margin-left: 0; }
.pub-list > li {
  margin: 0 0 1.35em 0;
  padding: 0 0 0 1.1em;
  border-left: 3px solid #ececec;
  line-height: 1.55;
}
.pub-list > li:hover { border-left-color: #c8c8c8; }
.pub-list .title { font-weight: bold; }
.pub-list .venue { font-style: italic; }
.me { font-weight: bold; }

/* DOI / link chips */
.doi {
  display: inline-block;
  font-size: 0.9em;
  padding: 1px 7px;
  margin-left: 2px;
  border: 1px solid #ddd;
  border-radius: 3px;
  color: #555 !important;
  text-decoration: none !important;
  white-space: nowrap;
}
.doi:hover { background: #f2f2f2; border-color: #bbb; }

/* Supplementary resource line */
.pub-links { margin: 0.4em 0 0; font-size: 0.9em; color: #777; }
.pub-links a { text-decoration: none; border-bottom: 1px dotted #aaa; }

/* Award note */
.award {
  display: block;
  margin: 0.35em 0 0;
  font-size: 0.9em;
  color: #8a6d1f;
  background: #fdf8e8;
  border-left: 3px solid #e0c65a;
  padding: 0.25em 0.6em;
}

/* ---------- Collapsible abstracts ---------- */
details.abstract { margin: 0.5em 0 0; }
details.abstract > summary {
  display: inline-block;
  cursor: pointer;
  list-style: none;
  color: #6b7f9e;
  padding: 2px 0;
  user-select: none;
}
details.abstract > summary::-webkit-details-marker { display: none; }
details.abstract > summary::before {
  content: "▸";
  display: inline-block;
  margin-right: 6px;
  transition: transform 0.15s ease;
}
details.abstract[open] > summary::before { transform: rotate(90deg); }
details.abstract > summary:hover { color: #2b4c7e; }
details.abstract .abstract-body {
  margin: 0.5em 0 0;
  padding: 0.85em 1.1em;
  background: #fafbfc;
  border: 1px solid #ececec;
  border-radius: 5px;
  line-height: 1.65;
}

/* Expand/collapse all control */
.abstract-toggle {
  float: right;
  font: inherit;
  cursor: pointer;
  color: #6b7f9e;
  border: 1px solid #ddd;
  border-radius: 4px;
  padding: 3px 10px;
  background: #fff;
}
.abstract-toggle:hover { background: #f3f6fa; }

/* ---------- Featured book ---------- */
.book {
  display: flex;
  gap: 1.6em;
  align-items: flex-start;
  margin: 1.2em 0 2em;
  padding: 1.4em;
  background: #fafafa;
  border: 1px solid #ececec;
  border-radius: 8px;
}
.book img {
  width: 165px;
  flex: 0 0 165px;
  border-radius: 3px;
  box-shadow: 0 3px 12px rgba(0,0,0,0.18);
}
.book .book-body { flex: 1; }
.book .book-title { font-weight: bold; line-height: 1.35; margin: 0 0 0.25em; }
.book .book-meta { color: #666; margin: 0 0 0.9em; }
.book .book-blurb { line-height: 1.65; margin: 0 0 1em; }
.book .order a {
  display: inline-block;
  margin-right: 0.5em;
  padding: 5px 14px;
  border: 1px solid #ccc;
  border-radius: 4px;
  text-decoration: none;
  color: #333 !important;
}
.book .order a:hover { background: #f0f0f0; border-color: #999; }

@media (max-width: 600px) {
  .book { flex-direction: column; align-items: center; }
  .book img { width: 140px; flex: 0 0 auto; }
  .abstract-toggle { float: none; display: inline-block; margin-bottom: 1em; }
}
</style>

{% if author.googlescholar %}
You can also find my articles on <u><a href="{{author.googlescholar}}">my Google Scholar profile</a></u>.
{% endif %}

<button class="abstract-toggle" onclick="toggleAbstracts(this)">Expand all abstracts</button>

<div class="section-nav" markdown="0">
  <a href="#books">Books</a>
  <a href="#peer-reviewed-journal-articles">Journal Articles</a>
  <a href="#edited-volume">Edited Volume</a>
  <a href="#book-chapters">Book Chapters</a>
  <a href="#public-scholarship">Public Scholarship</a>
</div>

## Books

<div class="book" markdown="0">
  <img src="https://assets.cambridge.org/97810094/45856/cover/9781009445856.jpg" alt="The Making of Leaderful Mobilization book cover">
  <div class="book-body">
    <p class="book-title">The Making of Leaderful Mobilizations: Power and Contention in Hong Kong</p>
    <p class="book-meta">With Edmund W. Cheng · Cambridge Studies in Contentious Politics · Cambridge University Press, 2025</p>
    <p class="book-blurb">The past few decades saw the transformation of Hong Kong from a liberal enclave to a revolutionary crucible. <em>The Making of Leaderful Mobilization</em> takes you through the evolution of protests in this restive city, where ordinary citizens gradually emerged as the protagonists of contention in place of social movement organizations. The book presents a theory of mediated threat that illuminates how threat perceptions fueled shifting forms of mobilization – from brokered mobilization where organizations played guiding roles to leaderful mobilization driven by peer collaboration among the masses. Bringing together event analysis, opinion polls, interviews, and social media data, this book provides a thorough and methodical anatomy of Hong Kong’s contentious politics. It unveils the processes and mechanisms of collective action that likely prevailed in many contemporary social movements worldwide. Our temporal approach also uncovers the multiple pathways reshaping hybrid regimes, underscoring their resilience and fragility.</p>
    <p class="order"><a href="#">Cambridge University Press</a><a href="#">Amazon</a></p>
    <span class="award">Co-winner, American Sociological Association, Political Sociology Section — 2026 Distinguished Contribution to Scholarship (Book) Award</span>
    <span class="award">Co-winner, American Political Science Association, Democracy and Autocracy Section — 2026 Best Book Award</span>
  </div>
</div>

## Peer-Reviewed Journal Articles

<ul class="field-nav" markdown="0">
  <li><a href="#contentious-politics">Contentious Politics</a></li>
  <li><a href="#migration">Migration</a></li>
  <li><a href="#greater-china">Greater China</a></li>
  <li><a href="#public-health">Public Health</a></li>
</ul>

### Contentious Politics
{: #contentious-politics}

<ul class="pub-list">

<li markdown="1">
<span class="me">Samson Yuen</span>. 2026. <span class="title">Braking Bad: How Internal Brakes Restrain Violent Tactics in Leaderless Protests.</span> <span class="venue">Journal of Peace Research</span>. <a class="doi" href="https://doi.org/10.1093/jopres/xjaf013">doi:10.1093/jopres/xjaf013</a>
<details class="abstract"><summary>Abstract</summary><div class="abstract-body">How do protesters restrain their use of violent tactics in leaderless and decentralized mass protests? While existing research highlights the role of leaders and movement organizations in enforcing nonviolent discipline, we lack understanding of how protester violence is regulated from within protest movements in the absence of centralized leadership. This article addresses this puzzle through a case study of Hong Kong's Anti-Extradition Movement of 2019. Through content and descriptive statistical analysis of LIHKG, an influential online discussion forum widely used by protesters during the movement, I examine the discursive strategies protesters employed to restrain violent escalation through the construction of “internal brakes”—discursive reasonings that aim to establish normative boundaries around the tactical use of violence. In addition to describing the basic characteristics of these internal brakes, I identify four subtypes based on their normative logic: proportionality, conditionality, consequentiality, and moral sanity. By analyzing how these brakes emerged and operated in relation to various forms of protester violence during the movement, I demonstrate that their salience varied depending on contextual factors including the target scope, predictability, and severity of the violence they aimed to restrain. The findings contribute to the contentious politics literature by developing a novel theoretical framework for understanding self-regulation mechanisms in leaderless and decentralized movements that experience tactical radicalization.</div></details>
</li>

<li markdown="1">
Francis L. F. Lee, <span class="me">Samson Yuen</span> &amp; Gary Tang. 2025. <span class="title">Protest Memories and Individual Persistence: Examining Participants’ Intention to Remember a Movement under Democratic Backsliding.</span> <span class="venue">Social Movement Studies</span>. <a class="doi" href="https://doi.org/10.1080/14742837.2025.2481050">doi:10.1080/14742837.2025.2481050</a>
<details class="abstract"><summary>Abstract</summary><div class="abstract-body">Researchers have paid increasing attention to the movement-memory nexus and recognized the role memories play in sustaining movement continuity. This article focuses on the role of individuals’ intention to remember in the movement abeyance process. Defined as a subjective emphasis on the need to remember a protest movement for the purpose of preserving the movement’s legacy and significance into the future, intention to remember is posited as part of a cluster of mutually reinforcing beliefs, attitudes, and behavior that sustain individual movement engagement in times of abeyance. Empirical analysis of a survey of participants in Hong Kong’s Anti-ELAB Movement, conducted three years after the protests ended, supports the arguments by showing that intention to remember positively relates to persistent actions, movement evaluation, collective efficacy, and collective identification. Nonetheless, intention to remember is related only to recall of protest events involving violence against protesters, but not to recall of peaceful protest events.</div></details>
</li>

<li markdown="1">
<span class="me">Samson Yuen</span> &amp; John Chit Wai Mok. 2023. <span class="title">Groundwork for Democracy? Community Activism and Movement Abeyance in Post-handover Hong Kong.</span> <span class="venue">The China Journal</span> 90(1): 78–105. <a class="doi" href="https://doi.org/10.1086/725129">doi:10.1086/725129</a>
<details class="abstract"><summary>Abstract</summary><div class="abstract-body">Studies on Hong Kong’s contentious politics have focused primarily on the high tides of mobilization. Scant attention is paid to what became of the intense mobilizations following their decline. This article spotlights the “abeyance” politics of community activism, in which activists sought to make territorial communities an arena of social and political participation in quieter times after mass mobilizations. Drawing on the concept of abeyance from political sociology, we argue that community activism served as “abeyance structures” after the mass mobilizations in the early 2010s, a major protest cycle preceding the 2019 anti-extradition movement. Based on mixed methods and original data, we argue that these abeyance structures not only allowed activists to maintain their political engagement but also gave rise to various practices of “lived citizenship” in territorial communities. These practices produced a changing sense of political subjectivity among citizens, establishing a more grounded notion of democracy that emphasizes their participation in local affairs and social entitlements. Our findings aim to enrich the literature on movement abeyance and provide a nuanced understanding of political activism in Hong Kong beyond street politics.</div></details>
</li>

<li markdown="1">
<span class="me">Samson Yuen</span>. 2023. <span class="title">Tolerant Solidarity with Violent Protesters: Evidence from a Survey Experiment.</span> <span class="venue">Journal of Conflict Resolution</span> 67(9): 1731–1756. <a class="doi" href="https://doi.org/10.1177/00220027231154451">doi:10.1177/00220027231154451</a>
<details class="abstract"><summary>Abstract</summary><div class="abstract-body">Add abstract here.</div></details>
<p class="pub-links"><a href="#">Appendix</a> · <a href="#">Replication data</a> · <a href="#">R code</a></p>
</li>

<li markdown="1">
Edmund W. Cheng, <span class="me">Samson Yuen</span>, Francis L. F. Lee &amp; Gary Tang. 2022. <span class="title">Total Mobilisation from Below: Abeyance Networks, Threats and Emotions in Hong Kong’s Freedom Summer.</span> <span class="venue">The China Quarterly</span> 251: 629–659. <a class="doi" href="https://doi.org/10.1017/S0305741022000236">doi:10.1017/S0305741022000236</a>
<details class="abstract"><summary>Abstract</summary><div class="abstract-body">Add abstract here.</div></details>
</li>

<li markdown="1">
<span class="me">Samson Yuen</span>, Gary Tang, Francis L. F. Lee &amp; Edmund W. Cheng. 2022. <span class="title">Surveying Spontaneous Mass Protests: Mixed-mode Sampling in Hong Kong’s Anti-Extradition Bill Movement.</span> <span class="venue">Sociological Methodology</span> 52(1): 75–102. <a class="doi" href="https://doi.org/10.1177/00811750211071130">doi:10.1177/00811750211071130</a>
<details class="abstract"><summary>Abstract</summary><div class="abstract-body">Add abstract here.</div></details>
</li>

<li markdown="1">
<span class="me">Samson Yuen</span>. 2021. <span class="title">Institutional Foundation of Countermobilization: Elites and Pro-Regime Grassroots Organizations in Post-handover Hong Kong.</span> <span class="venue">Government and Opposition</span> 1–22. <a class="doi" href="https://doi.org/10.1017/gov.2021.39">doi:10.1017/gov.2021.39</a>
<details class="abstract"><summary>Abstract</summary><div class="abstract-body">Countermobilization has been a common strategy for autocrats to counteract the threat of opposition. Although the use of countermobilization has drawn scholarly attention, research on the mechanisms that enable countermobilization remains limited. This article underscores the role of political institutions in allowing autocrats to carry out countermobilization through incentivizing elites to serve as a bridge between the state and the masses. Focusing on the case of Hong Kong, where pro-government countermobilization is rising along with pro-democracy challenges against the hybrid regime, the article argues that countermobilization is enabled because societal elites are incentivized through political institutions to organize the masses and develop mobilization capacity through grassroots organizations. Using original elite biographical data and organizational data, the article shows that elites with more ties with grassroots organizations are more likely to remain in office in the Chinese People's Political Consultative Conference. The findings offer an institutionalist explanation of how authoritarian rulers enact countermobilization by leveraging elite intermediaries and their grassroots networks.</div></details>
</li>

<li markdown="1">
<span class="me">Samson Yuen</span> &amp; Gary Tang. 2021. <span class="title">Instagram Networks and Social Capital: Teenage Activism in Hong Kong’s Anti-Extradition Bill Movement.</span> <span class="venue">Social Movement Studies</span>. <a class="doi" href="https://doi.org/10.1080/14742837.2021.2011189">doi:10.1080/14742837.2021.2011189</a>
<details class="abstract"><summary>Abstract</summary><div class="abstract-body">Add abstract here.</div></details>
<span class="award">Honourable mention, 2022 Britta Baumgarten Memorial Prize</span>
</li>

<li markdown="1">
<span class="me">Samson Yuen</span> &amp; Kin-long Tong. 2021. <span class="title">Solidarity in Diversity: Online Petitions and Collective Identity in Hong Kong’s Anti-Extradition Bill Movement.</span> <span class="venue">Japanese Journal of Political Science</span> 22(4): 215–232. <a class="doi" href="https://doi.org/10.1017/S146810992100030X">doi:10.1017/S146810992100030X</a>
<details class="abstract"><summary>Abstract</summary><div class="abstract-body">Add abstract here.</div></details>
</li>

<li markdown="1">
Kin-long Tong &amp; <span class="me">Samson Yuen</span>. 2021. <span class="title">Disciplining Student Activism: Secondary Schools as Sites of Political Struggle during Mass Protests.</span> <span class="venue">Sociological Forum</span> 36(4): 984–1004. <a class="doi" href="https://doi.org/10.1111/socf.12744">doi:10.1111/socf.12744</a>
<details class="abstract"><summary>Abstract</summary><div class="abstract-body">Add abstract here.</div></details>
</li>

<li markdown="1">
Francis L. F. Lee, Hai Liang, Edmund W. Cheng, Gary Tang &amp; <span class="me">Samson Yuen</span>. 2021. <span class="title">Affordances, Movement Dynamics, and LIHKG as a Centralized Communication Platform in the 2019 Hong Kong Protests.</span> <span class="venue">Information, Communication and Society</span> 25(12): 1699–1716. <a class="doi" href="https://doi.org/10.1080/1369118X.2021.1877772">doi:10.1080/1369118X.2021.1877772</a>
<details class="abstract"><summary>Abstract</summary><div class="abstract-body">Add abstract here.</div></details>
</li>

<li markdown="1">
Francis L. F. Lee, Edmund W. Cheng, Hai Liang, Gary Tang &amp; <span class="me">Samson Yuen</span>. 2021. <span class="title">Dynamics of Tactical Radicalization and Public Receptiveness in Hong Kong’s Anti-Extradition Bill Movement.</span> <span class="venue">Journal of Contemporary Asia</span> 52(3): 429–451. <a class="doi" href="https://doi.org/10.1080/00472336.2021.1910330">doi:10.1080/00472336.2021.1910330</a>
<details class="abstract"><summary>Abstract</summary><div class="abstract-body">Add abstract here.</div></details>
</li>

<li markdown="1">
Gary Tang, Eva P. W. Hung, Christopher H. K. Au-Yeung &amp; <span class="me">Samson Yuen</span>. 2020. <span class="title">Politically Motivated Internet Addiction: Relationship among Online Information Exposure, Internet Addiction, FOMO, Psychological Well-being, and Radicalism in a Massive Political Turbulence.</span> <span class="venue">International Journal of Environmental Research and Public Health</span> 17(2): 633. <a class="doi" href="https://doi.org/10.3390/ijerph17020633">doi:10.3390/ijerph17020633</a>
<details class="abstract"><summary>Abstract</summary><div class="abstract-body">Add abstract here.</div></details>
</li>

<li markdown="1">
Francis L. F. Lee, <span class="me">Samson Yuen</span>, Gary Tang &amp; Edmund W. Cheng. 2020. <span class="title">Hong Kong’s Summer of Uprising: From Anti-Extradition to Anti-Authoritarian Protests.</span> <span class="venue">China Review</span> 19(4): 1–32. <a class="doi" href="https://www.jstor.org/stable/26838911">JSTOR</a>
<details class="abstract"><summary>Abstract</summary><div class="abstract-body">Add abstract here.</div></details>
</li>

<li markdown="1">
Edmund W. Cheng &amp; <span class="me">Samson Yuen</span>. 2019. <span class="title">Memory in Movement: Collective Identity and Memory Contestation in Hong Kong’s Tiananmen Vigils.</span> <span class="venue">Mobilization: An International Quarterly</span> 24(4): 419–437. <a class="doi" href="https://doi.org/10.17813/1086-671X-24-4-419">doi:10.17813/1086-671X-24-4-419</a>
<details class="abstract"><summary>Abstract</summary><div class="abstract-body">Add abstract here.</div></details>
</li>

<li markdown="1">
<span class="me">Samson Yuen</span>. 2018. <span class="title">Contesting Middle-class Civility: Place-based Collective Identity in Hong Kong’s Occupy Mongkok.</span> <span class="venue">Social Movement Studies</span> 17(4): 393–407. <a class="doi" href="https://doi.org/10.1080/14742837.2018.1434501">doi:10.1080/14742837.2018.1434501</a>
<details class="abstract"><summary>Abstract</summary><div class="abstract-body">Add abstract here.</div></details>
</li>

<li markdown="1">
<span class="me">Samson Yuen</span> &amp; Edmund W. Cheng. 2017. <span class="title">Neither Repression nor Concession? A Regime’s Attrition against Mass Protests.</span> <span class="venue">Political Studies</span> 65(3): 611–630. <a class="doi" href="https://doi.org/10.1177/0032321716674024">doi:10.1177/0032321716674024</a>
<details class="abstract"><summary>Abstract</summary><div class="abstract-body">Add abstract here.</div></details>
</li>

</ul>

### Migration
{: #migration}

<ul class="pub-list">

<li markdown="1">
<span class="me">Samson Yuen</span> &amp; Gary Tang. 2026. <span class="title">Loyal to What and Whom? Relational Loyalty and Migration Decision-Making in Hong Kong.</span> <span class="venue">International Migration Review</span>. <a class="doi" href="https://doi.org/10.1177/01979183251409759">doi:10.1177/01979183251409759</a>
<details class="abstract"><summary>Abstract</summary><div class="abstract-body">Add abstract here.</div></details>
</li>

<li markdown="1">
Shuet-Ying Kitty Ho, <span class="me">Samson Yuen</span> &amp; Gary Tang. 2025. <span class="title">Citizens in Transit: Diasporic Citizenship of Hongkongers Living as British National Overseas Migrants in the United Kingdom.</span> <span class="venue">Asian Ethnicity</span>. <a class="doi" href="https://doi.org/10.1080/14631369.2025.2551704">doi:10.1080/14631369.2025.2551704</a>
<details class="abstract"><summary>Abstract</summary><div class="abstract-body">Add abstract here.</div></details>
</li>

</ul>

### State–Society Relations in Greater China
{: #greater-china}

<ul class="pub-list">

<li markdown="1">
Francis L. F. Lee, <span class="me">Samson Yuen</span> &amp; Gary K. Y. Tang. 2025. <span class="title">Adaptation and Resilience: How Pro-Democracy Protesters Respond to Autocratisation in Hong Kong.</span> <span class="venue">Journal of Contemporary Asia</span> 55(5): 801–821. <a class="doi" href="https://doi.org/10.1080/00472336.2024.2424173">doi:10.1080/00472336.2024.2424173</a>
<details class="abstract"><summary>Abstract</summary><div class="abstract-body">Add abstract here.</div></details>
</li>

<li markdown="1">
<span class="me">Samson Yuen</span> &amp; Karita Kan. 2021. <span class="title">Of Mad Cows and Dead Pigs: Negotiating Food Safety and Sovereignty in Taiwan.</span> <span class="venue">Geopolitics</span> 27(5): 1552–1573. <a class="doi" href="https://doi.org/10.1080/14650045.2020.1863791">doi:10.1080/14650045.2020.1863791</a>
<details class="abstract"><summary>Abstract</summary><div class="abstract-body">Add abstract here.</div></details>
</li>

<li markdown="1">
<span class="me">Samson Yuen</span>. 2021. <span class="title">Native-Place Networks and Political Mobilization: The Case of Post-handover Hong Kong.</span> <span class="venue">Modern China</span> 47(5): 510–539. <a class="doi" href="https://doi.org/10.1177/0097700420934093">doi:10.1177/0097700420934093</a>
<details class="abstract"><summary>Abstract</summary><div class="abstract-body">Add abstract here.</div></details>
<span class="award">ICAS 2021 Best Article Prize on Global Hong Kong Studies</span>
<span class="award">Academy of Hong Kong Studies 2021 Outstanding Paper Award</span>
</li>

<li markdown="1">
<span class="me">Samson Yuen</span> &amp; Edmund W. Cheng. 2020. <span class="title">Deepening the State: The Dynamics of China’s United Front Work in Post-Handover Hong Kong.</span> <span class="venue">Communist and Post-Communist Studies</span> 53(4): 136–154. <a class="doi" href="https://www.jstor.org/stable/48610604">JSTOR</a>
<details class="abstract"><summary>Abstract</summary><div class="abstract-body">Add abstract here.</div></details>
</li>

<li markdown="1">
Francis L. F. Lee, <span class="me">Samson Yuen</span>, Gary Tang &amp; Edmund W. Cheng. 2020. <span class="title">Five Demands and (Not Quite) Beyond.</span> <span class="venue">Communist and Post-Communist Studies</span> 53(4): 22–40. <a class="doi" href="https://www.jstor.org/stable/48610599">JSTOR</a>
<details class="abstract"><summary>Abstract</summary><div class="abstract-body">Add abstract here.</div></details>
</li>

<li markdown="1">
<span class="me">Samson Yuen</span>. 2020. <span class="title">Delivering Services in China’s Fragmented Local State: The Procurement of Social Work NGOs in Guangzhou.</span> <span class="venue">China Review</span> 20(4): 159–188. <a class="doi" href="https://www.jstor.org/stable/26959857">JSTOR</a>
<details class="abstract"><summary>Abstract</summary><div class="abstract-body">Add abstract here.</div></details>
</li>

<li markdown="1">
<span class="me">Samson Yuen</span> &amp; Edmund W. Cheng. 2020. <span class="title">Between High Autonomy and Sovereign Control in a Subnational Island Jurisdiction: The Paradox of Hong Kong under ‘One Country, Two Systems’.</span> <span class="venue">Island Studies Journal</span> 15(1): 131–150. <a class="doi" href="https://doi.org/10.24043/isj.110">doi:10.24043/isj.110</a>
<details class="abstract"><summary>Abstract</summary><div class="abstract-body">Add abstract here.</div></details>
</li>

<li markdown="1">
<span class="me">Samson Yuen</span> &amp; Sanho Chung. 2019. <span class="title">Explaining Localism in Post-handover Hong Kong: An Eventful Approach.</span> <span class="venue">China Perspectives</span> 3: 19–29. <a class="doi" href="https://doi.org/10.4000/chinaperspectives.8044">doi:10.4000/chinaperspectives.8044</a>
<details class="abstract"><summary>Abstract</summary><div class="abstract-body">Add abstract here.</div></details>
</li>

<li markdown="1">
<span class="me">Samson Yuen</span> &amp; Edmund W. Cheng. 2018. <span class="title">Rethinking Contentious Politics in Hong Kong: Change and Continuity.</span> <span class="venue">Hong Kong Studies</span> 1(1): 7–25. <a class="doi" href="https://cup.cuhk.edu.hk/chinesepress/journal/HKS1.1/HKS1.1_7-25.pdf">PDF</a>
<details class="abstract"><summary>Abstract</summary><div class="abstract-body">Add abstract here.</div></details>
</li>

<li markdown="1">
<span class="me">Samson Yuen</span>. 2018. <span class="title">Negotiating Service Activism in China: The Impact of NGOs’ Institutional Embeddedness in the Local State.</span> <span class="venue">Journal of Contemporary China</span> 27(111): 406–427. <a class="doi" href="https://doi.org/10.1080/10670564.2018.1410976">doi:10.1080/10670564.2018.1410976</a>
<details class="abstract"><summary>Abstract</summary><div class="abstract-body">Add abstract here.</div></details>
</li>

<li markdown="1">
Karita Kan &amp; <span class="me">Samson Yuen</span>. 2018. <span class="title">Visceral Politics: Food and Risk in China–Taiwan Relations.</span> <span class="venue">China Information</span> 32(3): 443–462. <a class="doi" href="https://doi.org/10.1177/0920203X18769217">doi:10.1177/0920203X18769217</a>
<details class="abstract"><summary>Abstract</summary><div class="abstract-body">Add abstract here.</div></details>
</li>

<li markdown="1">
<span class="me">Samson Yuen</span>. 2015. <span class="title">Friend or Foe? The Diminishing Space of China’s Civil Society.</span> <span class="venue">China Perspectives</span> 3: 51–56. <a class="doi" href="https://doi.org/10.4000/chinaperspectives.6807">doi:10.4000/chinaperspectives.6807</a>
<details class="abstract"><summary>Abstract</summary><div class="abstract-body">Add abstract here.</div></details>
</li>

<li markdown="1">
<span class="me">Samson Yuen</span>. 2015. <span class="title">Becoming a Cyber Power: China’s Cybersecurity Upgrades and its Consequences.</span> <span class="venue">China Perspectives</span> 2: 53–58. <a class="doi" href="https://doi.org/10.4000/chinaperspectives.6731">doi:10.4000/chinaperspectives.6731</a>
<details class="abstract"><summary>Abstract</summary><div class="abstract-body">Add abstract here.</div></details>
</li>

<li markdown="1">
<span class="me">Samson Yuen</span>. 2015. <span class="title">Hong Kong After the Umbrella Movement: An Uncertain Future for the ‘One Country Two Systems’.</span> <span class="venue">China Perspectives</span> 1: 49–53. <a class="doi" href="https://doi.org/10.4000/chinaperspectives.6656">doi:10.4000/chinaperspectives.6656</a>
<details class="abstract"><summary>Abstract</summary><div class="abstract-body">Add abstract here.</div></details>
</li>

<li markdown="1">
<span class="me">Samson Yuen</span>. 2014. <span class="title">Taming the ‘Foreign Tigers’: China’s Anti-Trust Crusade against Multinational Companies.</span> <span class="venue">China Perspectives</span> 4: 53–59. <a class="doi" href="https://doi.org/10.4000/chinaperspectives.6587">doi:10.4000/chinaperspectives.6587</a>
<details class="abstract"><summary>Abstract</summary><div class="abstract-body">Add abstract here.</div></details>
</li>

<li markdown="1">
<span class="me">Samson Yuen</span>. 2014. <span class="title">Disciplining the Party: Xi Jinping’s Anti-Corruption Campaign and its Limits.</span> <span class="venue">China Perspectives</span> 3: 41–47. <a class="doi" href="https://doi.org/10.4000/chinaperspectives.6542">doi:10.4000/chinaperspectives.6542</a>
<details class="abstract"><summary>Abstract</summary><div class="abstract-body">Add abstract here.</div></details>
</li>

<li markdown="1">
<span class="me">Samson Yuen</span>. 2014. <span class="title">Under the Shadow of China: Beijing’s Policy towards Hong Kong and Taiwan in Comparative Perspective.</span> <span class="venue">China Perspectives</span> 2: 69–76. <a class="doi" href="https://doi.org/10.4000/chinaperspectives.6491">doi:10.4000/chinaperspectives.6491</a>
<details class="abstract"><summary>Abstract</summary><div class="abstract-body">Add abstract here.</div></details>
</li>

<li markdown="1">
<span class="me">Samson Yuen</span>. 2014. <span class="title">China’s New Rural Land Reform? Assessment and Prospects.</span> <span class="venue">China Perspectives</span> 1: 61–65. <a class="doi" href="https://doi.org/10.4000/chinaperspectives.6403">doi:10.4000/chinaperspectives.6403</a>
<details class="abstract"><summary>Abstract</summary><div class="abstract-body">Add abstract here.</div></details>
</li>

<li markdown="1">
<span class="me">Samson Yuen</span>. 2013. <span class="title">Debating Constitutionalism in China: Dreaming of a Liberal Turn.</span> <span class="venue">China Perspectives</span> 4: 67–72. <a class="doi" href="https://doi.org/10.4000/chinaperspectives.6325">doi:10.4000/chinaperspectives.6325</a>
<details class="abstract"><summary>Abstract</summary><div class="abstract-body">Add abstract here.</div></details>
</li>

</ul>

### Public Health
{: #public-health}

<ul class="pub-list">

<li markdown="1">
Bobo H. P. Lau, <span class="me">Samson Yuen</span>, Ricci P. H. Yue &amp; Karen A. Grépin. 2022. <span class="title">Understanding the Societal Factors of Vaccine Acceptance and Hesitancy: Evidence from Hong Kong.</span> <span class="venue">Public Health</span> 207: 39–45. <a class="doi" href="https://doi.org/10.1016/j.puhe.2022.03.013">doi:10.1016/j.puhe.2022.03.013</a>
<details class="abstract"><summary>Abstract</summary><div class="abstract-body">Add abstract here.</div></details>
</li>

<li markdown="1">
Siu Yau Lee, <span class="me">Samson Yuen</span>, Nick Or, Edmund W. Cheng &amp; Ricci P. H. Yue. 2022. <span class="title">COVID-19 Vulnerability, Policy Feedback, and Support for Immigration: Evidence from Asia.</span> <span class="venue">British Journal of Social Psychology</span> 61(4): 1124–1143. <a class="doi" href="https://doi.org/10.1111/bjso.12529">doi:10.1111/bjso.12529</a>
<details class="abstract"><summary>Abstract</summary><div class="abstract-body">Add abstract here.</div></details>
</li>

<li markdown="1">
Nick Or, Edmund W. Cheng, Ricci P. H. Yue &amp; <span class="me">Samson Yuen</span>. 2021. <span class="title">Risk Perceptions, Anxiety and the Future of International Trade: A Cross-national Study of Public Trade Preferences in Asia under COVID-19.</span> <span class="venue">Journal of Elections, Public Opinion and Parties</span> 31(1): 26–40. <a class="doi" href="https://doi.org/10.1080/17457289.2021.1924732">doi:10.1080/17457289.2021.1924732</a>
<details class="abstract"><summary>Abstract</summary><div class="abstract-body">Add abstract here.</div></details>
</li>

<li markdown="1">
<span class="me">Samson Yuen</span>, Edmund W. Cheng, Nick Or, Karen A. Grépin, King-wa Fu, Ka Chun Yung &amp; Ricci P. H. Yue. 2021. <span class="title">A Tale of Two City-states: A Comparison of the State-led vs Civil Society-led Responses to COVID-19 in Singapore and Hong Kong.</span> <span class="venue">Global Public Health</span> 16(8–9): 1283–1303. <a class="doi" href="https://doi.org/10.1080/17441692.2021.1877769">doi:10.1080/17441692.2021.1877769</a>
<details class="abstract"><summary>Abstract</summary><div class="abstract-body">Add abstract here.</div></details>
</li>

</ul>

## Edited Volume

<ul class="pub-list">

<li markdown="1">
Edmund W. Cheng &amp; <span class="me">Samson Yuen</span>. 2018. <span class="title">The Epoch of Social Movement: Trajectory of Contentious Politics in Hong Kong 社運年代：香港抗爭政治的軌跡.</span> Hong Kong: Chinese University of Hong Kong Press. <em>[In Chinese]</em>
</li>

</ul>

## Book Chapters

<ul class="pub-list">

<li markdown="1">
Edmund W. Cheng &amp; <span class="me">Samson Yuen</span>. 2021. <span class="title">Anti-Extradition Movement.</span> In David A. Snow, Donatella della Porta &amp; Bert Klandermans (eds.), <span class="venue">The Wiley-Blackwell Encyclopedia of Social and Political Movements</span>. Malden: Wiley.
<details class="abstract"><summary>Abstract</summary><div class="abstract-body">Add abstract here.</div></details>
</li>

<li markdown="1">
Chi-shun Fong &amp; <span class="me">Samson Yuen</span>. 2021. <span class="title">Movement Leadership in an Era of Connective Action: A Study of Hong Kong’s Student-Led Umbrella Movement.</span> In Lorenzo Cini, Donatella della Porta &amp; César Guzmán-Concha (eds.), <span class="venue">Student Movements in Late Neoliberalism</span>. Palgrave Macmillan.
<details class="abstract"><summary>Abstract</summary><div class="abstract-body">Add abstract here.</div></details>
</li>

<li markdown="1">
<span class="me">Samson Yuen</span>. 2019. <span class="title">Transgressive Politics in Occupy Mongkok.</span> In Ching Kwan Lee &amp; Ming Sing (eds.), <span class="venue">Take Back Our Future: An Eventful Sociology of the Hong Kong Umbrella Movement</span>. Ithaca, NY: Cornell University Press.
<details class="abstract"><summary>Abstract</summary><div class="abstract-body">Add abstract here.</div></details>
</li>

<li markdown="1">
<span class="me">Samson Yuen</span>. 2019. <span class="title">From Repression to Attrition: State Responses towards the Umbrella Movement.</span> In Ngok Ma &amp; Edmund W. Cheng (eds.), <span class="venue">The Umbrella Movement: Civil Resistance and Contentious Space in Hong Kong</span>. Amsterdam: Amsterdam University Press.
<details class="abstract"><summary>Abstract</summary><div class="abstract-body">Add abstract here.</div></details>
</li>

</ul>

## Public Scholarship

<ul class="pub-list">

<li markdown="1">
<span class="me">Samson Yuen</span>. 2019. <span class="title">Hong Kong Protests: Why are People Demonstrating? How we Surveyed Protestors.</span> <span class="venue">Political Quarterly Blog</span>, October 16.
</li>

<li markdown="1">
<span class="me">Samson Yuen</span>. 2019. <span class="title">New Research Shows Vast Majority of Hong Kong Protesters Support More Radical Tactics.</span> <span class="venue">The Conversation</span>, September 2.
</li>

<li markdown="1">
<span class="me">Samson Yuen</span> &amp; Edmund W. Cheng. 2015. <span class="title">Hong Kong’s Umbrella Protests Were More Than Just a Student Movement.</span> <span class="venue">ChinaFile</span>, July 1.
</li>

<li markdown="1">
Edmund W. Cheng &amp; <span class="me">Samson Yuen</span>. 2015. <span class="title">The Umbrella Movement: Contentious Politics on China’s Periphery.</span> <span class="venue">Twenty-First Century Bimonthly</span> 147: 22–32. <em>[In Chinese]</em>
</li>

<li markdown="1">
<span class="me">Samson Yuen</span>. 2015. <span class="title">Youth Participation in Hong Kong’s Occupy Movement: How to Formulate Post-Occupy Youth Policy?</span> <span class="venue">Policy Bulletin, The Hong Kong Council of Social Service</span> 18. <em>[In Chinese]</em>
</li>

<li markdown="1">
Siu Yau Lee &amp; <span class="me">Samson Yuen</span>. 2015. <span class="title">How is Self-reliance Possible? An Analysis of Hawker Policy and the Privatization of the Link REIT.</span> <span class="venue">Journal of Local Discourse 2013–2014</span>. <em>[In Chinese]</em>
</li>

</ul>

<script>
function toggleAbstracts(btn) {
  var items = document.querySelectorAll('details.abstract');
  var open = btn.getAttribute('data-open') === 'true';
  items.forEach(function (d) { d.open = !open; });
  btn.setAttribute('data-open', (!open).toString());
  btn.textContent = open ? 'Expand all abstracts' : 'Collapse all abstracts';
}
</script>
