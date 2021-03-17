---
title: Hackathon projects
menu_title: Projects
menu_icon: briefcase
permalink: /projects/
---

### What is the transient sea level sensitivity in CMIP6 models?
#### Jon Bamber (Bristol)
{:.secondary}

> Many will be familiar with the concept of transient climate sensitivity: what
> is the transient temperature response to a doubling in CO2 concentrations?
> This is a key question for understanding the response of the climate system to
> CO2 forcing. But there are other important transient responses we need to
> understand. One of these is the response of global mean sea level to CO2
> forcing, which we can call the Transient Sea Level Sensitivity (TSLS). Sea
> level rise is one of the most serious consequences of climate warming but
> making projections of it has proved challenging. The TSLS will depend on the
> coupled climate system response and how glaciers and ice sheets respond to
> atmospheric and oceanic changes. The aim of this project is to determine the
> TSLS of CMIP6 coupled models for the 21st century and to compare this to the
> TSLS that has been estimated for CMIP5 and previous IPCC class experiments in
> Grinsted and Christensen 2021. This will be achieved by determining the mean
> response of the oceans and land ice to a change in temperature averaged over
> multiple decades. We will also explore the spread in TSLS amongst model
> simulations and the level of confidence we have in the ensemble mean.
>
> - Grinsted, A., and J. H. Christensen (2021), The transient sensitivity of sea
>   level rise, Ocean Sci., 17(1), 181-186, doi:10.5194/os-17-181-2021.

### How well do the CMIP6 models represent the tropical rainfall belt over Africa?
#### Katy Sheen (Exeter) and David Macleod (Bristol)
{:.secondary}

> Movement of the tropical rain belt (TRB) is arguably the most important
> determinant of regional climate in Africa: its average seasonal position
> defines humidity or aridity and fluctuations lead to flooding or drought.
> Accurate simulation of the TRB is thus essential to build confidence in future
> projections of regional African rainfall. However it has been shown that
> previous generations of climate models have shown significant problems with
> fundamental aspects of TRB seasonality, particularly over East Africa (Tierney
> et al. 2015). Here we propose to evaluate the representation of the TRB in
> CMIP6 models. Existing code is available (Nikulin and Hewitson 2019), which
> can be used to swiftly assess representation of key attributes of the TRB.
> From this a more in-depth focus on regional aspects of TRB variability, such
> as the TRB-influence on Sahel summer rainfall, and its representation in
> models can be explored, along with future projections.
>
> - Nikulin, G. and Hewitson, B., 2019. A simple set of indices describing the
>   Tropical Rain Belt over central and southern Africa. Atmospheric Science
>   Letters, 20(12), p.e946.
> - Tierney, J.E., Ummenhofer, C.C. and  Demenocal, P.B., 2015. Past and future
>   rainfall in the Horn of Africa. Science advances, 1(9), p.e1500682.

### Characterising the marine carbon cycle in CMIP6
#### Oliver Andrews (Bristol) and Jamie Wilson (Bristol)
{:.secondary}

