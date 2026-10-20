# GPU Cloud Pricing & Market Research

**An independent research project examining the pricing, cost structure, and commercial economics of GPU cloud infrastructure for AI workloads.**

**Status:** Research in progress | **Focus:** AI infrastructure · Cloud economics · Pricing analysis · GPU utilisation · Indian GPU cloud market

## Overview

The rapid growth of AI training and inference has increased demand for accelerated computing. However, GPU rental prices vary widely between cloud platforms, and the advertised hourly rate does not tell the full story about the cost of running an AI workload or the economics of operating GPU infrastructure.

This project investigates **how GPU cloud compute is priced, why comparable offerings can have different costs, and how workload characteristics and capacity utilisation influence economic outcomes**. It combines technical analysis of GPU systems with market research, data analysis, and illustrative infrastructure financial modelling.

### Core research question

> How do GPU cloud providers price compute, what explains differences between offerings, and how do workload costs and GPU utilisation affect commercial returns?

## Research objectives

1. **Map the GPU cloud market:** Understand the roles of hyperscalers, specialised GPU cloud providers, and emerging Indian infrastructure companies.
2. **Compare GPU offerings:** Study accelerator types, GPU counts, VRAM, CPU/RAM bundles, networking, regions, availability, and pricing terms.
3. **Build a traceable pricing dataset:** Record dated, publicly verifiable vendor quotes and their conditions.
4. **Normalise pricing:** Compare GPU-hour costs under appropriately matched hardware, regions, billing models, and commitments.
5. **Model workload costs:** Estimate the cost of representative model-training, steady-state inference, and intermittent enterprise workloads.
6. **Explore infrastructure economics:** Examine the effects of GPU utilisation, capital investment, operating costs, electricity, cooling, and power usage effectiveness (PUE).
7. **Study India-specific opportunities:** Evaluate the Indian GPU cloud landscape and potential customer segments, distinguishing announced capacity from operational offerings.

## Research scope

### Providers under consideration

The intended comparison includes at least five providers spanning different segments:

| Segment | Candidate providers |
| --- | --- |
| Hyperscale cloud | Amazon Web Services (AWS), Google Cloud |
| Specialised GPU cloud | CoreWeave, Lambda |
| India-focused GPU cloud | Yotta / Shakti Cloud, E2E Networks |

The final sample will depend on the availability of verifiable, sufficiently comparable public pricing. Reliance/Jio's AI infrastructure initiatives may be included in the **India market landscape**, but not in the quantitative pricing dataset without a dated, verifiable GPU rental offer.

### Factors being studied

- **Compute hardware:** GPU architecture/model, VRAM, memory bandwidth, accelerator count, and interconnects.
- **Cloud configuration:** CPU, RAM, storage, networking, region, and deployment constraints.
- **Commercial terms:** On-demand, spot/preemptible, reserved/committed pricing, minimum rental periods, and billing granularity.
- **AI workloads:** Training versus inference, job duration, throughput, latency, and scaling requirements.
- **Infrastructure operations:** Billable utilisation, electricity costs, cooling, PUE, capacity planning, and capital/operating expenditure.

## Methodology

### 1. Source and document pricing data

Collect publicly available provider specifications and pricing observations. Each observation will retain its **source URL, collection date, original currency, region, hardware details, billing model, and applicable caveats**.

Planned dataset fields include:

`provider`, `region`, `checked_at`, `gpu_model`, `gpu_count`, `vram_gb`, `cpu_count`, `system_ram_gb`, `network`, `instance_rate`, `currency`, `gpu_hour_rate`, `billing_model`, `term`, `source_url`, and `caveats`.

### 2. Build a like-for-like pricing comparison

A basic normalisation is:

```text
Price per GPU-hour = Hourly instance price / Number of GPUs
```

This metric is a **starting point, not a complete price/performance benchmark**. Comparisons will account for GPU model, region, bundled resources, contract conditions, data transfer/storage charges, and any relevant currency-conversion assumptions. Spot and on-demand quotes will be analysed separately.

### 3. Estimate costs for representative workloads

Develop assumption-driven scenarios for:

- **Training:** A time-limited multi-GPU training or fine-tuning job.
- **Steady inference:** An inference service with regular, sustained demand.
- **Intermittent usage:** An enterprise or research workload with irregular compute requirements.

Each scenario will consider the relationship between rental rates, runtime, GPU count, workload utilisation, and other billable resources. Where reliable throughput data are available, analysis may extend to cost per completed workload or unit of output.

### 4. Explore GPU infrastructure unit economics

Create an **illustrative 64-GPU capacity scenario**, varying:

- GPU acquisition or lease cost and associated infrastructure expenditure
- Electricity, cooling, PUE, networking, and other operating costs
- Customer pricing and billable GPU utilisation
- Capacity and demand assumptions

Use sensitivity analysis to explore how assumptions change potential revenue, cost recovery, and investment feasibility. **The model will be hypothetical and must not be interpreted as an audited provider financial statement.**

### 5. Visualise findings and assess the Indian market

Plan to build comparative charts and a dashboard that communicate cost differences, configuration trade-offs, and sensitivity to utilisation. A complementary India-focused research brief will examine relevant providers, market positioning, infrastructure developments, and customer needs.

## Planned outputs

| Deliverable | What it will contain |
| --- | --- |
| GPU pricing dataset | Sourced, dated observations and a data dictionary |
| Comparative analysis | Like-for-like pricing tables and visualisations |
| Workload cost model | Training, inference, and intermittent-use scenarios |
| Infrastructure economics model | Illustrative 64-GPU scenario and sensitivity analysis |
| Dashboard | Interactive comparison and decision-support views |
| India market brief | Indian provider landscape, opportunities, and constraints |
| Research report | Methodology, evidence, findings, assumptions, and limitations |

### Proposed repository structure

The folders below represent the **planned organisation**; they will be added as research outputs are produced.

```text
.
├── README.md
├── data/          # Cleaned, shareable pricing observations
├── sources/       # Source registry and collection dates
├── notebooks/     # Data cleaning, exploration, and comparisons
├── models/        # Workload-cost and 64-GPU economics scenarios
├── dashboard/     # Dashboard files and screenshots
└── reports/       # Research notes, final report, and presentation
```

## Research principles and limitations

- **Traceability:** Every commercial or pricing claim should be supported by an identifiable source and observation date.
- **Comparability:** A lower listed GPU-hour price does not necessarily mean a lower total workload cost.
- **Transparency:** Assumptions, missing data, exchange rates, and exclusions will be documented.
- **Separation of evidence:** Published offers, planned infrastructure investments, and hypothetical model outputs will not be presented as equivalent facts.
- **No premature results:** This README describes the research plan. Findings, datasets, and models will be published as they are developed and validated.

## Current progress

**Research and implementation are ongoing.** This repository will be updated progressively with collected data, analysis, models, visualisations, and documented findings. No completed benchmarks or conclusions are claimed here.

## Researcher

**Karthik Srivatsan**  
B.S. in Data Science & Artificial Intelligence, IIM Sambalpur  
Independent Research Project · 2026

---

*This project is an independent academic/portfolio research initiative and is not affiliated with or endorsed by any GPU cloud provider mentioned above.*
