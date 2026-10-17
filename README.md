# Free Datasets for Social Science Research
This is a compilation of free datasets that I hope can be useful to students, professors, and others for research, data visualization, etc. Most of the datasets are publicly available, but some aren't and require data agreements. If you have any additions (including new datasets or filling in details on existing entries), changes, or comments, please [contribute](https://github.com/toddrjones/datasets/blob/main/contributing.md)!

 \- [Todd Jones](https://www.toddrjones.com/)

--- 

### Contents

Skip to: [Time Use](#time-use), [Crime](#crime), [US Censuses and Economic History](#us-censuses-and-economic-history), [Household Surveys](#household-surveys), [Mobility and Migration](#mobility-and-migration), [Names](#names), [Injury and death](#injury-and-death), [Crashes and traffic](#crashes-and-traffic), [Education](#education), [Academia](#academia), [Temperature](#temperature), [Family](#family), [Sports](#sports), [Religion](#religion), [Government](#government), [Inflation and cost of living](#inflation-and-cost-of-living), [Working](#working), [Businesses](#businesses), [Politics and voting](#politics-and-voting), [Health, public health, and epidemiology](#health-public-health-and-epidemiology), [Real estate](#real-estate), [Patents](#patents), [Social networks](#social-networks), [Beliefs and values](#beliefs-and-values), [Law](#law), [Environment and energy](#environment-and-energy), [Shopping](#shopping), [Maps and geography](#maps-and-geography), [States, conflict, and regimes](#states-conflict-and-regimes), [Macroeconomics](#macroeconomics)

---

### Time Use

- [American Time Use Survey (ATUS)](https://www.bls.gov/tus/) - 24-hour US time diaries
  - Years: 2003-present; Access: Public; There is also an IPUMS [version](https://www.atusdata.org/atus/)
  - Includes minute-by-minute information on which  of hundreds of activities the person is doing. For most activities, there is also information on where and with whom the activity occurred.
  - The ATUS is a sample of the Current Population Survey (CPS), to which it can be linked.
  - Sample paper: [Parental and Student Time Use Around the Academic Year](https://www.sciencedirect.com/science/article/pii/S0167268124001598)
- [Multinational Time Use Study](https://www.mtusdata.org/mtus/) - Time diaries from a number of countries
  - Years: varies. Access: Requires IPUMS data agreement.

---

### Crime

- [National Incident-based Reporting System (NIBRS)](https://www.icpsr.umich.edu/sites/icpsr/view/studies/118281/versions/V11) - Individual-level crime data covering much of the US
  - Years: 1991-present. This version was standardized and compiled by Jacob Kaplan.
  - Includes information like offender age, sex, and race; victim age, sex, and race; type of offense; time of offense; location of offense; and relationship between victim and offender.
  - The geography is police agency, so the individual crimes are not geocoded.
    - [Useful crosswalk to get more information about the police agencies](https://www.icpsr.umich.edu/web/ICPSR/studies/35158/versions/V2)
  - Sample paper: [School and Crime](https://www.toddrjones.com/papers/School_Crime_most_recent.pdf)
- [National Crime Victimization Survey (NCVS)](https://www.icpsr.umich.edu/sites/nacjd/view/collections/95) - Self-reported victimization data
  - Years: 1992-present. This version is from ICPSR.
- City-level crime data - many cities have individual-level, geocoded crime data. A small number of examples:
  - [New York City](https://www.nyc.gov/site/nypd/stats/crime-statistics/citywide-crime-stats.page)
  - [Chicago](https://data.cityofchicago.org/Public-Safety/Crimes-2001-to-Present/ijzp-q8t2/about_data)
  - [Los Angeles](https://data.lacity.org/Public-Safety/Crime-Data-from-2020-to-2024/2nrs-mtv8/about_data)
  - [Seattle](https://data.seattle.gov/Public-Safety/SPD-Crime-Data-2008-Present/tazs-3rd5/about_data)
  - See also [this site](https://osf.io/zyaqn/wiki?wiki=t69q3), [this site](https://www.policedatainitiative.org/datasets/), and [this older site](http://us-city.census.okfn.org/dataset/crime-stats.html) each of which detail availability for many cities
  - And [OpenPoliceData](https://github.com/openpolicedata/openpolicedata), which compiles data from many sources
- 911 calls - many cities have data on 911 calls. A small number of examples:
  - [New York](https://data.cityofnewyork.us/Public-Safety/NYPD-Calls-for-Service-Year-to-Date-/n2zq-pubd/about_data)
  - [Los Angeles](https://data.lacity.org/Public-Safety/LAPD-Calls-for-Service-2024-to-Present/xjgu-z4ju/about_data)
  - [Seattle](https://www.seattle.gov/police/information-and-data/data/public-data-sets)
- [Stanford Open Policing Project](https://openpolicing.stanford.edu/) - Data on millions of police traffic stops across locations
- [Justice Outcomes Explorer](https://www.census.gov/data/experimental-data-products/justice-outcomes-explorer.html) - Collaboration between University of Michigan's [Criminal Justices Administrative Records System](https://cjars.org/) and the U.S. Census Bureau. Years covered: 2000-2020 (varies by jurisdiction). Criminal justice involvement includes criminal charges, prison releases, and probation and parole sentences. Outcomes: employment, earnings, government program participation, and mortality.

---

### US Censuses and Economic History

- [1850-1880 and 1900-1950 individual-level full count US Censuses](https://usa.ipums.org/usa/)
  - This version is from IPUMS, which requires an agreement.
    - IPUMS also has samples of some of the later Censuses
  - Information varies by year, but includes fields like age, sex, race, occupation, household structure, etc. Sometimes earnings and years of education.
  - It does not include name or address.
- [OpenCensus](https://opencensus.us/)
   - A project that is initially working to make the 1940 Census publicly available, so it includes name, address, etc.
- Individual-level links between Censuses
    - [Census Tree](https://www.censustree.org/) - The largest set of links and good coverage for women. It uses information from the world's largest family tree, [FamilySearch](https://www.familysearch.org/en/united-states/), to create the links. 
    - [IPUMS](https://usa.ipums.org/usa/) has its own links
    - Another option is the [Census Linking Project](https://censuslinkingproject.org/) 
- [Census Place Project](https://www.icpsr.umich.edu/sites/icpsr/view/studies/179401/versions/V2.1) - Census links to standardized and geocoded place names.
- [CenSoc](https://censoc.berkeley.edu/) - Links between the 1940 Census and death records.

---

### Household Surveys

- [American Community Survey (ACS)](https://usa.ipums.org/usa/) - Like a more-detailed version of the US Census, but only a sample of the population participates
  - Repeated cross-section. You can access it, e.g., via IPUMS (above link) or the [tidycensus](https://walker-data.com/tidycensus/) R package (requires a Census API key).
  - Depending on the geography, you can get a large number of variables like demographics, income, travel time to work, college major, industry, home value, and primary heating source.
- [Current Population Survey (CPS)](https://cps.ipums.org/cps/) - Large US labor force survey
  - Years: 1962-present. This version is via IPUMS.
  - A person participates every month for four months, takes eight months off, then does four more months.
  - A subset of the CPS participates in the ATUS (see above).
- [Panel Study of Income Dynamics (PSID)](https://psidonline.isr.umich.edu/) - long-running panel household survey
- [National Longitudinal Study of Youth (NLSY79 and NLSY97)](https://www.bls.gov/nls/cohorts.htm) - detailed, long-running panel surveys
  - NLSY79 follows people born 1957-64, with the first interview in 1979
  - NLSY97 follows people born 1980-84, with the first interview in 1997
- [IPUMS International](https://international.ipums.org/international/) - 100+ countries, 650+ surveys, 1B+ records
  - Massive, standardized compilation of censuses and surveys
 - [Household Pulse Survey/Household Trends and Outlook Pulse Survey](https://www.census.gov/programs-surveys/household-pulse-survey/data/datasets.html) Collected starting April 23, 2020 to measure timely issues affecting U.S. households. Household Pulse Survey ended on September 16, 2024 and was relaunched as Household Trends and Outlook Survey in early October 2024. 
  
---

### Mobility and Migration

- [MIGRATE](https://www.nature.com/articles/s41467-025-68019-2) - yearly migration patterns between US Census Blocks
  - From [Inferring fine-grained migration patterns across the United States](https://www.nature.com/articles/s41467-025-68019-2)
- [Opportunity Atlas](https://www.opportunityatlas.org/) - many adult outcomes of children at very fine-grained geographies
   - From [The Opportunity Atlas: Mapping the Childhood Roots of Social Mobility](https://opportunityinsights.org/wp-content/uploads/2018/10/atlas_paper.pdf) and [Changing Opportunity: Sociological Mechanisms Underlying Growing Class Gaps and Shrinking Race Gaps in Economic Mobility](https://opportunityinsights.org/wp-content/uploads/2024/07/ChangingOpportunity_Paper.pdf)
- [Migration Patterns](https://migrationpatterns.org/) - Counts of children commuting zone to adult commuting zone migration patterns, split by race and parental income
   - From [The Radius of Economic Opportunity: Evidence from Migration and Local Labor Markets](https://www2.census.gov/ces/wp/2022/CES-WP-22-27.pdf)

---

### Names

- [SSA baby names](https://www.ssa.gov/oact/babynames/limits.html) – Frequencies of baby names by year from the Social Security Administration
  - Years: 1880–present; Access: Public
  - Data presented separately by male and female and by state. Minimum 5 names.
  - Fun [article](https://nameberry.com/blog/most-popular-names-how-the-list-was-born) about the origins of these data.
- [England and Wales names](https://www.ons.gov.uk/releases/babynamesinenglandandwales2025#data) - Baby names from the Office of National Statistics
  - Years: 1996-present
  - Minimum 3 names.
- [US Census names](https://www.census.gov/topics/population/genealogy/data.html) - Most commonly-occurring first and last names in the US
  - Years: 1990, 2000, 2010, 2020. Access: Public
- [Facebook Name List](https://web.archive.org/web/20220119175817/http://sites.google.com/site/facebooknamelist/namelist) - How often names are male and female
  - Access: Public

 ---
 
### Injury and death

- [NCHS Multiple Cause of Death](https://www.nber.org/research/data/mortality-data-vital-statistics-nchs-multiple-cause-death-data) - Individual-level US mortality data
  - Years: 1959-present. Only years before 2005 have geographical information.
  - This version is cleaned by the NBER.
- [CDC Mortality Data](https://wonder.cdc.gov/deaths-by-underlying-cause.html) - County-level mortality data
  - Years: 1969-present. Requires agreement.
  - Depending on the year, splits by age, race, sex, and cause of death.
- [National Electronic Injury Surveillance System](https://www.cpsc.gov/Research--Statistics/NEISS-Injury-Data) - Individual-level data on injuries involving consumer products.
  - Sample paper: [Smartphones and child injuries](https://www.sciencedirect.com/science/article/pii/S0047272717301810)

---

### Crashes and traffic

- [Fatal Accident Reporting System (FARS)](https://www.nhtsa.gov/research-data/fatality-analysis-reporting-system-fars) - Individual-level data on virtually the universe of US fatal car crashes
  - Years: 1975-present. Includes drive and passenger demographics, car characteristics, location, and other circumstances regarding the crash.
- State-level crash data - some states (and cities) have individual-level, geocoded car crash data. A small number of examples:
  - [California](https://data.ca.gov/@california-highway-patrol/ccrs)
  - [Massachusetts](https://massdot-impact-crashes-vhb.opendata.arcgis.com/) and then search for "Crashes"
  - See also [this site](https://www.arcgis.com/home/item.html?id=3ef625ffe7ce4ef38be81ee6d80a5385#overview) and [this other site](https://sspf.tooledesign.com/crash_data_sources), which both detail data availability for each state. 
- [UTD19](https://utd19.ethz.ch/) - Traffic data from 20k+ stations across 40 cities
  - Years: 2017-2019. Access: public. 

---

### Education

- [IPEDS](https://nces.ed.gov/ipeds/) - Data on college enrollments, faculty/staff, expenditures, incoming test scores, graduation, etc.
- [SEDA](https://edopportunity.org/opportunity/data/downloads/) - K-12 district-, county-, and state-level test scores, by race and gender
  - Years: 2009-2019
- [Common Core of Data](https://nces.ed.gov/ccd/ccddata.asp) - K-12 school- and district-level data 
- You can access a lot of different datasets, such as IPEDS and CCD, using Urban Institute's [educationdata](https://educationdata.urban.org/documentation/), including R and Stata packages.
- [HERI](https://heri.ucla.edu/heri-data-archive/) - Detailed college freshman, senior, and faculty surveys
  - Years vary.  Some of data is publicly available; rest requires agreement.
- [Data on where colleges graduates go after graduating](https://www.openicpsr.org/openicpsr/project/170381/version/V3/view)
  - Years: 2010-2018. From [Grads on the Go: Measuring College-Specific Labor Markets for Graduates](https://onlinelibrary.wiley.com/doi/full/10.1002/pam.22553)
- [PISA](https://nces.ed.gov/surveys/pisa/datafiles.asp) - Data allowing cross-county comparisons on educational progress
- [Median earnings four years after graduation by university-major](https://www.theheagroup.com/blog/earnings-test-data)
  - Graduates from 2017-18 and 2018-19. Access: public. A university-major is only included if there are at least 16 graduates.
  - From the Department of Education; this version is made available by the HEA Group.
- [Post-Secondary Employment Outcomes (PSEO)](https://lehd.ces.census.gov/data/pseo_experimental.html) Earnings and employment outcomes for college and university graduates by degree level, degree major, post-secondary institution, and state of institution.
- [Educator Compensation Dashboard](https://www.sreb.org/educator-compensation-dashboard) - Southern state regional database of annual educator compensation and workforce data on K-12 education
  - Years: 2016 - present; Access: Public
  - This dashboard is compiled by scraping and pulling publicly available administrative data from state and national sources

<!-- [University enrollments](https://borealisdata.ca/dataset.xhtml?persistentId=doi:10.5683/SP3/P0D1KE&version=1.0) -->

---

### Academia

- [Openalex](https://openalex.org/) - over half a billion academic papers
  - Free to download the full data, but it is really big! Limited number of free API pulls per day
- [Metadata on NBER articles](https://www.nber.org/research/data/nber-working-papers-and-chapters-metadata) 
  - Includes information like authors, affiliations, and abstracts
- [Economics PhD Placements](https://www.econphdplacements.com/) - placements of 18k+ economics PhDs from 82 programs over 1990-2026
- [Economics Graduates North-America 1997-2017 with RePEc handles and Scopus IDs](https://dataverse.harvard.edu/dataset.xhtml?persistentId=doi:10.7910/DVN/ADSCLU)
- [Gender composition by academic field](https://edmond.mpg.de/dataset.xhtml?persistentId=doi:10.17617/3.BHU4FY)
  - Since 1950, based on estimated name from publications
- [PhD origins of academic faculty](https://larremorelab.github.io/us-faculty/) - where hundreds of thousands of professors got their PhDs, by university and field
   - From [Quantifying hierarchy and dynamics in US faculty hiring and retention](https://www.nature.com/articles/s41586-022-05222-x)
  
--- 

### Temperature

- [PRISM](https://prism.oregonstate.edu/) - Gridded weather data, including temperature and precipitation
  - Years: 1981-present (daily), 1895-present (monthly)
- [NOAA](https://www.ncdc.noaa.gov/cdo-web/datatools/findstation) - Weather station data
- [Open-Meteo](https://open-meteo.com/) - weather API
  - Some of data goes back to 1940. Forecast data from 2021. Free version of API is rate limited (300k/month)

---

### Family
*Births, Marriages, and Divorces*

- [NVSS Natality data](https://www.nber.org/research/data/vital-statistics-natality-birth-data) - Individual-level data on births
  - Years: 1968-present. Provided by NBER. Only years before 2005 have geographical information.
- [National Survey of Family Growth](https://www.cdc.gov/nchs/nsfg/index.htm) - Survey on things like pregnancy, infertility, births, and marriage
- [CDC and SSA Birthdates](https://github.com/fivethirtyeight/data/tree/master/births) - Counts of birth by calendar day
  - Years: 1994-2003 (CDC) and 2000-2014 (Social Security Administration)
  - From FiveThirtyEight. See [Some People Are Too Superstitious To Have A Baby On Friday The 13th](https://web.archive.org/web/20160516152410/http://fivethirtyeight.com/features/some-people-are-too-superstitious-to-have-a-baby-on-friday-the-13th/)
- [Marriages and Divorces in Texas](https://www.dshs.texas.gov/vital-statistics/marriage-divorce-records/marriage-divorce-indexes) - Individual-level data on marriages and divorces
   - Years vary. Some of the years are missing data.
   - Both files have names and dates. The divorce file has number of children and date of marriage.
- [Marriages in England and Wales](https://www.ons.gov.uk/peoplepopulationandcommunity/birthsdeathsandmarriages/marriagecohabitationandcivilpartnerships/datasets/marriagesinenglandandwales2013) - Counts of marriages by day
  - Years: 1999-present for the data with day of marriage. 

---
 
### Sports

- MLB
  - Pitch-level data from Baseball Savant's [Statcast](https://baseballsavant.mlb.com/statcast_search). You can get the location of the pitch, the distance a batted ball was estimated to travel, etc.
  - [Cot's salary data](https://legacy.baseballprospectus.com/compensation/cots/)
  - [Lahman Baseball Database](https://sabr.org/lahman-database/) - Season-level player statistics, 1871-present
  - [10,000 baseball scouting reports](https://github.com/jacobdanovitch/Trouble-With-The-Curve)
     - From [Trouble with the Curve: Predicting Future MLB Players Using Scouting Reports](https://arxiv.org/abs/1910.12622)
- NBA
  - [Box score data](https://www.kaggle.com/datasets/eoinamoore/historical-nba-data-and-player-box-scores), 1947-present, from Kaggle
  - [Play-by-play data](https://www.kaggle.com/datasets/szymonjwiak/nba-play-by-play-data-1997-2023), 1997-present, from Kaggle
- NFL
  - [nflverse](https://github.com/nflverse) - R package that you can use to get lots of data, including play-by-play
- Marathons
   - [Marathon times](https://www.kaggle.com/runningwithrock/datasets)

---

### Religion

- [2020 US Religion Census](https://www.usreligioncensus.org/node/1639) - Estimates of the number of adherents by faith at the county and state level
- [Pew's Religious Landscape Study (RLS)](https://www.icpsr.umich.edu/sites/icpsr/view/studies/221062/versions/V1) - large survey about religion
- [LDS Hymn Stats](https://hymnstats.joeystanley.com/overview.html) - the hymns sung at over 100,000 (non-representative) Latter-day Saint Sacrament Meetings
  - The microdata is not available, but counts by hymn are, overall and separately by before and since June 2024
- [The ARDA](https://thearda.com/data-archive/browse-categories) - compiles many datasets on religion
  
---

### Government
- [LocalView](https://www.localview.net/) - transcripts of local government meetings that were uploaded to YouTube
- [Voteview](https://voteview.com/) - how everyone in Congress has voted throughout all of US history as well as an ideology score for everyone
- [Visits by Foreign Leaders and Heads of State](https://github.com/HistoryAtState/visits) - Every visit of a foreign head of state to the US President (or VP if President was indisposed/abroad) from 1874-2020
- [CongressInData](https://www.congressindata.com/) - For Congress members between 2005-2015, it provides information on social networks, voting, etc.
- [Quality of Government Expert Survey](https://www.unesco.org/en/world-media-trends/qog-quality-government-data) - survey of around 1k experts on 117 countries about government quality
  - See also [here](https://www.gu.se/en/quality-government/qog-data/data-downloads) for other quality of government data

---

### Inflation and cost of living

- [CPI-U](https://fred.stlouisfed.org/series/CPIAUCNS#) - you can use this to adjust for inflation
  - To use, click on "Edit Graph" and adjust the frequency to "Annual" with "Average aggregation" method. 
- [Cost of living](https://www.commerce.gov/news/blog/2024/03/estimating-county-level-regional-price-parities-public-data) - County-level cost of living estimates

---

### Working

- CPS, ACS, PSID - see above
- [O*NET](https://www.onetcenter.org/database.html) - Data on occupational tasks
- [Quarterly Census of Employment and Wages (QCEW)](https://www.bls.gov/cew/downloadable-data-files.htm) - county-level data on employment and wages
- [Quarterly Workforce Indicators (QWI)](https://lehd.ces.census.gov/data/qwi_national.html) - employment, jobs creation, earnings and other measures of employment flows by detailed firm characteristics and worker demographics. Downloadable via [Census API](https://www.census.gov/data/developers/data-sets/qwi.html)
- [Job to Job Flows (J2J)](https://lehd.ces.census.gov/data/j2j_subsector_research.html) - statistics on job mobility in the United States, including the job-to-job transition rate, hires and separation rates, earnings changes due to job change, and characteristics of the origin and destination job.
- [LEHD Origin-Destination Employment Statistics (LODES)](https://lehd.ces.census.gov/data/) - source data for the Census [OnTheMap](https://onthemap.ces.census.gov/) data tool, providing statistics at the Census block level at both residential and workplace locations and flows between the two (origin-destination).
- [Veteran Employment Outcomes (VEO)](https://lehd.ces.census.gov/data/veo_experimental.html) - labor market outcomes for discharged veterans from five branches of the military - Air Force, Army, Coast Guard, Marine Corps, and Navy. Tabulated by military specialization, service characteristics, employer industry, and veteran demographics.
- [Mobility, Opportunity, and Volatility Statistics (MOVS)](https://www.census.gov/programs-surveys/ces/data/public-use-data/mobility-opportunity-volatility-statistics.html) a dataset that tracts the income changes of a 2005 cohort of U.S. adults from 2005 to 2019 by initial income decile, sex, and race/ethnicity. 

<!-- - [Anthropic Economic Index](https://huggingface.co/datasets/Anthropic/EconomicIndex) - Actual AI exposure by job and by geography
- [AI Job Exposure Index](https://github.com/openai/GPTs-are-GPTs) - [from Eloundout et. al](https://www.science.org/doi/10.1126/science.adj0998). Predicted exposure -->
- [US healthcare job postings and posted pay (CareJobs.Now)](https://doi.org/10.5281/zenodo.23395728) - Open dataset of US healthcare job postings and the hourly pay employers post, by kind of job

---
### Businesses
- [County Business Patterns](https://www.census.gov/programs-surveys/cbp/data.html) - county-level data on employment and payroll
- [Chicago Business Registrations](https://data.cityofchicago.org/Community-Economic-Development/Business-Licenses-Current-Active/uupf-x98q/about_data) - geocoded business licenses with business name, date of expiration, etc.
- [Business Dynamic Statistics](https://www.census.gov/programs-surveys/bds.html) - Annual measures of business dynamics - job creation and destruction, establishment births and deaths, firm startups and shutdowns by establishment and firm characteristics. Also available for specific types of firms/measures: [Patenting Firms](https://www.census.gov/data/experimental-data-products/bds-patenting-firms.html), [High Growth Firms](https://www.census.gov/data/experimental-data-products/bds-high-growth.html), [Goods Traders](https://www.census.gov/data/experimental-data-products/bds-goods-traders.html), [High Tech Industries](https://www.census.gov/data/experimental-data-products/bds-high-tech.html), [Single-Unit Firms with Revenue](https://www.census.gov/data/experimental-data-products/bds-single-unit.html), [Human Capital](https://www.census.gov/data/experimental-data-products/bds-human-capital.html), [Coastal Counties](https://www.census.gov/data/experimental-data-products/bds-coastal-counties.html).
- [Dispersion Statistics on Productivity (DiSP)](https://www.census.gov/data/experimental-data-products/dispersion-statistics-on-productivity.html) - within-industry measures of productivity dispersion. Covers every five years from 1987-2017 by 4-digit NAICS for manufacturing and retail sectors.
- [Business Trends and Outlook Survey (BTOS)](https://www.census.gov/data/experimental-data-products/business-trends-and-outlook-survey.html) high-frequency, nationally representative data on U.S. employer businesses. Collected starting September 11, 2023. Data released every 2 weeks by NAICS sector, state, and 25 most populous MSAs.

---

### Politics and voting
- [Small-Area Global Elections (SAGE) Dataset](https://noahdasanaike.github.io/sage.html) - Granular, geocoded voting returns for 134 countries
- [MIT Election Lab](https://electionlab.mit.edu/data) - Collection of various US election results
- [NYT's Presidential precinct data for the 2024 U.S. general election](https://github.com/nytimes/presidential-precinct-map-2024)
   - See also this [map](https://www.nytimes.com/interactive/2025/us/elections/2024-election-map-precinct-results.html)
- [North Carolina voter registration data](https://www.ncsbe.gov/results-data/voter-registration-data)

---

### Health, public health, and epidemiology

- [National Health and Nutrition Examination Survey (NHANES)](https://www.cdc.gov/nchs/nhanes/index.html) - National survey for adults and children with various health-related questions
- [National Health Interview Survey](https://nhis.ipums.org/nhis/)
- [Medical Expenditure Panel Survey](https://meps.ipums.org/meps/)
- [Global Health Surveys](https://globalhealth.ipums.org/)
- [National Immunization Survey](https://www.cdc.gov/nis/about/index.html)
- [National Survey of Children's Health](https://www.census.gov/programs-surveys/nsch.html)
- [Behavioral Risk Factor Surveillance System](https://www.cdc.gov/brfss/index.html)
- [Health and Retirement Survey](https://hrs.isr.umich.edu/)
- [Youth Risk Behavioral Surveillance System](https://www.cdc.gov/yrbs/index.html)
- [National Health and Aging Trends Study (NHATS)](https://www.nhats.org/nhats)
- [Global Survey of School Meal Programs](https://gcnf.org/survey-data/) - school meals survey across many countries
   - Years: 2019-present; Access: Public
   - Geography: Global (167 countries); Units of observation: Country and school meal program; Frequency: Every 2-3 years; Implementer: Global Child Nutrition Foundation
   - See [A comprehensive and standardized dataset on school feeding activities worldwide: The Global Survey of School Meal Programs](https://doi.org/10.1016/j.dib.2026.113018) 

---

### Real estate

- [Prices paid dataset](https://www.gov.uk/government/statistical-data-sets/price-paid-data-downloads) - All residential property sales in England and Wales (that are sold for value and registered)
  - Years: 2018-present. Has address and price paid.
- [Tract-level home price indices](https://www.fhfa.gov/PolicyProgramsResearch/Research/Pages/wp2101.aspx)
  - Years: 1989-2021
  - From [A Flexible Method of House Price Index Construction using Repeat-Sales Aggregates](https://onlinelibrary.wiley.com/doi/full/10.1111/1540-6229.12474)
 
---

### Patents

- [Worldwide patent data](https://dataverse.harvard.edu/dataset.xhtml?persistentId=doi:10.7910/DVN/OTTBDX) - Geocoded, 1980-2014, 46 countries
  - From [Geocoding of Worldwide Patent Data](https://www.nature.com/articles/s41597-019-0264-6)
- [US patent data](https://data.uspto.gov/home)

---

### Social networks

- [Facebook Social Connectedness Index (SCI)](https://ai.meta.com/ai-for-good/datasets/social-connectedness-index/) - county-to-county connectedness
  - Based on Facebook friendships. Also country-to-country and other subnational links.

---

### Beliefs and values
- [World Values Survey](https://www.worldvaluessurvey.org/WVSContents.jsp) - Worldwide survey on beliefs and values
- [European Social Survey](https://www.europeansocialsurvey.org/) - European survey on attitudes, values, etc.

---

### Law

- [A list of all federal laws](https://osf.io/qa289) 
 - From [A comprehensive dataset of U.S. federal laws (1789–2022)](https://www.nature.com/articles/s41597-023-02758-z)
- [LawAtlas](https://lawatlas.org/) - Coded laws from Temple University's Public Health Law Review 

---

### Environment and energy

- [ERCOT](http://ercot.com/gridinfo/load/load_hist/index.html) - hourly electricity load data in Texas
  - 1995-present. ERCOT is the largest provider in the state
- [Gridded Environmental Impacts Frame (Gridded EIF)](https://www.census.gov/data/experimental-data-products/gridded-eif.html) - detailed demographic counts by age, sex, race and ethnicity and data for environmental hazards on a 0.01 degree grid of the United States. 

---

### Shopping

- [1.8 million Amazon purchases from 5000 people](https://github.com/aberke/amazon-study/tree/master/data)
  - From [Open e-commerce 1.0, five years of crowdsourced U.S. Amazon purchase histories with user demographics](https://www.nature.com/articles/s41597-024-03329-6)

---

### Maps and geography
- [Historical Topographic Maps](https://www.usgs.gov/programs/national-geospatial-program/historical-topographic-maps-preserving-past)
  - Maps from 1884-2006
- [Elevation data](https://cran.r-project.org/web/packages/elevatr/index.html) - R package to get elevation data from a variety of sources

<!--Rivers
Lidar
-->

---

### States, conflict, and regimes

- [Interstate System Dataset (ISD), version 2.1](https://doi.org/10.7910/DVN/GFF9WN) - All independent states since 1816, a wider list than the Correlates of War one
  - Years: 1816-2016; Access: Public (CC0)
  - One row per state, with entry and exit dates and how the state ended (conquest, unification, dissolution, etc.)
- [Abramson (2017) replication data](https://doi.org/10.7910/DVN/9XBBHZ) - European states from 1100 to 1790, with their territory and when they ended
  - Years: 1100-1790; Access: Public (CC0)
  - From [The Economic Origins of the Territorial State](https://doi.org/10.1017/S0020818316000308)
- [Political Instability Task Force (PITF) State Failure Problem Set](https://www.systemicpeace.org/inscrdata.html) - Onsets and ends of ethnic wars, revolutionary wars, adverse regime changes and genocides
  - Years: 1955-2018; Access: Free download, cite the source, no redistribution without permission
- [Polity5](https://www.systemicpeace.org/inscrdata.html) - Regime scores for independent states with more than 500,000 people
  - Years: 1800-2018; Access: Free download
- [V-Dem](https://www.v-dem.net/data/the-v-dem-dataset/) - Hundreds of indicators of democracy and regime characteristics, by country and year
  - Years: 1789-present; Access: Public
- [CShapes 2.0](https://icr.ethz.ch/data/cshapes/) - Borders and capitals of states and dependent territories, as maps
  - Years: 1886-2019 (Europe from 1816); Access: Public (CC BY-NC-SA 4.0)
 
---

### Macroeconomics

- [World Macro-Financial Dataset](https://acamous.github.io/macro_financial_dataset/) - Data for many countries on credit, GDP, equity prices, bond yields and consumer prices
  - Years: 1950-2025; 49 countries; Frequency: quarterly
  - From [World Cycles Revisited: Diverging Trends in Prices and Quantities](https://www.banque-france.fr/en/publications-and-statistics/publications/world-cycles-revisited-diverging-trends-prices-and-quantities)

---

Disclaimer: This site may contain errors and in no way do we guarantee the accuracy or quality of the referenced data. In no event will we be liable for any loss or damage.

<!-- 
<details>
<summary>Details</summary>

- Test A
- Test B

</details> 

### Music

### Media and Text
Dataset with about 400 million semantic pairs from newspapers [Link ](https://huggingface.co/datasets/dell-research-harvard/headlines-semantic-similarity) 
Stanford’s Cable TV News Analyzer https://tvnews.stanford.edu/data
https://x.com/MelissaLDell/status/1806760404389179483 https://arxiv.org/abs/2406.09490 Newswire 
[Transcripts of 2 million YouTube videos (billions of words)](https://huggingface.co/datasets/PleIAs/YouTube-Commons)

-->