> Recent ocean heat uptake has been unprecedented, with the last five years
> being the warmest in recorded history. Superimposed on this secular trend,
> human-induced warming of the oceans has also caused more persistent and
> intense periods of extreme sea surface temperature, termed ‘marine heatwaves’.
> Marine heatwaves can rapidly disrupt marine life and commercial fisheries as
> organisms are exposed to extreme conditions outside of their normal ranges.
> Recent high-profile marine heatwaves, most notably in the North Pacific, have
> triggered mass die-offs and shifts in ecosystem structure. Alongside this,
> climate-driven changes in marine biogeochemistry, particularly ocean
> deoxygenation and acidification, are imposing additional stress on marine
> ecosystems. Just as for heatwaves, more extreme shifts in biogeochemistry are
> an expected consequence of climate change, and individual cases of extreme,
> inhospitable low-oxygen or low-pH conditions are on the rise. However, the
> increased persistence of marine biogeochemical extremes in a changing climate
> remains underexplored by the scientific community, despite major consequences
> for ecosystem stability.
>
> Plankton ecosystems continuously sequester ~1700 Pg of carbon from the
> atmosphere in the deep ocean via sinking particles of organic matter. The
> production of these particles is projected to decrease during the 21st century
> in response to warming-driven stratification of the surface ocean (Bopp et
> al., 2013). However, models are now including newly identified processes, such
> as temperature-dependent degradation, that influence how far these particles
> sink into the oldest deep ocean which in turns changes how long that carbon is
> stored for. However, this is not consistent across models. The impact of these
> new processes on future projections has yet to be quantified – do they change
> future projections of biologically sequestered carbon? Does the varied
> representation of sinking particles influence projections?
>
> In this hackathon group we will use CMIP6 data (OMIP, DAMIP, scenarioMIP) to
> assess historical and projected future changes in marine biogeochemistry from
> timescales of daily extremes to long term (multidecadal) carbon storage.
>
> Possible outcomes:
> 1. Marine extreme events atlas: Mapping present and future co-occurrence of
>    marine heatwaves + biogeochemical extremes (and their physical drivers –
>    including stratification, eddy influence, atmospheric heatwaves). Specific
>    focus will be given to high SST, low chlorophyll extremes.
> 2. Future changes in biological carbon sequestration: Quantifying present and
>    future carbon sequestration by marine biology across different models.
>    Specific focus will be given to identifying the role of biological and
>    physical drivers.
>
> Possible methods: 
> - (compound) extreme event statistics
> - climate attribution
> - analysis of physical drivers (eddy-tracking, Lagrangian framework)
> - downscaling or bias adjustment
> - analysis of biological drivers (export production, degradation of organic
>   carbon)
> - quantifying carbon storage using apparent oxygen utilisation
>
> Possible CMIP6 outputs to target:
> - experiments: piControl, historical, hist-NAT, hist-GHG, sspXXX
> - ocean outputs: thetao, so, mlotstmax, moltsmin, uo, vo, ssh  (Omon); tos,
>   sos (Oday) 
> - ocnBiogeochem outputs: o2, o2sat, ph, co3satarag, co3satcal, expc, epc100,
>   intpp, diss14cabio, dissoc (Omon); chlos and phycos (Oday) 

### Testing proxies of AMOC variability in CMIP6
#### Rory Bingham (Bristol)
{:.secondary}

> The Atlantic meridional overturning circulation (AMOC) plays an important role
> in regulating Earth's climate. Concerns over its stability in a warming
> climate have prompted a concerted effort to monitor the AMOC in recent
> decades, most prominently with the RAPID array at 26N. Yet, such direct
> observational records are still too short to discriminate between natural
> decadal variability and long-term decline. This has motivated the development
> and use of indirect AMOC proxies, based more readily observed quantities such
> as sea surface temperature and coastal sea level for which long-term records
> do exist. However, these proxies are founded on correlations and plausible
> physical relationship rather than robustly established dynamical links.
> Moreover, relationships may not be exclusive, with factors other than AMOC
> variability also driving changes in the proxy variables (e.g., sea level or
> SST), with relative contributions of AMOC and non-AMOC factors potentially
> also being timescale dependent. The CMIP6 data provide an ideal opportunity to
> test the robustness of AMOC proxies, the aim of this project. First, the
> zonally-integrated meridional transport (ZIMT) will be calculated from the
> model velocity fields and various statistical approaches used to characterise
> ZIMT variability. Next, a range of commonly used AMOC proxies will be
> diagnosed from the model output and the strength of their relationship with
> the ZIMT assessed. Novel proxies may also be sought and tested. We may also
> consider whether there is a relationship between a model’s ability to
> represent a proxy quantity and the realism of its AMOC judged, as far as is
> possible, against the RAPID array data. Finally, based on the strength of the
> proxies we will attempt to assess the most likely behaviour of the AMOC over
> the last century.  

### The atmospheric response to sea-ice loss in the PAMIP experiments and its sensitivity to model biases
#### James Screen (Exeter) and Stephen Thompson (Exeter)
{:.secondary}

