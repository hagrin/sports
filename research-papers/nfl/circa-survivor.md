# Circa Survivor Projection Model

Objective: Try to more accurately predict Circa Survivor contestant selections which have proven to be difficult to accurately project versus public resources such as SurvivorGrid.

## Theory

The following is a list of items I need to consider when building a selection projection model -
- Remaining pool size
- What week we are in (early weeks vs late weeks)
- "Candidate Selections" - much like in chess where you evaluate candidate moves, identify candidate selections and depth of candidate selections in a particular week and the depth's relationship to distribution
- Market price of the candidate selections
- Future value of the candidate selections
- SurvivorGrid EV and Pick% data - using the assumption that people are using this as a shortcut and then taking this data and modifying their selections based on the game theory

## Data Required

Following data is required - 
- Historical Circa pick selections
- Where possible more accurate entry selection data to better estimate available candidate selections
- Historical SurvivorGrid data
- Accurate market pricing history
- Injury data - not necessary, but there's a theory that a questionable / hurt starting QB that's projected as playing may offer some additional EV if you can accurately project injury news breaking your way after selections lock

## Pseudocode
