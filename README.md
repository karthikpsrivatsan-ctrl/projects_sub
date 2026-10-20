# GPU Cloud Pricing & Market Research

**An independent research project exploring GPU cloud pricing, AI computing costs, and the economics of GPU infrastructure.**

**Status:** Research in Progress  
**Area:** AI Infrastructure | Cloud Computing | Data Analysis | Technology Economics

## About the Project

As a second-year student pursuing a B.S. in Data Science and Artificial Intelligence at IIM Sambalpur, I've become interested in the infrastructure that makes modern AI systems possible, particularly the growing demand for GPUs used in training and running AI models.

While exploring this area, I came across a question that interested me: **why do different cloud providers charge different prices for GPU computing, and how can we determine which option is actually more cost-effective?**

GPU cloud services allow researchers, startups, and companies to access computing power without purchasing expensive hardware. However, comparing these services isn't always straightforward. The cost depends on factors such as GPU specifications, cloud provider, pricing model, location, and workload requirements.

Through this independent project, I want to understand these differences using publicly available data and develop a clearer picture of how GPU computing is priced and used.

## Research Question

**How do GPU cloud prices vary across providers, and what factors should be considered when comparing the cost of running AI workloads?**

To explore this, I plan to investigate three smaller questions:

1. How much do cloud providers charge for comparable GPU configurations?
2. How do GPU specifications, pricing models, and other included resources affect these comparisons?
3. How might these pricing differences influence the cost of AI training and inference workloads?

## Research Approach

### 1. Understanding the GPU Cloud Market

I'll begin by studying the basic structure of the GPU cloud industry, including the differences between major cloud platforms and specialised GPU providers.

Some providers I plan to explore include:

- AWS and Google Cloud
- CoreWeave and Lambda
- Indian providers such as Yotta and E2E Networks

I'll also look at the development of AI computing infrastructure in India and how domestic providers are positioning themselves in this market.

### 2. Collecting and Comparing GPU Pricing Data

The next step is to build a small dataset using publicly available pricing information.

Where available, I plan to collect information about GPU models, memory, hourly rental prices, regions, billing options, and included computing resources.

Using Python and pandas, I'll organise the data and compare prices across providers.

One of the initial metrics I'll use is:

**Cost per GPU-hour = Hourly instance price / Number of GPUs**

However, I'll also consider the limitations of this metric, since two GPUs with different performance characteristics cannot necessarily be compared using hourly prices alone.

The aim is to make comparisons as consistent and transparent as possible rather than simply identifying the lowest advertised price.

### 3. Exploring AI Workload Costs

Once I've established a basic pricing comparison, I want to explore how these differences could affect the cost of running AI workloads.

This may include estimating the computing costs of model training and inference under clearly stated assumptions.

If suitable benchmarking data or computing resources become available, I would also like to explore performance-related metrics such as inference throughput and cost per unit of output.

This part of the project will depend on the data and resources available, and any estimates will be distinguished from actual measurements.

### 4. Analysing and Presenting Findings

I plan to use data analysis and visualisation to identify useful patterns in the dataset.

The broader objective is to understand how technical specifications and pricing decisions connect to the economics of AI infrastructure.

I am particularly interested in what these comparisons might mean for startups, researchers, and organisations deciding between different computing options.

## Tools and Skills

The project is intended to involve:

- **Python and pandas** for data collection, cleaning, and analysis
- **Matplotlib / Seaborn** for data visualisation
- **Excel** for pricing comparisons and basic cost modelling
- **Jupyter Notebook** for documenting and reproducing analysis
- **Public cloud documentation and research literature** as data sources

## Planned Outcomes

As the project progresses, I aim to develop:

- A documented dataset of publicly available GPU cloud pricing
- Python notebooks comparing selected providers and configurations
- Visualisations explaining pricing differences
- A basic model exploring the cost of selected AI workloads
- A short research report discussing findings, assumptions, and limitations

These are planned outcomes and will be added to the repository as they are completed.

## Current Status

This project is in its early stages. The research question and initial methodology have been outlined, and the next step is to develop the pricing dataset and begin the comparative analysis.

The scope and methodology may evolve as I gain a better understanding of GPU infrastructure and the availability of reliable data.

## Why I'm Working on This

My coursework in Data Science and AI has introduced me to machine learning, programming, and quantitative analysis. This project is an opportunity to connect those subjects with a part of the AI industry that I would like to understand better.

I'm especially interested in the intersection of **AI technology, computing infrastructure, and business economics**.

Beyond learning about GPU cloud services, I hope to gain practical experience in conducting independent research: asking a focused question, working with real-world data, evaluating assumptions, and communicating findings clearly.

I also hope this project can serve as a foundation for further research or collaborative work in AI infrastructure and cloud computing.

---

**Karthik Srivatsan**  
B.S. Data Science & Artificial Intelligence  
Indian Institute of Management Sambalpur

*Independent student research project | 2026*
