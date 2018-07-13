Functional diversity improves tropical forest recovery from disturbance shifting from complementarity to selection effect (to rework)
================
Sylvain Schmitt, Isabelle Maréchaux, Jerome Chave, Fabian Fischer, Camille Piponiot, Stéphane Traissac & Bruno Hérault
2018-05-31

Abstract
========

**To be written**

Introduction
============

Natural disturbances caused by tree death play a major role in tropical forest functioning through gap-phase regeneration (Veblen [1992](#ref-Veblen1992)). Climate change and direct human activities are currently deeply modifying forest disturbance regimes (Davidson *et al.* [2012](#ref-Davidson2012); Lewis *et al.* [2015](#ref-Lewis2015)). If deforestation has been rightly the focus of worldwide attention, forest degradation has been less studied and quantified through tropics (Simula [2009](#ref-Simula2009); Putz & Redford [2010](#ref-Putz2010)). However, degraded forests cover areas over ten times larger than deforestation (Herold *et al.* [2011](#ref-Herold2011)), a majority of which is being logged for timber production (Blaser *et al.* [2011](#ref-Blaser2011)). Forest degradation can trigger severe biodiversity loss (Burivalova *et al.* [2014](#ref-Burivalova2014)) and is estimated to account for 20.7 billion of tons of carbon dioxide emissions per year (Pearson *et al.* [2017](#ref-Pearson2017)), representing 20% of greenhouse gas emissions in the Brazilian Amazon (Asner *et al.* [2005](#ref-Asner2005)). Understanding the drivers of tropical forest resilience to disturbance is thus critical.

Resilience concept has met numerous definitions, but resilience in ecology can encompass both ecosystem ability to adsorb and recover from disturbance, resistance and recovery respectively (Gunderson [2010](#ref-Gunderson2010)). Both exogenous (e.g. climate, disturbance features) and endogenous (e.g. forest structure and composition) factors can drive ecosystem recovery after disturbance. Among the former, logging intensity has been reported to strongly control and increase time-to-recovery of post-logging tree carbon, subsequent animal biodiversity loss, and change in tree species composition (Burivalova *et al.* [2014](#ref-Burivalova2014); Avila *et al.* [2015](#ref-DeAvila2015); Rutishauser *et al.* [2015](#ref-Rutishauser2015)). Among endogenous drivers, forest pre-disturbance composition has been identified as a key driver of forest recovery (Hérault & Piponiot [2018](#ref-Herault2018)), as different species respond differently to perturbations depending on their ecological strategies and functional properties (Hérault *et al.* [2011](#ref-herault_functional_2011)). Beyond species identity, tree community diversity may also foster forest resilience to perturbations (Ives & Carpenter [2007](#ref-Ives2007); Cadotte *et al.* [2011](#ref-Cadotte2011); Loreau & Mazancourt [2013](#ref-Loreau2013)).

Two types of mechanisms can underlie an effect of biodiversity on ecosystem properties: complementarity and selection effects (Loreau & Hector [2001](#ref-Loreau2001)). Complementarity effect results from resources partitioning and niche differentiation, and facilitation, leading to a more efficient use of available resources. Selection effect results from a higher probability of more diverse community to include particularly efficient species regarding ecosystem process or stability. Moreover the sampling effect additionally implies redundancy and a lower risk to lose important functional traits, further improving resilience of species rich-forest (Tilman *et al.* [2001](#ref-Tilman2001); Hooper *et al.* [2005](#ref-Hooper2005a)).

The effect of biodiversity on ecosystem functioning has been intensely studied over the last decades, through theoretical work (Loreau [2010](#ref-Loreau2010)), experiments (Cardinale *et al.* [2009](#ref-Cardinale2009)), or observations along natural gradient of biodiversity (Paquette & Messier [2011](#ref-Paquette2011); Chisholm *et al.* [2013](#ref-Chisholm2013); Liang *et al.* [2016](#ref-Liang2016); Poorter *et al.* [2017](#ref-Poorter2017)). However, experiments have mostly been conducted on grasslands (Hector & Loreau [2005](#ref-Hector2005)), while studies relying on forest stand inventories often lack repeatability (Schnitzer & Carson [2016](#ref-Schnitzer2016)), rarely include logged forests (Sist *et al.* [2015](#ref-Sist2015)), and monitoring temporal coverage remains too low to assess long-term effect as trees are long-lived organisms (Hérault & Piponiot [2018](#ref-Herault2018)). Forest simulators have thus proven useful to investigate the effect of biodiversity on forest ecosystem functioning through virtual biodiversity experiments (Morin *et al.* [2011](#ref-Morin2011), [2014](#ref-Morin2014); Sakschewski *et al.* [2016](#ref-Sakschewski2016)), but the problem of biodiversity representation beyond a few plant functional types in models of tropical forests have long been an impediment to apply this approach to this species-rich ecosystem (Köhler & Huth [1998](#ref-Kohler1998); Purves & Pacala [2008](#ref-Purves2008); Kazmierczak *et al.* [2014](#ref-Kazmierczak2014)).

In the present study, we take advantage of recent developments made in the forest simulator TROLL (Chave [1999](#ref-Chave1999)), an individual-based and spatially-explicit model of tropical forest, that allow to deal with high diversity levels through a parameterization using plant functional traits (Maréchaux & Chave [2017](#ref-Marechaux2017)). Consequently, TROLL offers the opportunity to study biodiversity-ecosystem functioning *in silico* in tropical forest communities.

We used a simulation approach to assess the effect of species richness and functional composition on long-term forest recovery from disturbances of different levels. We manipulated species number and identity across a large number of simulations, and measured the biodiversity net effect on simulated forest recovery after disturbance. In order to further investigate the mechanisms underlying such potential effect of biodiversity, we partitioned it into complementarity and selection effects. Based on the general hypothesis of a positive relationships between biodiversity and productivity (Liang *et al.* [2016](#ref-Liang2016)), we hypothesized that more diverse forest will recover quicker to a disturbance due to an increased productivity.

Material and Methods
====================

TROLL Model
-----------

TROLL is an individual-based and spatially explicit forest dynamic model in which the life cycle of individual trees (recruitment, growth, seed production and death) &gt;1*c**m* diameter is simulated. Trees grows in a forest light environment explicitly computed within a 1*m*<sup>3</sup> resolution voxel grid. Seedlings below the 1*c**m* size class are not modeled explicitly, but are part of a seed/seedlings pool. A maximum of one tree can establish in each 1 \* 1*m* pixel. Each tree is defined by its age, diameter at breast height (dbh), height (h), crown radius (CR), crown depth (CD) and leaf area (LA). Tree geometry is calculated with allometric relationships. Additionally, each tree is flagged with a species label inherited from the parent tree through the seedling recruitment. To each species label is associated a number of species-specific traits (Table @ref(tab:traits)) from which processes are simulated using up-to-date established relationships drawn from the literature. The model thus represents tree biodiversity in a realistic way, where data requirement and model outputs parallel current trait collection efforts and field inventories, respectively.

Carbon assimilation is computed over half-hourly period of a representative day per month using the Farquhar, von Caemmerer, and Berry model of photosynthesis (Farquhar *et al.* [1980](#ref-Farquhar1980)). Photosynthetic capacities, as well as leaf respiration rate, are computed from species-specific leaf concentration of nitrogen (N) and phosphorous (P), and leaf mass per area (Domingues *et al.* [2010](#ref-Domingues2010); LMA; Atkin *et al.* [2015](#ref-Atkin2015)). The net amount of assimilated carbon available for growth is then partitioned among the different plant organs using empirical factors, and converted into increments of stem volume and leaf area using species-specific wood-density and LMA respectively. Leaf demography is simulated using species-specific leaf lifespan derived from LMA. Following an underestimation of leaf lifespan for low LMA species, we designed our own leaf lifespan allometry, specific to tropical tree species, to be used in subsequent analysis (see supplementary materials S1). Natural tree deaths are stochastic events whose background rate is negatively correlated with wood density, as observed pan-tropically (Poorter *et al.* [2008](#ref-poorter_are_2008); Kraft & Ackerly [2010](#ref-kraft_functional_2010); Wright *et al.* [2010](#ref-Wright2010)). Additionally, tree can die due to carbon starvation or treefalls. Below-ground processes, herbaceous plants, epiphytes and lianas are not simulated in this version of TROLL. The source code is written in C++ and available at <https://github.com/TROLL-code/TROLL>. A further detailed description of the model is available in Maréchaux & Chave ([2017](#ref-Marechaux2017)).

| Abbreviation                           | Description                                | Units                   |
|:---------------------------------------|:-------------------------------------------|:------------------------|
| *L**M**A*                              | leaf mass per area                         | *g*.*m*<sup>−2</sup>    |
| *N*<sub>*m*</sub>                      | leaf nitrogen content per dry mass         | *m**g*.*g*<sup>−1</sup> |
| *P*<sub>*m*</sub>                      | leaf phosphorous content per dry mass      | *m**g*.*g*<sup>−1</sup> |
| *w**s**g*                              | wood specific gravity                      | *g*.*c**m*<sup>−3</sup> |
| *d**b**h*<sub>*t**h**r**e**s**h*</sub> | diameter at breasth height threshold       | *m*                     |
| *h*<sub>*l**i**m*</sub>                | asymptotic height                          | *m*                     |
| *a*<sub>*h*</sub>                      | parameter of the tree-height-dbh allometry | *m*                     |

A new disturbance module was developed for this study. At a given iteration *d**i**s**t**u**r**b*<sub>*i**t**e**r*</sub>, individual trees are randomly picking following a uniform law and without any individuals nor species targeting. Selected individuals are then removed without triggering a treefall to avoid any side effect. The operation is repeated until the disturbance result in a defined removed basal area (*d**i**s**t**u**r**b*<sub>*i**n**t**e**n**s**i**t**y*</sub>).

Simulation experiment
---------------------

In order to assess the role of biodiversity on ecosystem recovery from disturbance, we simulated forest trajectories for different levels of disturbance intensity and tree community compositions. For each simulation, we first simulated forest regeneration from bare soil for 600 years (pre-disturbance step, Maréchaux & Chave [2017](#ref-Marechaux2017)), then simulated the disturbance described as above (*d**i**s**t**u**r**b*<sub>*i**t**e**r*</sub>), and finally let the simulated forest community freely recover from the disturbance during 600 years (post-disturbance step). Disturbance intensity was quantified by the percentage of basal area loss, here fixed at 0% (control), 25%, 50% and 75%. For each level of disturbance, we performed simulations differing in the original number of species (*S**R* = 15, 25, 125) and composition. For each level of species richness, we created 1000 virtual communities by randomly picking desired number of species among the regional species pool. We used 20 communities for simulations with a large range of convex hull volume *C**V**H* but with a community weighted mean close to the regional species pool community weighted mean. This led to 240 simulations varying in community composition and disturbance intensity (3 *S**R* \* 20 *C**H**V* \* 4 *l**e**v**e**l**s* *o**f* *d**i**s**t**u**r**b**a**n**c**e*).

All simulations were made with a parameterization for an Amazonian forest of French Guiana, with 163 parameterized species, as in Maréchaux & Chave ([2017](#ref-Marechaux2017)).

Analysis
--------

### Quantifying simulated community diversity

We focused on functional richness with convex hull volume *C**H**V* and functional mean with community weighted mean *C**W**M* to define simulation communities. Whereas species and functional diversities were assessed for each simulation at the end of the pre-disturbance step with species richness (*S**R*) and Villeger ([2008](#ref-villeger_dynamique_2008)) indices (*F**R**I**C*, *F**E**v**e*, and *F**D**i**v*).

### Ecosystem recovery from disturbance

**We described the simulated tropical forests from changes in values of forest structure (aboveground biomass (*A**G**B* in *t**o**n* *C*.*h**a*<sup>−1</sup>), basal area (*B**A* in *m*<sup>2</sup>.*h**a*<sup>−1</sup>), total number of stem (*N*), number of stem above 10 *c**m* diameter (*N*10), and number of stem above 30 *c**m* diameter (*N*30)) and in values of forest functioning (growth primary productivity (*G**P**P* in *M**g**C*.*h**a*<sup>−1</sup>), net primary productivity (*N**P**P* in *M**g**C*.*h**a*<sup>−1</sup>), tree autotrophic respiration in day (*R**d**a**y* in *M**g**C*.*h**a*<sup>−1</sup>) and tree autotrophic respiration in night (*R**n**i**g**h**t* in *M**g**C*.*h**a*<sup>−1</sup>)).**

The recovery of the simulated forest ecosystem at a time *t*(*R*(*t*)) regarding a given properties *X* was defined ad follows:

where *X*<sub>*T*</sub>(*t*) and *X*<sub>*C*</sub>(*t*) are the ecosystem metric values at time *t* in the disturbed simulation (*d**i**s**t**u**r**b*<sub>*i**n**t**e**n**s**i**t**y*</sub> = 25%,50%,75%) and in the undisturbed control simulation (*d**i**s**t**u**r**b*<sub>*i**n**t**e**n**s**i**t**y*</sub> = 0%). Note that demographic stochasticity in the model induces a low variability among replicated simulations with the same set-up so that **XX** (Maréchaux & Chave [2017](#ref-Marechaux2017)). When *R*(*t*) approaches *R*<sub>*e**q*</sub> = 1, the disturbed and control systems are considered equivalent, indicating a perfect recovery. We then calculated the euclidean distance to this state of perfect recovery as $d\_{eq}(t) = \\sqrt{(R\_{eq}-R(t))^2}$. **Ecosystem euclidean distance to equilibrium distance was calculated in a multi-dimensional space for (the two functions described above: (i) forest structure (AGB, BA, N, N10, and N30) and (ii) forest functioning (GPP, NPP, Rday, and Rnight). We then integrate the euclidean distances over time to get our ecosystem recovery indicators.** (Figure @ref(fig:datatrans)). We used the cumulative integral after 600 years *I**e**q*<sub>600</sub> as a measurement of ecosystem recovery. A high value of *I**e**q*<sub>600</sub> indicating a slow recovery. The influence of pre-disturbance species richness (*S**R*), functional evenness (*F**E**v**e*) and functional diversity (*F**D**i**v*) on ecosystem recovery index *I**e**q*<sub>600</sub> was finally investigated by linear regression (*I**e**q*<sub>600</sub> ∼ *S**R* + *F**E**v**e* + *F**D**i**v*).

![Ecosystem outputs data transformation. Ecosystem outputs (**A**) are normalized by the control value over time to calculate recovery (**B**); recovery of different ecosystem outputs is then used in a multidimensional space to caluclate ecosystem distance to equilibrium (**C**); finally distance at equilibrium is integrated over time in a cumulative sum (**D**).](draft_files/figure-markdown_github/datatrans-1.png)

### Biodiversity effect

The net effect of biodiversity on ecosystem recovery (NE) is defined as the difference between the ecosystem recovery of the mixed-species community and the one expected under the null hypothesis that there is no effect of biodiversity, i.e. ecosystem recovery for the mixed-species community equals the abundance-weighted sum of that in monoculture (Loreau & Hector [2001](#ref-Loreau2001)). We then split this net biodiversity effect in complementarity and selection effect using Loreau & Hector ([2001](#ref-Loreau2001)) partitioning:

where *N* represents the total number of species, and *M* the vector of monoculture performance. Both metrics depend on the variation of relative ecosystem variable *Δ**R**X*:

where *X*<sub>*s**p*</sub> is the ecosystem variable value for one species either in mixture *X*<sub>*s**p*</sub>(*m**i**x**t**u**r**e*) or in monoculture *X*<sub>*s**p*</sub>(*m**o**n**o**c**u**l**t**u**r**e*). *P*<sub>*s**p*</sub> is the proportion of the species in the mixture represented by species relative abundance. Consequently, *C**E* averages diversity effects of all species presents in the mixture (both negatives and positives). Whereas *S**E* become positive when dominant species outperform themselves in mixture than in monoculture, and negative when less dominant species outperform themselves in mixture than in monoculture (Tobner *et al.* [2016](#ref-Tobner2016)). But similarly, to recovery measurement, biodiversity net effect *N**E* is a dynamic equilibrium and vary over time without disturbance. So in order to correctly assess selection and complementarity effect in answer to disturbance, we normalized it by ecosystem net effect *N**E*<sub>*C*</sub> from the undisturbed control simulation (*d**i**s**t**u**r**b*<sub>*i**n**t**e**n**s**i**t**y*</sub> = 0%) to measure treatments net effect recovery *R*(*N**E*<sub>*T*</sub>):

Recovery trajectories of ecosystem variable after disturbance were partitioned between complementarity effect *C**E* and selection effect *S**E*. In order to do that, we simulated the 163 species individually representing 652 simulations of monoculture.

Results
=======

Ecosystem functions
-------------------

Species richness was not significantly influencing *I**e**q*<sub>600</sub> with forest structure and had a small positive effect on forest production (Table @ref(tab:tgIeq)). Increased functional diversity reduced cumulative integral from ecosystem distance to equilibrium after 600 years (*I**e**q*<sub>600</sub>) and functional evenness was complementary reducing *I**e**q*<sub>600</sub> (Figure @ref(fig:gIeq) and Table @ref(tab:tgIeq)). Finally, low species richness could result in variant *I**e**q*<sub>600</sub>, but increased species richness resulted in increased functional diversity and consequently lower *I**e**q*<sub>600</sub>. We found similar results for all disturbance levels (see \[Appendix 5: Disturbance simulations\]).

![Ecosystem recovery after 600 years with taxonomic and functional diversity for different levels of disturbance. Cumulative integral from ecosystem distance to forest structure equilibrium after 600 years was represented against functional diversity (FDiv, Villéger *et al.* [2008](#ref-villeger_new_2008)) for different level of disturbance (25, 50 and 75% of total basal area); dot shapes represents the species richness whereas dot color represents functional evenness (FEve, Villéger *et al.* [2008](#ref-villeger_new_2008)). Solid lines and grey areas show fitted relationships with their mean and variance of the form *I**e**q*<sub>600</sub> = *F**D**i**v* + *ϵ*.](draft_files/figure-markdown_github/gIeq-1.png)

<table class="table" style="width: auto !important; margin-left: auto; margin-right: auto;">
<caption>
Result of linear regression testing the effect of species richness and functional diversity indices on the recovery index by recovery type and disturbance intensity.
</caption>
<thead>
<tr>
<th style="text-align:left;">
Recovery
</th>
<th style="text-align:left;">
Disturbance intensity
</th>
<th style="text-align:left;">
Variable
</th>
<th style="text-align:right;">
Coefficient
</th>
<th style="text-align:left;">
P-value
</th>
</tr>
</thead>
<tbody>
<tr>
<td style="text-align:left;font-weight: bold;vertical-align: middle !important;" rowspan="9">
structure
</td>
<td style="text-align:left;vertical-align: middle !important;" rowspan="3">
25
</td>
<td style="text-align:left;">
SR
</td>
<td style="text-align:right;">
-0.02
</td>
<td style="text-align:left;">
n.s.
</td>
</tr>
<tr>
<td style="text-align:left;">
FEve
</td>
<td style="text-align:right;">
-3.37
</td>
<td style="text-align:left;">
\*\*\*
</td>
</tr>
<tr>
<td style="text-align:left;">
FDiv
</td>
<td style="text-align:right;">
-9.44
</td>
<td style="text-align:left;">
\*\*\*
</td>
</tr>
<tr>
<td style="text-align:left;vertical-align: middle !important;" rowspan="3">
50
</td>
<td style="text-align:left;">
SR
</td>
<td style="text-align:right;">
-0.26
</td>
<td style="text-align:left;">
.
</td>
</tr>
<tr>
<td style="text-align:left;">
FEve
</td>
<td style="text-align:right;">
-6.93
</td>
<td style="text-align:left;">
\*\*\*
</td>
</tr>
<tr>
<td style="text-align:left;">
FDiv
</td>
<td style="text-align:right;">
-33.21
</td>
<td style="text-align:left;">
\*\*\*
</td>
</tr>
<tr>
<td style="text-align:left;vertical-align: middle !important;" rowspan="3">
75
</td>
<td style="text-align:left;">
SR
</td>
<td style="text-align:right;">
-0.01
</td>
<td style="text-align:left;">
n.s.
</td>
</tr>
<tr>
<td style="text-align:left;">
FEve
</td>
<td style="text-align:right;">
-33.87
</td>
<td style="text-align:left;">
\*\*\*
</td>
</tr>
<tr>
<td style="text-align:left;">
FDiv
</td>
<td style="text-align:right;">
-53.32
</td>
<td style="text-align:left;">
\*\*\*
</td>
</tr>
<tr>
<td style="text-align:left;font-weight: bold;vertical-align: middle !important;" rowspan="9">
production
</td>
<td style="text-align:left;vertical-align: middle !important;" rowspan="3">
25
</td>
<td style="text-align:left;">
SR
</td>
<td style="text-align:right;">
0.71
</td>
<td style="text-align:left;">
\*\*\*
</td>
</tr>
<tr>
<td style="text-align:left;">
FEve
</td>
<td style="text-align:right;">
-11.79
</td>
<td style="text-align:left;">
\*\*\*
</td>
</tr>
<tr>
<td style="text-align:left;">
FDiv
</td>
<td style="text-align:right;">
-4.68
</td>
<td style="text-align:left;">
\*\*\*
</td>
</tr>
<tr>
<td style="text-align:left;vertical-align: middle !important;" rowspan="3">
50
</td>
<td style="text-align:left;">
SR
</td>
<td style="text-align:right;">
1.38
</td>
<td style="text-align:left;">
\*\*\*
</td>
</tr>
<tr>
<td style="text-align:left;">
FEve
</td>
<td style="text-align:right;">
-26.89
</td>
<td style="text-align:left;">
\*\*\*
</td>
</tr>
<tr>
<td style="text-align:left;">
FDiv
</td>
<td style="text-align:right;">
-12.41
</td>
<td style="text-align:left;">
\*\*\*
</td>
</tr>
<tr>
<td style="text-align:left;vertical-align: middle !important;" rowspan="3">
75
</td>
<td style="text-align:left;">
SR
</td>
<td style="text-align:right;">
3.30
</td>
<td style="text-align:left;">
\*\*\*
</td>
</tr>
<tr>
<td style="text-align:left;">
FEve
</td>
<td style="text-align:right;">
-62.07
</td>
<td style="text-align:left;">
\*\*\*
</td>
</tr>
<tr>
<td style="text-align:left;">
FDiv
</td>
<td style="text-align:right;">
-13.06
</td>
<td style="text-align:left;">
\*\*\*
</td>
</tr>
</tbody>
</table>
Biodiversity effect
-------------------

The net effect of biodiversity on ecosystem recovery was partitioned between selection and complementarity effect after normalizing using undisturbed control simulation (*d**i**s**t**u**r**b*<sub>*i**n**t**e**n**s**i**t**y*</sub> = 0%, see Table @ref(tab:tNE)) for every ecosystem global variable, e.g. aboveground biomass (see Figure @ref(fig:gBE)). We found that complementarity effect was dominant in the biodiversity net effect in the first decades. But after few decades the complementarity effect diminished toward an extremely low value. On the contrary, selection effect was reduced in the initial times after disturbance. It increased during the first decades and was then greater. The time lag for which complementarity effect overcame the selection effect increased with disturbance intensity. Finally, 600 years after disturbance, the biodiversity net effect on aboveground biomass was still not at equilibrium for a disturbance intensity greater than 25% of basal area. We found similar results but with an amplified signal for basal area (*B**A*) and stem abundance (*N* but with an inverted signal because of the forest self thinning) (see Supplementary materials S2). Finally, forest growth primary productivity (*G**P**P*) recovered in few years (proportionally to disturbance), and its net effect was maintained by complementarity effect (see Supplementary materials S2).

| variable |     mean|  standard deviation| name                                 | unit                                |
|:---------|--------:|-------------------:|:-------------------------------------|:------------------------------------|
| agb      |   32.721|              17.839| aboveground biomass                  | *t**o**n**C*.*h**a*<sup>−1</sup>    |
| ba       |    1.633|               0.743| basal area                           | *m*<sup>2</sup>.*h**a*<sup>−1</sup> |
| n        |  103.880|             231.623| number of stems                      | *n*.*h**a*<sup>−1</sup>             |
| n10      |   -6.815|              13.003| number of stems above 10cm dbh       | *n*.*h**a*<sup>−1</sup>             |
| gpp      |    0.147|               0.047| growth primary production            | *M**g**C*.*h**a*<sup>−1</sup>       |
| npp      |   -0.041|               0.036| net primary production               | *M**g**C*.*h**a*<sup>−1</sup>       |
| Rday     |    0.046|               0.018| autotrophic respiration during day   | *M**g**C*.*h**a*<sup>−1</sup>       |
| Rnight   |    0.074|               0.030| autotrophic respiration during night | *M**g**C*.*h**a*<sup>−1</sup>       |

![recovery of complementarity and selection effects. Complementarity effect (CE) and selection effect (SE) where normalized by control net effect (NEc), thus measuring their recovery over time. Solid lines represents the mean value whereas areas represents the interval of values among simulations.](draft_files/figure-markdown_github/gBE-1.png)

Discussion
==========

In the limit of the model, we were able to show that functional diversity improved tropical forest recovery from disturbance. More particularly, functional diversity and evenness are key components of diversity in forest recovery trajectory after disturbance. Moreover, we found that complementarity between species was insuring forest recovery in the early times before more productive species dominate the forest and insure late recovery. We thus advocate the view that both diversity theory (with niche complementarity and facilitation) and mass ratio theory (represented by selection) are implied in ecosystem recovery but with relative importance depending on the spatial grain and time since the disturbance event.

Functional diversity improve tropical forest recovery
-----------------------------------------------------

Our results validated the hypothesis of a significant positive relationship between forest recovery and functional diversity and evenness. More particularly, functional diversity (volume of the functional space occupied by the community, Villéger *et al.* [2008](#ref-villeger_new_2008)) seems a major aspect of recovery if it's strengthened by a high functional evenness (regularity of the distribution of abundance in this volume, Villéger *et al.* [2008](#ref-villeger_new_2008)). Indeed, high functional diversity combined to high evenness avoid hegemonic effect of a few dominant species. Our results thus confirms both the review of Díaz & Cabido ([2001](#ref-Diaz2001)),advocating for an under-evaluated importance of plant functional diversity in ecosystem processes, and Zhang *et al.* ([2012](#ref-Zhang2012)) who highlighted the role of evenness in productivity and resilience of terrestrial ecosystems. Finally, species richness is not directly increasing resilience, thus supporting the idea that species diversity is often an inadequate surrogate of functional diversity (Díaz & Cabido [2001](#ref-Diaz2001); but see Poorter *et al.* [2015](#ref-Poorter2015)). Still, increased species richness will increase chance for high functional diversity through the sampling effect (Loreau [1998](#ref-Loreau1998)). An higher sampling of regional species pool will allow a greater chance to pick more functionally diverse species.

<!-- OK good point. But you need to go more into the details of the diversity effect, perhaps highlighting the key choice of the traits? BH -->
Complementarity and selection insure forest recovery
----------------------------------------------------

We found that complementary effect was insuring forest recovery in the beginning of forest successions. We interpreted this result as the consequence of facilitation processes or lower competition due to different niche. As the only resource currently simulated by TROLL is the light, the main facilitation would be light shading of post-pioneer species by pioneer species in disturbance gaps, confirming the study of Morin *et al.* ([2011](#ref-Morin2011)) who also highlighted the importance of facilitation through light shading in forest resilience. But the complementarity effect quickly reduced through time, to let the selection effect insure forest recovery due to an re-enforced dominance of more productive species. The diminishing of complementarity effect is attributed to the selection of the most competitive species though time.

In addition, the study scale matters as shown by Chisholm *et al.* ([2013](#ref-Chisholm2013)) and Sullivan *et al.* ([2017](#ref-Sullivan2017)). In this work, we look at processes to a 16-ha scale, being limited by the computational effort and, our simulation did not include topography resulting in the absence of micro environmental variation affecting both water and nutrient availability. Because several studies suggest that, in mature ecosystems, complementarity will be stronger at smaller scale (Chisholm *et al.* [2013](#ref-Chisholm2013); Sullivan *et al.* [2017](#ref-Sullivan2017)), this could explain the low value of complementarity after the initial stages of forest recovery. Still, the absence of topography and environmental heterogeneity in our simulations could explain why we observed an effect of complementarity to a 16-ha scale, strengthening Sullivan *et al.* ([2017](#ref-Sullivan2017)) interpretation.

Our results follows several studies advocating for multiple mechanisms through which functional diversity affect ecosystem functions. Complementarity effect encompass niche complementarity theory (or diversity theory), which has been shown to indirectly improve forest biomass and coarse wood productivity in subtropical forest (Chiang *et al.* [2016](#ref-Chiang2016)). Similarly, complementarity has been shown of primary importance in grassland functioning (Cardinale *et al.* [2007](#ref-Cardinale2007); Isbell *et al.* [2011](#ref-Isbell2011)). On the other hand, selection effect can be related to the mass ratio hypothesis, which proposes that ecosystem functions are regulated by dominant species of the community (Grime [1998](#ref-Grime1998)). And mass ratio theory has been shown to primarily influence ecosystem functions with biomass accumulation (aboveground and shoots), productivity (coarse wood or aboveground), water use, and light interception for both grassland and subtropical forests (Mokany *et al.* [2008](#ref-Mokany2008); Chiang *et al.* [2016](#ref-Chiang2016)). Consequently, concerning mechanisms responsible for the positive effect of functional diversity on tropical forest functions after disturbance, we also advocate for the interplay of both niche complementarity and mass ratio theories, depending on time since the disturbance event and the spatial grain.

Finally, our findings confirm results from experimental studies. Williams *et al.* ([2017](#ref-Williams2017)) also found experimentally an over yielding due to complementarity effect based on light and spatial complementarity with tree crown of young trees. In addition, Tobner *et al.* ([2016](#ref-Tobner2016)) studied 4-years stand in low diverse forests of Canada. They also found that selection effect was greater than complementarity in most of the cases, promoting the idea that mass ratio theory is the primary mechanisms involved in functional diversity effect on ecosystem functions (Mokany *et al.* [2008](#ref-Mokany2008)).

Conclusion
----------

We used closed forest system simulated with TROLL forest model to evaluate the role and mechanisms of biodiversity in tropical forest recovery from disturbance, and thus in tropical forest resilience. We found that diversity improved forest recovery, similarly to productivity (Poorter *et al.* [2015](#ref-Poorter2015); Liang *et al.* [2016](#ref-Liang2016)). Additionally, we found that complementarity between species was insuring forest recovery in forest succession start with facilitation, before more productive species dominate the forest and insure the final forest recovery.

Supplementary materials
=======================

-   Supplementary materials S1: Leaf lifespan model
    -   [HTML](S1.html)
    -   [PDF](S1.pdf)
-   Supplementary materials S2: Disturbance simulations
    -   [HTML](S2.html)
    -   [PDF](S2.pdf)

References
==========

Asner, G.P., Knapp, D.E., Broadbent, E.N., Oliveira, P.J.C., Keller, M. & Silva, J.N. (2005). Selective Logging in the Brazilian Amazon. *Science*, **310**. Retrieved from <http://science.sciencemag.org/content/310/5747/480>

Atkin, O.K., Bloomfield, K.J., Reich, P.B., Tjoelker, M.G., Asner, G.P., Bonal, D., B??nisch, G., Bradford, M.G., Cernusak, L.A., Cosio, E.G., Creek, D., Crous, K.Y., Domingues, T.F., Dukes, J.S., Egerton, J.J.G., Evans, J.R., Farquhar, G.D., Fyllas, N.M., Gauthier, P.P.G., Gloor, E., Gimeno, T.E., Griffin, K.L., Guerrieri, R., Heskel, M.A., Huntingford, C., Ishida, F.Y., Kattge, J., Lambers, H., Liddell, M.J., Lloyd, J., Lusk, C.H., Martin, R.E., Maksimov, A.P., Maximov, T.C., Malhi, Y., Medlyn, B.E., Meir, P., Mercado, L.M., Mirotchnick, N., Ng, D., Niinemets, ?., O’Sullivan, O.S., Phillips, O.L., Poorter, L., Poot, P., Prentice, I.C., Salinas, N., Rowland, L.M., Ryan, M.G., Sitch, S., Slot, M., Smith, N.G., Turnbull, M.H., Vanderwel, M.C., Valladares, F., Veneklaas, E.J., Weerasinghe, L.K., Wirth, C., Wright, I.J., Wythers, K.R., Xiang, J., Xiang, S. & Zaragoza-Castells, J. (2015). Global variability in leaf respiration in relation to climate, plant functional types and leaf traits. *New Phytologist*, **206**, 614–636. Retrieved from <http://doi.wiley.com/10.1111/nph.13253>

Avila, A.L. de, Ruschel, A.R., Carvalho, J.O.P. de, Mazzei, L., Silva, J.N.M., Lopes, J. do C., Araujo, M.M., Dormann, C.F. & Bauhus, J. (2015). Medium-term dynamics of tree species composition in response to silvicultural intervention intensities in a tropical rain forest. *Biological Conservation*, **191**, 577–586. Retrieved from <http://dx.doi.org/10.1016/j.biocon.2015.08.004>

Baraloto, C., Paine, C.E.T., Poorter, L., Beauchene, J., Bonal, D., Domenach, A.M., Hérault, B., Patiño, S., Roggy, J.C. & Chave, J. (2010). Decoupled leaf and stem economics in rain forest trees. *Ecology Letters*, **13**, 1338–1347.

Blaser, J., Sarre, A., Poore, D. & Johnson, S. (2011). No Title. *International Tropical Timber Organization, Yokohoma, Japan*.

Burivalova, Z., Şekercioǧlu, Ç.H. & Koh, L.P. (2014). Thresholds of logging intensity to maintain tropical forest biodiversity. *Current Biology*, **24**, 1893–1898. Retrieved from <https://www.sciencedirect.com/science/article/pii/S0960982214007829>

Cadotte, M.W., Carscadden, K. & Mirotchnick, N. (2011). Beyond species: Functional diversity and the maintenance of ecological processes and services. **48**, 1079–1087. Retrieved from <http://doi.wiley.com/10.1111/j.1365-2664.2011.02048.x>

Cardinale, B.J., Srivastava, D.S., Duffy, J.E., Wright, J.P., Downing, A.L., Sankaran, M., Jouseau, C., Cadotte, M.W., Carroll, I.T., Weis, J.J., Hector, A. & Loreau, M. (2009). Effects of biodiversity on the functioning of ecosystems: a summary of 164 experimental manipulations of species richness (W.K. Michener, Ed.). *Ecology*, **90**, 854–854. Retrieved from <http://doi.wiley.com/10.1890/08-1584.1>

Cardinale, B.J., Wright, J.P., Cadotte, M.W., Carroll, I.T., Hector, A., Srivastava, D.S., Loreau, M. & Weis, J.J. (2007). Impacts of plant diversity on biomass production increase through time because of species complementarity. *Proceedings of the National Academy of Sciences of the United States of America*, **104**, 18123–8. Retrieved from [http://www.ncbi.nlm.nih.gov/pubmed/17991772 http://www.pubmedcentral.nih.gov/articlerender.fcgi?artid=PMC2084307](http://www.ncbi.nlm.nih.gov/pubmed/17991772 http://www.pubmedcentral.nih.gov/articlerender.fcgi?artid=PMC2084307)

Chave, J. (1999). Study of structural, successional and spatial patterns in tropical rain forests using TROLL, a spatially explicit forest model. *Ecological Modelling*, **124**, 233–254.

Chiang, J., Spasojevic, M.J., Muller-Landau, H.C., Sun, I., Lin, Y., Su, S., Chen, Z.-S., Chen, C., Swenson, N.G. & McEwan, R.W. (2016). Functional composition drives ecosystem function through multiple mechanisms in a broadleaved subtropical forest. *Oecologia*, **182**, 829–840. Retrieved from [https://link.springer.com/content/pdf/10.1007/s00442-016-3717-z.pdf http://link.springer.com/10.1007/s00442-016-3717-z](https://link.springer.com/content/pdf/10.1007/s00442-016-3717-z.pdf http://link.springer.com/10.1007/s00442-016-3717-z)

Chisholm, R.A., Muller-Landau, H.C., Abdul Rahman, K., Bebber, D.P., Bin, Y., Bohlman, S.A., Bourg, N.A., Brinks, J., Bunyavejchewin, S., Butt, N., Cao, H., Cao, M., Cárdenas, D., Chang, L.-W., Chiang, J.-M., Chuyong, G., Condit, R., Dattaraja, H.S., Davies, S., Duque, A., Fletcher, C., Gunatilleke, N., Gunatilleke, S., Hao, Z., Harrison, R.D., Howe, R., Hsieh, C.-F., Hubbell, S.P., Itoh, A., Kenfack, D., Kiratiprayoon, S., Larson, A.J., Lian, J., Lin, D., Liu, H., Lutz, J.A., Ma, K., Malhi, Y., McMahon, S., McShea, W., Meegaskumbura, M., Mohd. Razman, S., Morecroft, M.D., Nytch, C.J., Oliveira, A., Parker, G.G., Pulla, S., Punchi-Manage, R., Romero-Saltos, H., Sang, W., Schurman, J., Su, S.-H., Sukumar, R., Sun, I.-F., Suresh, H.S., Tan, S., Thomas, D., Thomas, S., Thompson, J., Valencia, R., Wolf, A., Yap, S., Ye, W., Yuan, Z. & Zimmerman, J.K. (2013). Scale-dependent relationships between tree species richness and ecosystem function in forests (D. Coomes, Ed.). *Journal of Ecology*, **101**, 1214–1224. Retrieved from <http://doi.wiley.com/10.1111/1365-2745.12132>

Davidson, E.A., De Araüjo, A.C., Artaxo, P., Balch, J.K., Brown, I.F., Mercedes, M.M., Coe, M.T., Defries, R.S., Keller, M., Longo, M., Munger, J.W., Schroeder, W., Soares-Filho, B.S., Souza, C.M. & Wofsy, S.C. (2012). The Amazon basin in transition. **481**, 321–328. Retrieved from <https://www.nature.com/articles/nature10717>

Díaz, S. & Cabido, M. (2001). Vive la différence: Plant functional diversity matters to ecosystem processes. **16**, 646–655. Retrieved from <http://linkinghub.elsevier.com/retrieve/pii/S0169534701022832>

Domingues, T.F., Meir, P., Feldpausch, T.R., Saiz, G., Veenendaal, E.M., Schrodt, F., Bird, M., Djagbletey, G., Hien, F., Compaore, H., Diallo, A., Grace, J. & Lloyd, J. (2010). Co-limitation of photosynthetic capacity by nitrogen and phosphorus in West Africa woodlands. *Plant, Cell and Environment*, **33**, 959–980. Retrieved from <http://doi.wiley.com/10.1111/j.1365-3040.2010.02119.x>

Farquhar, G.D., Caemmerer, S. von & Berry, J.A. (1980). A biochemical model of photosynthetic CO2 assimilation in leaves of C3 species. *Planta*, **149**, 78–90. Retrieved from <http://link.springer.com/10.1007/BF00386231>

Grime, J.P. (1998). Benefits of plant diversity to ecosystems: Immediate, filter and founder effects. **86**, 902–910. Retrieved from <http://doi.wiley.com/10.1046/j.1365-2745.1998.00306.x>

Gunderson, L. (2010). Ecological and human community resilience in response to natural disasters. *Ecology and Society*, **15**, 29. Retrieved from <http://www.ecologyandsociety.org/vol15/iss2/art18/>

Hector, A. & Loreau, M. (2005). Relationships between biodiversity and production in grasslands at local and regional scales. *Grassland: A Global Resource*, 295–304.

Herold, M., Román-Cuesta, R., Mollicone, D., Hirata, Y., Van Laake, P., Asner, G.P., Souza, C., Skutsch, M., Avitabile, V. & MacDicken, K. (2011). Options for monitoring and estimating historical carbon emissions from forest degradation in the context of REDD+. *Carbon Balance and Management*, **6**, 13. Retrieved from [https://www.biomedcentral.com/track/pdf/10.1186/1750-0680-6-13?site=cbmjournal.springeropen.com http://cbmjournal.springeropen.com/articles/10.1186/1750-0680-6-13](https://www.biomedcentral.com/track/pdf/10.1186/1750-0680-6-13?site=cbmjournal.springeropen.com http://cbmjournal.springeropen.com/articles/10.1186/1750-0680-6-13)

Hérault, B. & Piponiot, C. (2018). Key drivers of ecosystem recovery after disturbance in a neotropical forest. *Forest Ecosystems*, **5**, 2. Retrieved from <https://forestecosyst.springeropen.com/articles/10.1186/s40663-017-0126-7>

Hérault, B., Bachelot, B., Poorter, L., Rossi, V., Bongers, F., Chave, J., Paine, C.E.T., Wagner, F. & Baraloto, C. (2011). Functional traits shape ontogenetic growth trajectories of rain forest tree species: {{}Plant{}} traits shape growth trajectory. *Journal of Ecology*, **99**, 1431–1440. Retrieved from <http://doi.wiley.com/10.1111/j.1365-2745.2011.01883.x>

Hooper, D.U., Chapin, F.S., Ewel, J.J., Hector, A., Inchausti, P., Lavorel, S., Lawton, J.H., Lodge, D.M., Loreau, M., Naeem, S., Schmid, B., Setälä, H., Symstad, A.J., Vandermeer, J. & Wardle, D.A. (2005). Effects of biodiversity on ecosystem functioning: A consensus of current knowledge. *Ecological Monographs*, **75**, 3–35. Retrieved from <http://doi.wiley.com/10.1890/04-0922>

Isbell, F., Calcagno, V., Hector, A., Connolly, J., Harpole, W.S., Reich, P.B., Scherer-Lorenzen, M., Schmid, B., Tilman, D., Ruijven, J. van, Weigelt, A., Wilsey, B.J., Zavaleta, E.S. & Loreau, M. (2011). High plant diversity is needed to maintain ecosystem services. *Nature*, **477**, 199–202. Retrieved from [https://www.nature.com/nature/journal/v477/n7363/pdf/nature10282.pdf http://www.nature.com/doifinder/10.1038/nature10282](https://www.nature.com/nature/journal/v477/n7363/pdf/nature10282.pdf http://www.nature.com/doifinder/10.1038/nature10282)

Ives, A.R. & Carpenter, S.R. (2007). Stability and diversity of ecosystems. **317**, 58–62. Retrieved from <http://www.ncbi.nlm.nih.gov/pubmed/17615333>

Kattge, J., Diaz, S., Lavorel, S., Prentice, I.C., Leadley, P., B??nisch, G., Garnier, E., Westoby, M., Reich, P.B., Wright, I.J., Cornelissen, J.H.C., Violle, C., Harrison, S.P., Van Bodegom, P.M., Reichstein, M., Enquist, B.J., Soudzilovskaia, N.A., Ackerly, D.D., Anand, M., Atkin, O., Bahn, M., Baker, T.R., Baldocchi, D., Bekker, R., Blanco, C.C., Blonder, B., Bond, W.J., Bradstock, R., Bunker, D.E., Casanoves, F., Cavender-Bares, J., Chambers, J.Q., Chapin, F.S., Chave, J., Coomes, D., Cornwell, W.K., Craine, J.M., Dobrin, B.H., Duarte, L., Durka, W., Elser, J., Esser, G., Estiarte, M., Fagan, W.F., Fang, J., Fern??ndez-M??ndez, F., Fidelis, A., Finegan, B., Flores, O., Ford, H., Frank, D., Freschet, G.T., Fyllas, N.M., Gallagher, R.V., Green, W.A., Gutierrez, A.G., Hickler, T., Higgins, S.I., Hodgson, J.G., Jalili, A., Jansen, S., Joly, C.A., Kerkhoff, A.J., Kirkup, D., Kitajima, K., Kleyer, M., Klotz, S., Knops, J.M.H., Kramer, K., K??hn, I., Kurokawa, H., Laughlin, D., Lee, T.D., Leishman, M., Lens, F., Lenz, T., Lewis, S.L., Lloyd, J., Llusi??, J., Louault, F., Ma, S., Mahecha, M.D., Manning, P., Massad, T., Medlyn, B.E., Messier, J., Moles, A.T., M??ller, S.C., Nadrowski, K., Naeem, S., Niinemets, ?., N??llert, S., N??ske, A., Ogaya, R., Oleksyn, J., Onipchenko, V.G., Onoda, Y., Ordo??ez, J., Overbeck, G., Ozinga, W.A., Pati??o, S., Paula, S., Pausas, J.G., Pe??uelas, J., Phillips, O.L., Pillar, V., Poorter, H., Poorter, L., Poschlod, P., Prinzing, A., Proulx, R., Rammig, A., Reinsch, S., Reu, B., Sack, L., Salgado-Negret, B., Sardans, J., Shiodera, S., Shipley, B., Siefert, A., Sosinski, E., Soussana, J.F., Swaine, E., Swenson, N., Thompson, K., Thornton, P., Waldram, M., Weiher, E., White, M., White, S., Wright, S.J., Yguel, B., Zaehle, S., Zanne, A.E. & Wirth, C. (2011). TRY - a global database of plant traits. *Global Change Biology*, **17**, 2905–2935. Retrieved from <http://doi.wiley.com/10.1111/j.1365-2486.2011.02451.x>

Kazmierczak, M., Wiegand, T. & Huth, A. (2014). A neutral vs. non-neutral parametrizations of a physiological forest gap model. *Ecological Modelling*, **288**, 94–102. Retrieved from <https://www.sciencedirect.com/science/article/pii/S0304380014002270>

Köhler, P. & Huth, A. (1998). The effects of tree species grouping in tropical rainforest modelling: Simulations with the individual-based model FORMIND. *Ecological Modelling*, **109**, 301–321. Retrieved from <http://www.sciencedirect.com/science/article/pii/S0304380098000660>

Kraft, N.J.B. & Ackerly, D.D. (2010). Functional trait and phylogenetic tests of community assembly across spatial scales in an {{}Amazonian{}} forest. *Ecological Monographs*, **80**, 401–422. Retrieved from <http://onlinelibrary.wiley.com/doi/10.1890/09-1672.1/full>

Lewis, S.L., Edwards, D.P. & Galbraith, D. (2015). Increasing human dominance of tropical forests. **349**, 827–832. Retrieved from <http://www.ncbi.nlm.nih.gov/pubmed/26293955>

Liang, J., Crowther, T.W., Picard, N., Wiser, S., Zhou, M., Alberti, G., Schulze, E.-D., McGuire, D., Bozzato, F., Pretzsch, H., De-Miguel, S., Paquette, A., Hérault, B., Scherer-Lorenzen, M., Barrett, C.B., Glick, H.B., Hengeveld, G.M., Nabuurs, G.-J., Pfautsch, S., Viana, H., Vibrans, A.C., Ammer, C., Schall, P., Verbyla, D., Tchebakova, N., Fischer, M., Watson, J.V., Chen, H.Y., Lei, X., Schelhaas, M.-J., Lu, H., Gianelle, D., Parfenova, E.I., Salas, C., Lee, E., Lee, B., Kim, H.S., Bruelheide, H., Coomes, D.A., Piotto, D., Sunderland, T., Schmid, B., Gourlet-Fleury, S., Sonké, B., Tavani, R., Zhu, J., Brandl, S., Vayreda, J., Kitahara, F., Searle, E.B., Neldner, V.J., Ngugi, M.R., Baraloto, C., Frizzera, L., Bałazy, R., Oleksyn, J., Zawiła-Niedźwiecki, T., Bouriaud, O., Bussotti, F., Finér, L., Jaroszewicz, B., Jucker, T., Valladares, F., Jagodzinski, A.M., Peri, P.L., Gonmadje, C., Marthy, W., O’Brien, T., Martin, E.H., Marshall, A., Rovero, F., Bitariho, R., Niklaus, P.A., Alvarez-Loayza, P., Chamuya, N., Valencia, R., Mortier, F., Wortel, V., Engone-Obiang, N.L., Ferreira, L.V., Odeke, D.E., Vasquez, R.M. & Reich, P.B. (2016). Positive biodiversity–productivity relationship predominant in global forests. *Science*, **354**, 196. Retrieved from <http://science.sciencemag.org/content/354/6309/aaf8957>

Loreau, M. (2010). Linking biodiversity and ecosystems: towards a unifying ecological theory. *Philosophical transactions of the Royal Society of London. Series B, Biological sciences*, **365**, 49–60. Retrieved from [http://apps.webofknowledge.com/full{\\\_}record.do?product=WOS{\\&}search{\\\_}mode=CitingArticles{\\&}qid=7{\\&}SID=V1TwrrLNJKUhYkGvYOi{\\&}page=10{\\&}doc=91{\\&}cacheurlFromRightClick=no](http://apps.webofknowledge.com/full{\_}record.do?product=WOS{\&}search{\_}mode=CitingArticles{\&}qid=7{\&}SID=V1TwrrLNJKUhYkGvYOi{\&}page=10{\&}doc=91{\&}cacheurlFromRightClick=no)

Loreau, M. (1998). Separating Sampling and Other Effects in Biodiversity Experiments. *Oikos*, **82**, 600. Retrieved from <http://www.jstor.org/stable/3546381?origin=crossref>

Loreau, M. & Hector, a. (2001). Partitioning selection and complementarity in biodiversity experiments. *Nature*, **412**, 72–6. Retrieved from <http://www.ncbi.nlm.nih.gov/pubmed/11452308>

Loreau, M. & Mazancourt, C. de. (2013). Biodiversity and ecosystem stability: A synthesis of underlying mechanisms (E. Duffy, Ed.). *Ecology Letters*, **16**, 106–115. Retrieved from <http://doi.wiley.com/10.1111/ele.12073>

Maréchaux, I. & Chave, J. (2017). An individual-based forest model to jointly simulate carbon and tree diversity in Amazonia: description and applications. *Ecological Monographs*, **87**, 632–664. Retrieved from <http://doi.wiley.com/10.1002/ecm.1271>

Mokany, K., Ash, J. & Roxburgh, S. (2008). Functional identity is more important than diversity in influencing ecosystem processes in a temperate native grassland. *Journal of Ecology*, **96**, 884–893. Retrieved from <http://doi.wiley.com/10.1111/j.1365-2745.2008.01395.x>

Morin, X., Fahse, L., Mazancourt, C. de, Scherer-Lorenzen, M. & Bugmann, H. (2014). Temporal stability in forest productivity increases with tree diversity due to asynchrony in species dynamics (M. Rejmanek, Ed.). *Ecology Letters*, **17**, 1526–1535. Retrieved from <http://doi.wiley.com/10.1111/ele.12357>

Morin, X., Fahse, L., Scherer-Lorenzen, M. & Bugmann, H. (2011). Tree species richness promotes productivity in temperate forests through strong complementarity between species. *Ecology Letters*, **14**, 1211–1219. Retrieved from <http://doi.wiley.com/10.1111/j.1461-0248.2011.01691.x>

Paquette, A. & Messier, C. (2011). The effect of biodiversity on tree productivity: From temperate to boreal forests. *Global Ecology and Biogeography*, **20**, 170–180. Retrieved from <http://doi.wiley.com/10.1111/j.1466-8238.2010.00592.x>

Pearson, T.R.H., Brown, S., Murray, L. & Sidman, G. (2017). Greenhouse gas emissions from tropical forest degradation: an underestimated source. *Carbon Balance and Management*, **12**, 3. Retrieved from [http://www.atmos-chem-phys.net/10/11707/2010/ http://cbmjournal.springeropen.com/articles/10.1186/s13021-017-0072-2](http://www.atmos-chem-phys.net/10/11707/2010/ http://cbmjournal.springeropen.com/articles/10.1186/s13021-017-0072-2)

Poorter, L., Sande, M.T. van der, Arets, E.J., Ascarrunz, N., Enquist, B., Finegan, B., Licona, J.C., Martínez-Ramos, M., Mazzei, L., Meave, J.A., Muñoz, R., Nytch, C.J., Oliveira, A.A. de, Pérez-García, E.A., Prado-Junior, J., Rodríguez-Velázques, J., Ruschel, A.R., Salgado-Negret, B., Schiavini, I., Swenson, N.G., Tenorio, E.A., Thompson, J., Toledo, M., Uriarte, M., Hout, P. van der, Zimmerman, J.K. & Peña-Claros, M. (2017). Biodiversity and climate determine the functioning of Neotropical forests. *Global Ecology and Biogeography*, **26**, 1423–1434. Retrieved from <http://doi.wiley.com/10.1111/geb.12668>

Poorter, L., Sande, M.T. van der, Thompson, J., Arets, E.J., Alarcón, A., Álvarez-Sánchez, J., Ascarrunz, N., Balvanera, P., Barajas-Guzmán, G., Boit, A., Bongers, F., Carvalho, F.A., Casanoves, F., Cornejo-Tenorio, G., Costa, F.R., Castilho, C.V. de, Duivenvoorden, J.F., Dutrieux, L.P., Enquist, B.J., Fernández-Méndez, F., Finegan, B., Gormley, L.H., Healey, J.R., Hoosbeek, M.R., Ibarra-Manríquez, G., Junqueira, A.B., Levis, C., Licona, J.C., Lisboa, L.S., Magnusson, W.E., Martínez-Ramos, M., Martínez-Yrizar, A., Martorano, L.G., Maskell, L.C., Mazzei, L., Meave, J.A., Mora, F., Muñoz, R., Nytch, C., Pansonato, M.P., Parr, T.W., Paz, H., Pérez-García, E.A., Rentería, L.Y., Rodríguez-Velazquez, J., Rozendaal, D.M., Ruschel, A.R., Sakschewski, B., Salgado-Negret, B., Schietti, J., Simões, M., Sinclair, F.L., Souza, P.F., Souza, F.C., Stropp, J., Steege, H. ter, Swenson, N.G., Thonicke, K., Toledo, M., Uriarte, M., Hout, P. van der, Walker, P., Zamora, N. & Peña-Claros, M. (2015). Diversity enhances carbon storage in tropical forests. *Global Ecology and Biogeography*, **24**, 1314–1328. Retrieved from <http://doi.wiley.com/10.1111/geb.12364>

Poorter, L., Wright, S.J., Paz, H., Ackerly, D.D., Condit, R., Ibarra-Manríquez, G., Harms, K.E., Licona, J.C., Martínez-Ramos, M., Mazer, S.J. & Others. (2008). Are functional traits good predictors of demographic rates? {{}Evidence{}} from five neotropical forests. *Ecology*, **89**, 1908–1920. Retrieved from <http://www.esajournals.org/doi/abs/10.1890/07-0207.1>

Purves, D. & Pacala, S. (2008). Predictive models of forest dynamics. **320**, 1452–1453. Retrieved from <http://www.ncbi.nlm.nih.gov/pubmed/18556548>

Putz, F.E. & Redford, K.H. (2010). The importance of defining ’Forest’: Tropical forest degradation, deforestation, long-term phase shifts, and further transitions. *Biotropica*, **42**, 10–20. Retrieved from <http://doi.wiley.com/10.1111/j.1744-7429.2009.00567.x>

Rutishauser, E., Hérault, B., Baraloto, C., Blanc, L., Descroix, L., Sotta, E.D., Ferreira, J., Kanashiro, M., Mazzei, L., D’Oliveira, M.V., De Oliveira, L.C., Peña-Claros, M., Putz, F.E., Ruschel, A.R., Rodney, K., Roopsind, A., Shenkin, A., Da Silva, K.E., De Souza, C.R., Toledo, M., Vidal, E., West, T.A., Wortel, V. & Sist, P. (2015). Rapid tree carbon stock recovery in managed Amazonian forests. *Current Biology*, **25**, R787–R788. Retrieved from <https://www.sciencedirect.com/science/article/pii/S0960982215008684>

Sakschewski, B., Bloh, W. von, Boit, A., Poorter, L., Peña-Claros, M., Heinke, J., Joshi, J. & Thonicke, K. (2016). Resilience of Amazon forests emerges from plant trait diversity. *Nature Climate Change*, **6**, 1032–1036. Retrieved from <http://www.nature.com/doifinder/10.1038/nclimate3109>

Schnitzer, S.A. & Carson, W.P. (2016). Would Ecology Fail the Repeatability Test? **66**, 98–99. Retrieved from <http://academic.oup.com/bioscience/article/66/2/98/2468677/Would-Ecology-Fail-the-Repeatability-Test>

Simula, M. (2009). Towards defining forest degradation: comparative analysis of existing definitions. 62. Retrieved from [http://www.ardot.fi/Documents{\\\_}2/Degradationdefintions.pdf](http://www.ardot.fi/Documents{\_}2/Degradationdefintions.pdf)

Sist, P., Rutishauser, E., Peña-Claros, M., Shenkin, A., Hérault, B., Blanc, L., Baraloto, C., Baya, F., Benedet, F., Silva, K.E. da, Descroix, L., Ferreira, J.N., Gourlet-Fleury, S., Guedes, M.C., Bin Harun, I., Jalonen, R., Kanashiro, M., Krisnawati, H., Kshatriya, M., Lincoln, P., Mazzei, L., Medjibé, V., Nasi, R., D’Oliveira, M.V.N., Oliveira, L.C. de, Picard, N., Pietsch, S., Pinard, M., Priyadi, H., Putz, F.E., Rodney, K., Rossi, V., Roopsind, A., Ruschel, A.R., Shari, N.H.Z., Rodrigues de Souza, C., Susanty, F.H., Sotta, E.D., Toledo, M., Vidal, E., West, T.A., Wortel, V. & Yamada, T. (2015). The Tropical managed forests Observatory: A research network addressing the future of tropical logged forests (M. Chytrý, Ed.). *Applied Vegetation Science*, **18**, 171–174. Retrieved from <http://doi.wiley.com/10.1111/avsc.12125>

Sullivan, M.J., Talbot, J., Lewis, S.L., Phillips, O.L., Qie, L., Begne, S.K., Chave, J., Cuni-Sanchez, A., Hubau, W., Lopez-Gonzalez, G., Miles, L., Monteagudo-Mendoza, A., Sonké, B., Sunderland, T., Ter Steege, H., White, L.J., Affum-Baffoe, K., Aiba, S.I., De Almeida, E.C., De Oliveira, E.A., Alvarez-Loayza, P., Dávila, E.Á., Andrade, A., Aragão, L.E., Ashton, P., Aymard, G.A., Baker, T.R., Balinga, M., Banin, L.F., Baraloto, C., Bastin, J.F., Berry, N., Bogaert, J., Bonal, D., Bongers, F., Brienen, R., Camargo, J.L.C., Cerón, C., Moscoso, V.C., Chezeaux, E., Clark, C.J., Pacheco, Á.C., Comiskey, J.A., Valverde, F.C., Coronado, E.N., Dargie, G., Davies, S.J., De Canniere, C., Djuikouo, M.N., Doucet, J.L., Erwin, T.L., Espejo, J.S., Ewango, C.E., Fauset, S., Feldpausch, T.R., Herrera, R., Gilpin, M., Gloor, E., Hall, J.S., Harris, D.J., Hart, T.B., Kartawinata, K., Kho, L.K., Kitayama, K., Laurance, S.G., Laurance, W.F., Leal, M.E., Lovejoy, T., Lovett, J.C., Lukasu, F.M., Makana, J.R., Malhi, Y., Maracahipes, L., Marimon, B.S., Junior, B.H.M., Marshall, A.R., Morandi, P.S., Mukendi, J.T., Mukinzi, J., Nilus, R., Vargas, P.N., Camacho, N.C., Pardo, G., Peña-Claros, M., Pétronelli, P., Pickavance, G.C., Poulsen, A.D., Poulsen, J.R., Primack, R.B., Priyadi, H., Quesada, C.A., Reitsma, J., Réjou-Méchain, M., Restrepo, Z., Rutishauser, E., Salim, K.A., Salomão, R.P., Samsoedin, I., Sheil, D., Sierra, R., Silveira, M., Slik, J.W., Steel, L., Taedoumg, H., Tan, S., Terborgh, J.W., Thomas, S.C., Toledo, M., Umunay, P.M., Gamarra, L.V., Vieira, I.C.G., Vos, V.A., Wang, O., Willcock, S. & Zemagho, L. (2017). Diversity and carbon storage across the tropical forest biome. *Scientific Reports*, **7**, 39102. Retrieved from <http://www.nature.com/articles/srep39102>

Tilman, D., Reich, P.B., Knops, J., Wedin, D., Mielke, T. & Lehman, C. (2001). Diversity and Productivity in a Long-Term Grassland Experiment. *Science*, **294**.

Tobner, C.M., Paquette, A., Gravel, D., Reich, P.B., Williams, L.J. & Messier, C. (2016). Functional identity is the main driver of diversity effects in young tree communities (F. He, Ed.). **19**, 638–647. Retrieved from <http://doi.wiley.com/10.1111/ele.12600>

Veblen, T.T.T. (1992). Regeneration dynamics. *Plant succession: Theory and prediction*, **11**, 152—–87. Retrieved from [http://books.google.com/books?hl=en{\\&}lr={\\&}id=N3kyrwCznc8C{\\&}oi=fnd{\\&}pg=PA152{\\&}dq=Regeneration+Dynamics{\\&}ots=P5wKKCL-uZ{\\&}sig=Uz{\\\_}YoUYI0xhN2F76k7isKxZYgmU](http://books.google.com/books?hl=en{\&}lr={\&}id=N3kyrwCznc8C{\&}oi=fnd{\&}pg=PA152{\&}dq=Regeneration+Dynamics{\&}ots=P5wKKCL-uZ{\&}sig=Uz{\_}YoUYI0xhN2F76k7isKxZYgmU)

Villeger, S. (2008). *Dynamique de la diversité fonctionnelle des communautés de poissons ({Lagune} de {Terminos}, {Mexique})*. PhD thesis thesis, Montpellier SupAgro. Retrieved from <http://archimer.ifremer.fr/doc/00000/6178/>

Villéger, S., Mason, N.W.H. & Mouillot, D. (2008). New multidimensional functional diversity indices for a multifaceted framework in functional ecology. *Ecology*, **89**, 2290–2301. Retrieved from <http://doi.wiley.com/10.1890/07-1206.1>

Williams, L.J., Paquette, A., Cavender-Bares, J., Messier, C. & Reich, P.B. (2017). Spatial complementarity in tree crowns explains overyielding in species mixtures. *Nature Ecology and Evolution*, **1**, 63. Retrieved from <http://www.ncbi.nlm.nih.gov/pubmed/28812675>

Wright, S.J., Kitajima, K., Kraft, N.J., Reich, P.B., Wright, I.J., Bunker, D.E., Condit, R., Dalling, J.W., Davies, S.J., DíAz, S., Engelbrecht, B.M., Harms, K.E., Hubbell, S.P., Marks, C.O., Ruiz-Jaen, M.C., Salvador, C.M. & Zanne, A.E. (2010). Functional traits and the growth-mortality trade-off in tropical trees. *Ecology*, **91**, 3664–3674. Retrieved from [https://conservancy.umn.edu/bitstream/handle/11299/174640/Wright et al 2010.pdf?sequence=1{\\&}isAllowed=y](https://conservancy.umn.edu/bitstream/handle/11299/174640/Wright et al 2010.pdf?sequence=1{\&}isAllowed=y)

Zhang, Y., Chen, H.Y.H. & Reich, P.B. (2012). Forest productivity increases with evenness, species richness and trait variation: A global meta-analysis. *Journal of Ecology*, **100**, 742–749. Retrieved from <http://doi.wiley.com/10.1111/j.1365-2745.2011.01944.x>
