# UW–Madison Data Challenge: U.S. Trade Analysis

This repository contains our submission for the **UW–Madison Data Challenge**, where we analyzed U.S. trade patterns with partner countries to understand what drives differences in export volumes across countries and over time.

## Project Overview

Our goal was to answer two core questions:
1. How do U.S. trade volumes differ across regions and countries?
2. What country-specific factors explain changes in U.S. exports over time?

To address these questions, we constructed a **country × commodity × year panel dataset** using U.S. trade data combined with country-level economic and political indicators.

## Methods

We used a combination of:
- Exploratory visualizations of trade trends across major partner countries
- Hypothesis testing to assess within-region heterogeneity
- Panel data models, including:
  - **Country fixed-effects models** (to study within-country changes over time)
  - **Random-effects / gravity-style models** (to incorporate time-invariant factors like distance)

Model selection was guided by a **Hausman test**, which indicated fixed effects as the primary specification for inference.

## Key Findings

- **Market size matters**: Countries with growing populations tend to import more from the U.S., leading to higher U.S. export volumes.
- **Distance remains a major friction**: Even after controlling for market size and product categories, greater distance from the U.S. is strongly associated with lower trade volumes.
- **Political stability plays a secondary role**: Stability appears significant in simpler models but weakens once market size and distance are accounted for, suggesting its effects operate indirectly.
- **Regional averages mask variation**: Countries within the same region often differ substantially in trade intensity, highlighting the importance of country-specific analysis.

Overall, our results are consistent with a **gravity model of trade**, where scale and geography dominate U.S. export patterns.
