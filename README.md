Analysis of Confirmed COVID-19 Cases by Age in US States
================
Alan Farahani

  - [Introduction](#introduction)
  - [Methods and Materials](#methods-and-materials)
  - [Major Trends](#major-trends)
  - [Recommendations](#recommendations)

# Introduction

The rapidity of the spread of the novel coronavirus, COVID-19, is one of
the most notable features of this disease. Much scientific and
journalistic investigation into the epidemiological aspects of the
coronavirus have focused on *case fatality rates* (CFRs) and other
demographic variables that may contribute to increased morbidity. For
instance, it has been argued based on data deriving from China, and more
recently the CDC, that CFRs for those under 40 are relatively low.

In contrast, less attention has been given to the *case detection rate*
(CDR) by age, except in cases where the asymptomatic nature of
transmission has been noted, especially in younger age groups. This
analysis aggregates available data from US states to identify which age
groups are potentially leaders in CDRs, and the extent to which this is
variable by state or a broader consequence of the disease. All analyses
are for visualization purposes – no inferential statistics have been
employed due to the inherent biases emanating from under-testing of the
US population.

First, thanks are given to the site www.covidtracking.com, which has
provided the links to various state pages with demographic data. Second,
this is an ongoing “document” that is updated every day. The paragraph
below describes the represented date range of data and states
represented. Unfortunately, due to the vagaries of state reporting, most
states do not provide sufficient data to conduct these analyses. For
comments, concerns, or access to higher resolution data, please contact
me at <alanfarahani@gmail.com>.  A full HTML file that contains reproducible R code
(raw data pending) is available in the repository as "covid19_age_demographics.html". 
Download that HTML file and open it in any browser.

The assembled data extend from 2020-03-24 to 2020-03-27, and comprise 10
unique states (the states represented are California, Colorado,
Connecticut, Georgia, Louisiana, Massachussets, Nevada, Oregon,
Tennessee, Washington) for a total of 17357 confirmed cases.

# Methods and Materials

Data are acquired from state sources where age-demographic material is
published
(e.g. <https://www.cdph.ca.gov/Programs/CID/DCDC/Pages/Immunization/ncov2019.aspx>).
In most cases, states provide either the raw case count or a proportion
of cases followed by an absolute number of confirmed cases.

Screenshots of all of the state pages are taken, and the data are
hand-recorded into an excel spreadsheet that contains untransformed
data. In one case (the state of Connecticut), absolute numeric data
apart from the total number of confirmed cases are not provided.
Nevertheless a graph is – therefore counts for each age range were
estimated visually and the sum of these counts was made to match the
published confirmed cases. Therefore it is possible there is some error
(\~ +/-10) associated with the estimates for this state.

![Representative example of data supplied by the state of Nevada
regarding distribution of confirmed cases across age ranges. Accessed on
26-03-2020.](covid19_demographics2_git_files/figure-gfm/Screenshot_2020-03-26%20Power%20BI%20Report.png)

# Major Trends

Without transformation of the age-ranges, the percent of confirmed cases
by ages as of 2020-03-27 can be seen in the figure below.

![Percent of confirmed COVID-19 cases by age-range given by state
authorities.](covid19_demographics2_git_files/figure-gfm/state-dist-1.png)

Grouping of states by commonly used age-ranges reveals additional
insights into the age-structure of those confirmed with the novel
coronavirus. It can be observed that contrary to widespread assumptions,
positive carriers of the novel coronavirus (at least those who were
symptomatic or suspicious enough of their condition to seek testing),
can range uniformly across age groups. Inter-state differences must be
accounted for either by a) patterns of community spread of the virus
specific to the social dynamics of those states and/or b) patterns of
testing based on the ability of state officials (and representatives) to
respond.

The groups represented in the figure above are the following:

1.  Colorado, Connecticut, Massachussets, Nevada, Oregon, Washington

![Percent of confirmed COVID-19 cases by age-range across states, where
it is possible to group states by
age-range.](covid19_demographics2_git_files/figure-gfm/new-state-dist-1.png)

The figure below illustrates the new cases by age according to absolute
case count.

![Absolute number of confirmed COVID-19 cases by age-range across
states, where it is possible to group states by
age-range.](covid19_demographics2_git_files/figure-gfm/new-state-dist-case-1.png)

The absolute change in the age-demographic profile of recent confirmed
COVID-19 cases can be seen in the figure below. It is important to note
that some states are actively in the process of changing their
age-reporting ranges, and so many states (such as Georgia) may not have
cumulative case data that concords with previously published data.

![Absolute change in confirmed coronavirus cases where the black points
represent all previously aggregated data. The colors and size of the
rightmost points indicate the intensity of the proportional
change.](covid19_demographics2_git_files/figure-gfm/covid-case-change-1.png)

# Recommendations

In order to effectively combat the spread of the novel coronavirus, data
on community transmission is needed. In particular, understanding how
and why the virus spreads among certain age demographics rather than
others can help official planners respond in advance to possible
transmission scenarios. Furthermore, these data are also essential in
messaging to all populations, especially those with maximal visibility
in flouting physical distancing recommendations, that transmission of
the virus is more demographically widespread than perhaps assumed.
