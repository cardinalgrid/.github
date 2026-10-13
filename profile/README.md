# Cardinal Grid

**Open methods for load forecasting and grid data quality.**

I am a load forecasting engineer. My day job is at a national system operator, where I help produce the load forecasts that feed the grid's electrical and energy studies. Cardinal Grid is what I do with that experience on public data: measure how well U.S. balancing authorities forecast their own load, build open tools for the data problems that make those forecasts fail, and write up what I find so that anyone can check it.

The starting point is simple. Since 2015, every balancing authority in the contiguous U.S. has reported to EIA, hour by hour, both the demand that occurred and the day-ahead forecast it produced the day before. FERC and NERC have documented what happens when that forecast is wrong: reserves fall short and load is shed ([FERC/NERC 2023](https://www.ferc.gov/news-events/news/ferc-nerc-release-final-report-lessons-winter-storm-elliott), [FERC 2024](https://www.ferc.gov/news-events/news/presentation-system-performance-review-january-2024-arctic-storms)), and NERC now says traditional forecasting may not keep up with the load growth ahead ([NERC 2026](https://www.nerc.com/globalassets/our-work/assessments/nerc_ltra_2025.pdf)). Nobody had been scoring those forecasts continuously and in the open. Now somebody is.

## Projects

| Repository | What it is | Status |
|---|---|---|
| [`ba-forecast-scorecard`](https://github.com/cardinalgrid/ba-forecast-scorecard) | Daily scoring of every U.S. balancing authority's own day-ahead load forecast from EIA-930 public data, 2015 to today: error by BA, season and named event, with explicit data-quality rules. | Live, updated daily. [DOI 10.5281/zenodo.22697386](https://doi.org/10.5281/zenodo.22697386) |
| [`grid-data-sentinel`](https://github.com/cardinalgrid/grid-data-sentinel) | Python package for detecting and correcting anomalies in load telemetry while keeping the genuine extremes, with an audit trail, in batch or streaming. Based on the methods from my M.Sc. thesis and my 2024 paper. | v0.4.0. [DOI 10.5281/zenodo.22726013](https://doi.org/10.5281/zenodo.22726013) (all versions) |
| [`ba-load-forecast`](https://github.com/cardinalgrid/ba-load-forecast) | An open day-ahead load forecaster built only from public data (EIA-930 demand, NOAA HRRR, NBM and GFS weather forecasts), run unchanged on 43 balancing authorities and scored against each one's own forecast, with every rule and every rejected test documented. | v1.0.0. [DOI 10.5281/zenodo.23327586](https://doi.org/10.5281/zenodo.23327586) |
| [`notes`](https://github.com/cardinalgrid/notes) | Short, reproducible technical notes on U.S. forecasting and data-quality problems, each with its code and a DOI. Plain-language versions at [cardinalgrid.com/notes](https://cardinalgrid.com/notes). | Four notes published |

## How I work

Public data only, always. Every chart comes with the script that made it. Results are reported with their limitations, including when a method loses to a baseline. Releases and notes carry DOIs so a number quoted today can be checked years from now. Code is Apache-2.0; text and figures are CC BY 4.0.

## About me

Ricardo W. C. Guerra Filho. Electrical engineer (CREA/PB), M.Sc. in Optimization of Energy Systems (Universidade Federal da Paraíba, 2023; thesis on outlier detection in energy demand curves). I have worked on electricity demand forecasting since 2015, in university research, at a distribution utility and now at the national system operator. Author of [*Outlier Detection and Correction in Smart Grid Energy Demand Data Using Sparse Autoencoders*, Energies 2024](https://www.mdpi.com/1996-1073/17/24/6403). The analyses here are my own and are not those of any employer.

[cardinalgrid.com](https://cardinalgrid.com) · [ORCID 0000-0001-6699-9951](https://orcid.org/0000-0001-6699-9951) · ricardo.guerra@cardinalgrid.com · project inbox: contact@cardinalgrid.com
