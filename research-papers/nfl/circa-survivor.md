# Circa Survivor Projection Model

Objective: Try to more accurately predict Circa Survivor contestant selections which have proven to be difficult to accurately project versus public resources such as SurvivorGrid.

## Theory

The following is a list of items I need to consider when building a selection projection model -
- Remaining pool size
- What week we are in (early weeks vs late weeks)
- Accurate %s of what entries still have what teams available
- "Candidate Selections" - much like in chess where you evaluate candidate moves, identify candidate selections and depth of candidate selections in a particular week and the depth's relationship to distribution
- Market price of the candidate selections
- Future value of the candidate selections
- SurvivorGrid EV and Pick% data - using the assumption that people are using this as a shortcut and then taking this data and modifying their selections based on the game theory
- Actual Elimination% vs Projected Elimination% - the theory behind this is that there's some correlation between actual elimination % vs the projected elimination % of public model pick %s. The greater the divergence between actual vs projected should mean how closely or divergent the remaining contestants are to the public pick %s. This item seems especially relevant in years where the actual elimination% far exceeds the projected elimination% (ex: 2024) where the remaining contestents were extremelly contrarian as a group to public pick %s

## Data Required

Following data is required - 
- Historical Circa pick selections
- Where possible more accurate entry selection data to better estimate available candidate selections
- Historical SurvivorGrid data
- Accurate market pricing history
- Injury data - not necessary, but there's a theory that a questionable / hurt starting QB that's projected as playing may offer some additional EV if you can accurately project injury news breaking your way after selections lock

### Limitaions of the Data

There are some limitations on the data that, for better fits / accuracy, need to be accounted for specifically. First, SurvivorGrid data will update basically until the latest lock time for the 3 sets of contests they scrape - Yahoo, ESPN and OFP (OfficeFootballPool). However, Circa Survivor entries are due (in most cases) the day earlier at 4PM PST. Therefore, if there is late line movement or injury news, it's possible SurvivorGrid data will diverge from Circa pick selection data due to the later deadline and ability to process late breaking information.

## Pseudocode
