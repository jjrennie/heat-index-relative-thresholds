# Extreme Heat: It's All Relative! 
## A Lesson on the Heat Index and Why the Mountains Aren't Always an Escape from It.
## Written By Jared Rennie (@jjrennie)

I do not like the heat, yet whenever I complain about it in the mountains of North Carolina, I always get the following comment:

<span style="color: red">***"aT lEaSt yOu dOn'T lIvE iN rAlEiGh or cHaRlOtTe wHeRe iT's mUcH hOtTeR"***</span>

Sure, it's much hotter at lower elevations, but I don't live in Raleigh or Charlotte, *I LIVE IN THE WESTERN NORTH CAROLINA MOUNTAINS* so extreme heat in our area can still have an impact, even if it's in the low to mid 90s. It may not affect all of us, but it certainly <a href='https://www.weather.gov/images/wrn/Infographics/_heat-vulnerable-populations-descriptions.png' target='blank'>affects those vulnerable to heat</a>.

Another gripe I have is that <a href='https://journals.ametsoc.org/view/journals/wcas/9/1/wcas-d-15-0037_1.xml' target="_blank">according to the National Weather Service</a>, a heat advisory is issued ANYWHERE IN THE STATE OF NORTH CAROLINA if the heat Index is 105°F.

***Um...what?*** 

It has NEVER gotten to 105 here in the mountains. No wonder why we have <a href='https://mesonet.agron.iastate.edu/plotting/auto/plot/90/t:state::v:total::ilabel:no::geo:ugc::drawc:yes::year:1986::year2:2025::sdate:1986-01-01%200000::edate:2025-08-20%200000::network:WFO::station:DMX::state:NC::fema:7::phenomena:HT::significance:Y::cmap:YlOrRd::_r:t::dpi:100.png' target='_blank'>NEVER BEEN ISSUED A HEAT ADVISORY IN OUR AREA!!!</a>

Just because we do not get triple digit heat a lot does not mean we are exempted from heat exteremes and associated impacts!

**And I'm going to prove it to you using data and statistics!**

This notebook will tap into data archived by <a href='https://www.ncei.noaa.gov/' target="_blank">NOAA's National Centers for Environmetal Information</a>, calculate the Heat Index used by the National Weather Service, and use statistical percentiles to show what thresholds would be considered out of the ordinary, thus showing heat can still be a problem in the mountains.

**YES, I AM THAT PETTY!**

The dataset we will be using is from the Global Historical Climatology Network's (GHCN's) hourly dataset, which includes multiple sources of US and international data, including airport data from the ASOS network. If you would like to learn more about this dataset, check out the information below. 

- GHCNh Info: https://www.ncei.noaa.gov/products/global-historical-climatology-network-hourly
- GHCNh Documentation: https://www.ncei.noaa.gov/oa/global-historical-climatology-network/hourly/doc/ghcnh_DOCUMENTATION.pdf

This notebook is designed so you do not have to download any data locally, and with just a few lines of code, you can develop data and plots at your fingertips. Let's get into it!

### What You Need

First off, the entire codebase works in Python 3. In addition to base Python, you will need the following packages installed: 
- pandas and numpy (to slice annd dice the data)
- matplotlib (to make pretty plots)

The "easiest" way is to install these is by installing <a href='https://www.anaconda.com' target="_blank">anaconda</a>, and then applying <a href='https://conda-forge.org/' target="_blank">conda-forge</a>. Afterward, then you can install the above packages. 

### Launch automatically with Binder:
[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/jjrennie/heat-index-relative-thresholds/HEAD?urlpath=%2Fdoc%2Ftree%2Fghcnh_heatIndex.ipynb)
