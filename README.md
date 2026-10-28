# GPU Cloud Pricing and Workload Economics

**Independent undergraduate research project | Data Science & AI | 2026**

**Status:** In progress — research design and data collection  
**Focus:** GPU-as-a-Service (GPUaaS), cloud pricing, AI workload costs, and the Indian AI infrastructure market

## Overview

GPUs are essential for many modern AI applications, but accessing them through the cloud can be expensive. While several providers publish GPU rental rates, comparing their offerings is not as simple as choosing the lowest hourly price. Hardware specifications, included resources, location, billing terms, and the type of AI workload can all affect the actual cost.

I'm a second-year B.S. Data Science and Artificial Intelligence student at IIM Sambalpur. I started this independent project to better understand **how GPU cloud services are priced and how those prices translate into costs for people building or running AI systems**.

The project begins with a small, source-verified pricing dataset and will gradually expand into comparative analysis and workload-based cost estimates. I'm particularly interested in what these findings could mean for researchers, startups, and GPU cloud providers in India.

## Research question

> How do GPU cloud prices differ across providers, and how useful is the advertised price per GPU-hour for comparing the cost of AI workloads?

I plan to investigate:

1. How prices vary for comparable GPU configurations across selected providers.
2. How region, memory, bundled resources, and billing terms affect the comparison.
3. How workload requirements might change which GPU cloud option is more economical.

This is an **exploratory undergraduate research project**. The questions and methods may be refined as I collect data and review relevant literature.

## Research approach

### 1. Understand the provider landscape

I will study different types of cloud GPU providers, including hyperscalers, specialist GPU cloud companies, and Indian providers. Initial candidates include AWS, Google Cloud, Lambda, CoreWeave, Yotta, and E2E Networks.

The final comparison will depend on which providers have **publicly verifiable prices and sufficiently comparable configurations**. I will document omissions rather than fill gaps with estimates presented as facts.

### 2. Build a documented pricing dataset

For each public quote I use, I plan to record:

- Provider, GPU model and number of GPUs
- Region, CPU/RAM and other included resources (when available)
- Original price, currency, billing unit and pricing model
- Date collected, source URL, and relevant restrictions or exclusions

A first comparison metric will be:

```text
Price per GPU-hour = Instance hourly price / Number of GPUs
```

This is useful for describing list prices, **not a complete measure of performance or value**. I will avoid treating different GPU generations, spot versus on-demand rates, or different contractual terms as directly equivalent.

### 3. Analyse prices with Python

Using pandas and Jupyter Notebook, I plan to clean and inspect the pricing observations, calculate normalised rates, and build simple charts. The initial objective is a reproducible comparison of a small number of providers and GPU configurations—not a comprehensive ranking of the market.

### 4. Explore AI workload economics

After completing the initial dataset, I hope to estimate costs for a few clearly defined AI training or inference scenarios. If I can obtain suitable GPU access or comparable benchmark data, I may extend the analysis to measures such as inference throughput and cost per unit of output.

**Assumption-based estimates, third-party benchmarks, and experiments I run myself will be labelled separately.**

## Planned repository contents

These are **planned folders**, not completed outputs:

```text
.
├── README.md
├── data/           # Public pricing observations and data dictionary
├── sources/        # Source log and collection dates
├── notebooks/      # Data cleaning, exploration and visualisations
└── reports/        # Research notes, methodology and findings
```

As the project develops, I aim to publish:

- A source-verified GPU pricing dataset
- A reproducible Python notebook comparing selected offerings
- A few charts explaining the main differences
- A short write-up of observations, assumptions, and limitations
- An optional workload cost model, if the data support one

## Current progress and next milestone

**Current stage:** The research question and initial methodology have been defined. No completed pricing study or benchmark results are claimed yet.

**Next milestone:** Collect a first batch of dated public pricing observations, preferably for the same GPU model across multiple providers, and record any differences in region, billing terms or bundled resources. Then publish a documented dataset and the first cleaning/analysis notebook.

## Research practices

- Link every pricing observation to its original source and collection date.
- Preserve original currencies; document any exchange-rate conversions.
- Separate on-demand, spot, and committed pricing.
- Clearly state assumptions and avoid unsupported performance comparisons.
- Report missing data and limitations alongside findings.
- Update conclusions when new evidence becomes available.

## Why I'm doing this

I want to connect what I'm learning in Python, data analysis and AI with a practical question about the infrastructure behind AI systems. Working through the data myself is also a way to learn how to frame a research question, check sources, build reproducible analyses and explain results responsibly.

I hope this project will give me a useful foundation for future research or industry work related to AI infrastructure and cloud computing.

---

**Karthik Srivatsan**  
B.S. Data Science & Artificial Intelligence  
IIM Sambalpur

*Independent student project. This repository is not affiliated with the cloud providers mentioned above.*
