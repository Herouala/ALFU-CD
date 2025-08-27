Adaptive Caching Strategies for NDN (ALFU-CD and Baselines)

This repository contains the implementation and evaluation of multiple caching strategies for Named Data Networking (NDN), with a focus on the proposed Adaptive Least Frequently Used with Change Detection (ALFU-CD) strategy. The project simulates dynamic workloads with popularity shifts and compares cache performance across several well-known policies.

📌 Implemented Strategies

FIFO (First-In, First-Out)

LRU (Least Recently Used)

LFU (Least Frequently Used)

LFUDA (LFU with Aging)

SIEVE (Recency–frequency hybrid)

ALFU-CD (proposed strategy: LFU + dual-window + chi-squared change detection)

📊 Evaluation Metrics

The simulations evaluate each caching policy using four metrics:

Hit Rate – fraction of cache hits.

Eviction Ratio – normalized number of evictions.

Utilization – average cache occupancy.

Fairness – Jain’s fairness index across cached items.

⚙️ Simulation Setup

Workload requests are generated using Zipf distributions with varying skewness (
α
α) to model realistic content popularity.

Popularity shifts occur in three phases, each with a different Zipf exponent.

Results are averaged over multiple runs for robustness.

Outputs include plots exported to PDF.

🚀 Getting Started
1. Clone the repository
2. https://github.com/Herouala/ndn-caching-alfu-cd.git
cd ndn-caching-alfu-cd
2. Install dependencies

This project requires Python 3 and the following libraries:
pip install numpy==1.24.0 matplotlib==3.6.3 scipy==1.14.1

3. Run simulations
4. python ALFU-CD.py
This will generate a cache_strategies_results.pdf file containing plots of all metrics.

📂 Repository Structure
.
├── ALFU-CD.py                # Main simulation code
├── cache_strategies_results.pdf (output after running)
├── README.md                  # Project description

📘 Citation

If you use this code in academic work, please cite our paper:
[citation once paper is published]

