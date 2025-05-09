# Total Fertility Rates Data Exploration

This project explores demographic data related to fertility, with a particular focus on how male occupation correlates with the number of children in the household.

The initial analysis uses IPUMS microdata to compute average values of `NCHILD` (number of biological children living with the respondent) for each male occupation code (`OCC2010`). Results are presented both weighted by `PERWT` (IPUMS population weights) and unweighted.

## Current Analysis
- Aggregates fertility outcomes by male occupation
- Uses IPUMS ACS 5-year microdata from the following periods:
  - 2009–2013
  - 2014–2018
  - 2019–2023
- Primary variables used:
  - `NCHILD`: number of biological children living in the household
  - `OCC2010`: occupation codes
  - `PERWT`: person-level population weights
- Compares weighted vs. unweighted fertility estimates
  
## TODO
- Re-run analysis using less granular occupation groupings (e.g., 2-digit or sector-level codes)
- Analyze fertility patterns by marital status (e.g., married vs. divorced fathers)
- Analyze geographic variation in fertility by state (`STATEFIP`)
- Explore seasonal birth patterns by mother's birth quarter (`BIRTHQTR`)  
  *(Birth month data is unavailable in ACS/IPUMS)*
- Clean and standardize occupation label mappings (`OCC2010`) for better display and analysis


## Future Work
I plan to explore broader social and policy factors potentially affecting fertility, including:
- The impact of multi-family housing prevalence on family formation
- The effects of increased smartphone use (particularly among Gen Z) on adolescent mental health and downstream fertility rates
