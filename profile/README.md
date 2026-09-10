# Cardinal Grid

**Open methods for load forecasting and grid data quality.**

Cardinal Grid is an independent, open initiative that publishes reproducible benchmarks, tools and technical notes on load forecasting and telemetry data quality for the U.S. bulk power system. Everything here is built from public data, with code anyone can run.

Federal reliability authorities have documented that day-ahead forecast error and bad telemetry contributed to load shed in recent extreme-weather events, and that the load growth now projected makes both problems harder ([FERC/NERC 2023](https://www.ferc.gov/news-events/news/ferc-nerc-release-final-report-lessons-winter-storm-elliott), [FERC 2024](https://www.ferc.gov/news-events/news/presentation-system-performance-review-january-2024-arctic-storms), [NERC 2025 LTRA](https://www.nerc.com/globalassets/our-work/assessments/nerc_ltra_2025.pdf)). This initiative works on two links of that chain: the forecast, and the data the forecast depends on.

## Projects

| Repository | What it is | Status |
|---|---|---|
| [`ba-forecast-scorecard`](https://github.com/cardinalgrid/ba-forecast-scorecard) | Daily scoring of every U.S. balancing authority's own day-ahead load forecast, from EIA-930 public data. Error by BA, season, extreme-weather day and named event. | Launching October 2026 |
| [`grid-data-sentinel`](https://github.com/cardinalgrid/grid-data-sentinel) | Python package for detecting and correcting anomalies in load telemetry while preserving genuine extremes, with an audit trail. Recursive TEDA and sparse autoencoders. | v0.1 October 2026 |
| [`notes`](https://github.com/cardinalgrid/notes) | Short, reproducible technical notes on U.S. forecasting and data-quality problems. Each note ships with its notebook and a DOI. | First note October 2026 |

## Principles

- **Public data only.** EIA-930, ISO/RTO archives, NOAA. No proprietary or employer data, ever.
- **Reproducible.** Every chart ships with the notebook that produced it and a pinned data snapshot.
- **Honest about limits.** Results are reported with their limitations, including when a method underperforms a baseline.
- **Versioned and citable.** Releases, reports and notes carry DOIs (Zenodo); corrections are logged, not overwritten.

## Licenses

Code: Apache-2.0. Notes and reports: CC BY 4.0.

## Maintainer

Ricardo W. C. Guerra Filho, electrical engineer (CREA/PB), M.Sc. in Optimization of Energy Systems, load forecasting engineer at Brazil's national system operator. Author of [*Outlier Detection and Correction in Smart Grid Energy Demand Data Using Sparse Autoencoders*, Energies 2024, 17(24), 6403](https://www.mdpi.com/1996-1073/17/24/6403). The analyses here are his own and rely on public data only.

Website: [cardinalgrid.com](https://cardinalgrid.com) · ORCID: [0000-0001-6699-9951](https://orcid.org/0000-0001-6699-9951) · Contact: contact@cardinalgrid.com
