# 🌍 CarbonGlobe Dataset
> **Accepted to NeurIPS 2025 (Datasets & Benchmarks Track)** 
> Project page is available on NeurIPS: https://neurips.cc/virtual/2025/loc/san-diego/poster/121701.
> Datasets are available on Kaggle: https://www.kaggle.com/datasets/zhihaow/carbonglobe.



## Overview
**CarbonGlobe** is a comprehensive, ML-ready dataset for modeling and forecasting the forest carbon cycle. It integrates heterogeneous Earth system variables into a consistent spatiotemporal grid and provides standardized **scenario-based evaluations** and **benchmark implementations** to accelerate research across climate science, environmental monitoring, and ecological modeling.


## Key Features
- **Global coverage at 0.5°**  
  First global-scale ML-ready dataset for monitoring and forecasting forest carbon dynamics.
- **Multi-decadal span (40 years)**  
  Enables long-term trend and variability analysis.
- **100+ variables**  
  Harmonized inputs from meteorology, CO₂, soils, vegetation, and ancillary layers.
- **Scenario-based splits**  
  Training/testing protocols resembling real applications (e.g., climate zones, forest age).
- **Benchmarks & metrics**  
  Strong baselines (LSTM, Transformer family, DeepED, etc.) and **problem-driven metrics** for carbon forecasting.


## Source Datasets
All inputs are from open sources. Please follow original licenses and citation guidelines.

- **Meteorological (MERRA-2)**  
  NASA GMAO MERRA-2 (Gelaro et al., 2017).  
  Source: https://gmao.gsfc.nasa.gov/reanalysis/MERRA-2/  
  Citation guidance: https://gmao.gsfc.nasa.gov/reanalysis/MERRA-2/citing_MERRA-2/

- **CO₂ (NOAA CarbonTracker)**  
  Peters et al., 2007.  
  Source: https://gml.noaa.gov/ccgg/carbontracker/

- **Soils (ROSETTA)**  
  Montzka et al., 2017. CC BY 3.0.  
  DOI: https://doi.pangaea.de/10.1594/PANGAEA.870605

- **Climate Zones (Köppen–Geiger)**  
  Beck et al., 2018. CC BY 4.0.  
  Data: https://figshare.com/articles/dataset/6396959/2



## Benchmarks 
We provide reproducible baselines covering classical sequence models, knowledge-guided emulators, and recent transformer variants:

- **LSTM** — Standard recurrent model for time-series forecasting [[Graves, 2012]](https://www.cs.toronto.edu/~graves/phd.pdf)  
- **LSTNet** — CNN+RNN for short/long dependencies [[Lai et al., 2018]](https://arxiv.org/abs/1703.07015)  
- **DeepED** — Knowledge-guided ED emulator (error-accumulation mitigation) [[Wang et al., 2023]](https://doi.org/10.1145/3589132.3625577)  
- **Transformer** — Vanilla self-attention [[Vaswani et al., 2017]](https://arxiv.org/abs/1706.03762)  
- **Informer** — ProbSparse attention for efficiency [[Zhou et al., 2021]](https://arxiv.org/abs/2012.07436)  
- **DLinear** — Seasonal/trend decomposition with linear heads [[Zeng et al., 2023]](https://arxiv.org/abs/2205.13504)  
- **Crossformer** — Cross-time/feature attention [[Zhang et al., 2023]](https://openreview.net/forum?id=vSVLM2j9eie)  
- **TimeXer** — Decoupled inter-target & input-target modeling [[Wang et al., 2024]](https://arxiv.org/abs/2402.19072)

**Problem-driven metrics** (e.g., RMSE, MAE, delta error, cumulative error) are included to capture both step-wise and long-horizon behavior.


## 📚 Citation

f you use CarbonGlobe in your research, please cite:

> **Zhihao Wang**, **Lei Ma**, **George Hurtt**, **Xiaowei Jia**, **Yanhua Li**, **Ruohan Li**, **Zhili Li**, **Shuo Xu**, **Yiqun Xie**.  
> *CarbonGlobe: A Global-Scale, Multi-Decade Dataset and Benchmark for Carbon Forecasting in Forest Ecosystems.*  
> In *Proceedings of the 39th Conference on Neural Information Processing Systems (NeurIPS)*, 2025.

<!-- ```bibtex
@inproceedings{wang2025carbonglobe,
  title     = {CarbonGlobe: A Global-Scale, Multi-Decade Dataset and Benchmark for Carbon Forecasting in Forest Ecosystems},
  author    = {Wang, Zhihao and Ma, Lei and Hurtt, George and Jia, Xiaowei and Li, Yanhua and Li, Ruohan and Li, Zhili and Xu, Shuo and Xie, Yiqun},
  booktitle = {Proceedings of the 39th Conference on Neural Information Processing Systems (NeurIPS 2025), Datasets and Benchmarks Track},
  year      = {2025}
}
``` -->


## 📬 Contact

For questions or feedback, feel free to reach out:

- **Zhihao Wang** — [zhwang1@umd.edu](mailto:zhwang1@umd.edu)
- **Yiqun Xie** — [xie@umd.edu](mailto:xie@umd.edu)

