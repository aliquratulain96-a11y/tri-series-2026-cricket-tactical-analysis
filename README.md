# tri-series-2026-cricket-tactical-analysis
Python-based tactical analysis of the 2026 Pakistan–England–Sri Lanka ODI Tri-Series using ball-by-ball data.
# Tri-Series 2026: Tactical Cricket Analytics

A ball-by-ball investigation of scoring patterns, innings progression and team performance in the Pakistan–England–Sri Lanka ODI Tri-Series.

## 1. Project Overview

This project examines the 2026 Pakistan–England–Sri Lanka ODI Tri-Series through delivery-level cricket data. Using Python, I analysed scoring patterns, innings phases, wicket-loss rates and scoring progression across seven matches.

Rather than focusing only on final match results, the project investigates how teams approached different stages of an innings and how their scoring patterns varied throughout the tournament.

## 2. Research Questions

The analysis was guided by five questions:

1. How did Pakistan, England and Sri Lanka differ in their scoring rates across the Powerplay, middle and death overs?
2. Which team recorded the highest average innings score?
3. How did wicket-loss rates vary across the three innings phases?
4. How did scoring rates change across successive overs, and what patterns emerged between teams?
5. How did scoring progression differ between the two innings across the seven matches?

## 3. Tournament Coverage

| Detail | Coverage |
|---|---|
| Tournament | Pakistan–England–Sri Lanka ODI Tri-Series 2026 |
| Teams | Pakistan, England, Sri Lanka |
| Matches | 7 ODIs |
| Dates | 18–31 October 2026 |
| Venues | Rawalpindi Cricket Stadium; Gaddafi Stadium, Lahore |

## 4. Data and Tools

Data source: Cricsheet ball-by-ball JSON files.

The seven relevant match files were processed into a structured delivery-level dataset.

Tools used:
- Python
- Pandas
- NumPy
- Matplotlib
- Google Colab

## 5. Analytical Methodology

### Innings phase analysis

Each innings was divided into three phases:

- Powerplay: Overs 1–10
- Middle overs: Overs 11–40
- Death overs: Overs 41–50

Scoring rate was calculated as:

`Total runs / Legal balls × 6`

### Average innings score

Innings totals were grouped by team and averaged across the available matches.

### Wicket-loss rate

To account for differences in phase duration, wicket loss was standardized as wickets lost per 10 legal overs:

`Wickets lost / Legal balls × 60`

### Over-by-over scoring profile

Scoring rates were aggregated by over number across available innings. This provides a tournament-level comparison rather than a single-match trajectory.

### Run-rate progression

Cumulative runs from both innings were plotted across all seven matches to compare innings progression and changes in scoring patterns.

## 6. Visualisations

### 6.1 Tournament Tactical Dashboard

This dashboard brings together four dimensions of tournament analysis: phase-based scoring rates, average innings scores, normalized wicket-loss rates and over-by-over scoring profiles.

![Tournament Tactical Dashboard](visuals/tactical_dashboard.png)

### 6.2 Seven-Match Run-Rate Worms

These charts compare cumulative scoring progression between the two innings in each match. They provide a match-level view of how innings developed over time.

![Seven-Match Run-Rate Worms](visuals/seven_match_worms.png)

## 7. Findings and Interpretation

The dashboard identifies several differences in team scoring patterns:

England: Recorded the highest average innings score (318) and the strongest Powerplay (5.93) and death-over (10.88) scoring rates.
  Sri Lanka: Recorded the highest middle-over scoring rate (7.17).
  Pakistan: Increased its scoring rate from 4.98 in the Powerplay to 8.31 in the death overs.
  Wicket-loss patterns: Varied across teams and phases. Sri Lanka's death-over wicket-loss rate was particularly high, although this should be interpreted in light of the number of deliveries available in that phase.

These findings describe observed scoring patterns. They do not, on their own, establish why a team performed in a particular way.

## 8. Limitations

- The over-by-over scoring profile pools innings, so later overs may have fewer observations.
- Wicket-loss rates are normalized by legal balls faced, but phase-level sample sizes still differ.
- The dataset does not contain shot-location coordinates; therefore, genuine pitch maps and wagon wheels could not be produced.
- This project is descriptive and does not claim to predict match outcomes.

## 9. Future Development

Possible extensions include:

- Batter and bowler performance analysis.
- Partnership analysis.
- Boundary and dot-ball distribution.
- Phase-specific bowling effectiveness.
- Predictive modelling of innings outcomes.

## 10. Data Source

Cricsheet: https://cricsheet.org/

Only the seven relevant match files were used for this project.

## Author
Qurat Ul Ain Ali
Qurat Ul Ain Ali

Cricket Analytics | Python | Data Visualisation