> Polar amplification, the phenomenon that external radiative forcing produces a
> larger change in surface temperature at high latitudes than the global
> average, is a key aspect of anthropogenic climate change, but its causes and
> consequences are not fully understood. The Polar Amplification Model
> Intercomparison Project (PAMIP) seeks to improve our understanding of this
> phenomenon through a coordinated set of numerical model experiments. As one of
> the Coupled Model Intercomparison Project Phase 6 (CMIP6) endorsed MIPs, PAMIP
> addresses the how the global climate system responds to changes in Arctic and
> Antarctic sea ice. The PAMIP community will convene for a remote workshop in
> late March to share scientific results and to facilitate/foster collaborative
> studies based on the PAMIP multi-model experiment database. The workshop will
> inspire the choice of priority topics for focussed attention during the CMIP6
> Hackathon, with a view toward accelerating the analysis and publication of the
> PAMIP multi-model experiments. Early results from the PAMIP suggest that the
> atmospheric response to future sea-ice loss is model dependent, particularly
> in the stratosphere. One focus of analysis will be attempting to explain the
> diversity in the response to sea-ice loss across CMIP6 models to model biases,
> particularly in the upper troposphere and lower stratosphere.

### Differences between 'turning down the sun' and stratospheric sulfate injection
#### Matthew Henry (Exeter)
{:.secondary}

> Solar geoengineering refers to the idea of deliberately increasing Earth's
> albedo to temporarily cool the planet while we cut emissions and remove
> greenhouse gases from the atmosphere. There are many ways this could be
> achieved, the most studied is stratospheric sulfate injection, which mimics what
> happens during a volcanic eruption. The increase in Earth's albedo is not the
> only effect of stratospheric sulfate injection, yet many studies just reduce the
> solar constant (or 'turn down the sun') to simulate solar geoengineering. As
> part of the Geoengineering Model Intercomparison Project (GeoMIP), the G6sulfur
> and G6solar simulations reduce the warming from the high-tier emission scenario
> to the medium-tier emission scenario by adding a stratospheric sulfate aerosol
> layer (G6sulfur) or a uniform reduction in the solar constant (G6solar). By
> analysing the differences between these two simulations, we can isolate the
> climate impacts of stratospheric aerosol injection that arise independently from
> the increase in Earth's albedo.
> 
> - https://agupubs.onlinelibrary.wiley.com/doi/10.1029/2020JD033952

### Uncertainty in sea-ice-cloud feedbacks across the CMIP6 ensemble
#### Jo Browse (Exeter) and Tony Payne (Bristol)
{:.secondary}

> To what extent will constraining sea-ice-cloud feedbacks reduce uncertainty in
> our understanding of Arctic amplification and global climate sensitivity? Both
> observations and modelling studies have evidenced the importance of polar clouds
> (and aerosol) in controlling the surface energy budget at high-latitudes.
> High-latitude clouds are highly sensitive to changes in aerosol concentration
> and strongly coupled to sea-ice processes. Thus, our expectation is that
> high-latitude clouds will fundamentally change in a warming world with the
> potential to both mitigate or enhance warming at high-latitudes. However, both
> high-latitude cloud and aerosol have (historically) been poorly simulated in
> global climate models and across CMIP6 we predict significant variation in model
> outcomes with respect to high-latitude cloud forcings. In this project we will
> quantify the importance of sea-ice cloud feedbacks across CMIP6 ensembles and
> estimate the impact of constraining this feedback on our understanding of Arctic
> amplification and global climate sensitivity.

### Interactive graphics of key CMIP6-based IPCC figures
#### Mat Collins (Exeter)
{:.secondary}

> Figures in IPCC reports, especially those in the Summaries for Policy Makers,
> are often densely packed with information from multiple sources. This makes it
> challenging to understand the full impact of the figure without having
> additional information. This project will investigate adding interactive
> elements to key IPCC figures from the 5th Assessment Report or other recent
> Special Reports. These elements could include highlighting key aspects and
> relating them to key conclusions, adding numerical values or even animating
> graphics. The possibilities are endless.

### Impacts of changing wind regimes and sea ice on the world's longest migrant
#### Joanne Morten (Exeter), Lucy Hawkes (Exeter) and Will Thurston (Exeter)
{:.secondary}

> Arctic terns are one of very few species in the world to spend considerable
> parts of time every year at both poles, migrating at least 90,000 km per year
> between the two (1, 2), which is the longest recorded migration of any animal.
> They are particularly vulnerable to climate change, with a short window to breed
> in their arctic range during the boreal summer, their reliance on tailwinds to
> support both their south- and north- bound migrations (3), and their use of sea
> ice to forage in the Southern Ocean during the austral summer. Using tracking
> data (from breeding arctic terns caught in Greenland (1) and Sweden (4)), and
> Iceland,  we are interested in investigating how predicted changes over the next
> 100 years will impact the winds that migrating arctic terns rely on, and how the
> changing ice edge will affect their foraging during the non-breeding period.
> 
> 1. Egevang C, Stenhouse IJ, Phillips RA, Petersen A, Fox JW, Silk JR (2010)
>    Tracking of Arctic terns Sterna paradisaea reveals longest animal migration
>    Proc Natl Acad Sci U S A 107:2078-2081 doi:10.1073/pnas.0909493107
> 2. Fijn RC, Hiemstra D, Phillips RA, van der Winden J (2013) Arctic Terns Sterna
>    paradisaea from The Netherlands migrate record distances across three oceans
>    to Wilkes Land, East Antarctica Ardea 101:3-12 doi:Doi 10.5253/078.101.0102
> 3. Hromádková T, Pavel V, Flousek J, Briedis M (2020) Seasonally specific
>    responses to wind patterns and ocean productivity facilitate the longest
>    animal migration on Earth. Mar Ecol Prog Ser 638:1-12.
>    https://doi.org/10.3354/meps13274
> 4. Alerstam, T, Bäckman, J, Grönroos, J, Olofsson, P, Strandberg, R (2019)
>    Hypotheses and tracking results about the longest migration: The case of the
>    arctic tern. Ecol Evol 9: 9511– 9531. https://doi.org/10.1002/ece3.5459"

### Human heat stress in a warming world
#### Chris Smith (Leeds)
{:.secondary}

> Climate projections tend to agree that extremes of heat over the populated
> land surface areas of the world will rise faster than the global mean surface
> temperature (Samset et al., 2018; Schleussner et al., 2016; Seneviratne and
> Hauser, 2020). Traditional extremes of heat and other climate indices defined
> by the ETCCDI such as monthly maximum temperature or heatwave duration (Zhang
> et al., 2011) do not directly estimate the impacts on human welfare. In this
> work I propose to directly compute a metric of human heat stress, the
> Universal Thermal Climate Index (UTCI; Błazejczyk et al., 2013), using CMIP6
> projections. This work will build on the work of Claudia Di Napoli (U.
> Reading) who has used UTCI in the present climate with reanalysis data (Di
> Napoli et al., 2020). Claudia or others from Reading could be invited to
> collaborate on this project as part of the MOAP group.
>
> The work would proceed as follows:
> 1. obtaining 3-hourly CMIP6 data from participating CMIP6 models. The
>    following variables are required on 3-hour resolution: tas, hurs, rlds,
>    rlus, rsus, rsds, plus one of rsdsdiff or rsdt, and ideally (vas and uas)
>    or sfcWind
> 2. Bias-correction of this data to correct for any model biases in absolute
>    temperatures in the present-day and recent past.
> 3. Calculation of UTCI from the bias-corrected data
> 4. Presenting the change in UTCI, and absolute projected UTCI, as spatial
>    plots under different SSP scenarios at the end of the 21st Century
> 5. Determining the change in UTCI as a function of global mean surface
>    temperature for each of the Giorgi world regions (Giorgi and Francisco,
>    2000), allowing these projections to be scenario-independent and coupled to
>    a simple emissions-based climate model (Smith et al., 2018).
> 6. Implementation of this into an interactive web tool showing regional heat
>    stress as a function of global mean temperature change. Open-source tools
>    for calculating UTCI from climate data are already available , and the hope
>    is that this project will help develop this software repository further to
>    be more useful to the research community.
>
> References
> - Błazejczyk, K., Jendritzky, G., Bröde, P., Fiala, D., Havenith, G., Epstein,
>   Y., et al. (2013). An introduction to the Universal thermal climate index
>   (UTCI). Geogr. Pol. 86, 5–10. doi:10.7163/GPol.2013.1.
> - Di Napoli, C., Hogan, R. J., and Pappenberger, F. (2020). Mean radiant
>   temperature from global-scale numerical weather prediction models. Int. J.
>   Biometeorol. 64, 1233–1245. doi:10.1007/s00484-020-01900-5.
> - Giorgi, F., and Francisco, R. (2000). Uncertainties in regional climate
>   change prediction: A regional analysis of ensemble simulations with the
>   HADCM2 coupled AOGCM. Clim. Dyn. 16, 169–182. doi:10.1007/PL00013733.
> - Samset, B. H., Sand, M., Smith, C. J., Bauer, S. E., Forster, P. M.,
>   Fuglestvedt, J. S., et al. (2018). Climate Impacts From a Removal of
>   Anthropogenic Aerosol Emissions. Geophys. Res. Lett. 45, 1020–1029.
>   doi:10.1002/2017GL076079.
> - Schleussner, C. F., Lissner, T. K., Fischer, E. M., Wohland, J., Perrette,
>   M., Golly, A., et al. (2016). Differential climate impacts for
>   policy-relevant limits to global warming: The case of 1.5 °c and 2 °c. Earth
>   Syst. Dyn. 7, 327–351. doi:10.5194/esd-7-327-2016.
> - Seneviratne, S. I., and Hauser, M. (2020). Regional Climate Sensitivity of
>   Climate Extremes in CMIP6 Versus CMIP5 Multimodel Ensembles. Earth’s Futur.
>   8, e2019EF001474. doi:10.1029/2019EF001474.
> - Smith, C. J., Forster, P. M., Allen, M., Leach, N., Millar, R. J.,
>   Passerello, G. A., et al. (2018). FAIR v1.3: a simple emissions-based
>   impulse response and carbon cycle model. Geosci. Model Dev. 11, 2273–2297.
>   doi:10.5194/gmd-11-2273-2018.
> - Zhang, X., Alexander, L., Hegerl, G. C., Jones, P., Tank, A. K., Peterson,
>   T. C., et al. (2011). Indices for monitoring changes in extremes based on
>   daily temperature and precipitation data. Wiley Interdiscip. Rev. Clim.
>   Chang. 2, 851–870. doi:10.1002/wcc.147.

### Rainfall extremes and groundwater recharge in the tropics
#### Richard Taylor (UCL)
{:.secondary}

> As the planet warms, substantial uncertainty remains in where, when and how
> much rain and snow will fall. A consistent, observed impact of global warming
> is the intensification of precipitation, particularly acute in the tropics,
> which results in fewer light rain events and more frequent, heavy rainfalls.
> The consequences of this changing distribution in precipitation globally
> include reduced soil moisture, more frequent and intense floods as well as
> longer and more frequent droughts. There is, however, mounting evidence of a
> possible 'silver lining' to these changes in the form of a distinct bias in
> groundwater replenishment to heavy, extreme rainfall. This bias is observed on
> a variety of timesteps (extreme annual, monthly, daily, hourly rainfall) and
> scales from a few square kilometres by piezometry to a hundred thousand square
> kilometres using GRACE satellite data. Understanding the magnitude of the
> projected intensification of rainfall in the tropics on annual to hourly
> timesteps will not only inform increased flood risk but also the opportunities
> that may be provided by groundwater for adaptation in the tropics to the
> amplification of drought.

