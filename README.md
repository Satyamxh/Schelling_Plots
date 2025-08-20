# Thesis Plots Repository

This repository contains the PDF plots generated for my Master's thesis on **Schelling Point Oracles and p+ε Attacks**.  
All plots are stored together in a single folder due to upload restrictions.  

---

## File Naming Convention

Each file name encodes the **plot type**, **parameter focus**, and **mechanism**:

- **Sensitivity Analysis**
  - `morris_scatter_<mechanism>.pdf` → Global sensitivity via Morris method  
  - `sobol_<mechanism>_M7.pdf` → Sobol’ decomposition plots (baseline M=7)  
  - `eps_slope_heatmap_<mechanism>.pdf` → Heatmap of local bribe sensitivity (∂P/∂ε)  

- **Robustness Analysis**
  - `sice_<mechanism>_<param>_M7_<attack|noattack>.pdf` → S-ICE plots (λ, x, or ε varied)  
  - `eps_tau_ecdf_<mechanism>_M7.pdf` → ECDF of robustness thresholds (ε*, varying τ)  
  - `eps_star_frontier_overlay.pdf` → Robustness frontier ε* vs jury size M  

- **Parameter Response Surfaces**
  - `PX_surface_x_lambda__<mechanism>__batch_results_x_lambda_<mechanism>.pdf`  
  - `PX_surface_p_d__<mechanism>__batch_results_p_d_<mechanism>.pdf`  
  - `PX_surface_M_eps__<mechanism>__batch_results_M_epsilon_<mechanism>.pdf`  

Where `<mechanism>` ∈ {`basic`, `redistributive`, `symbiotic`}.

---

## Purpose of Repository

- To provide a **complete set of final plots** for sensitivity, robustness, and parameter response analysis.  
- To allow structured **discussion writing** based on empirical results.  
- Figures will be referenced in the thesis discussion sections as:
  - *Sensitivity and Robustness Analysis*
  - *Parameter Response Surfaces for Schelling Oracle Outcomes*

---

## Instructions for Deep Research Query

When analyzing these plots:
1. **Group by theme** (sensitivity, robustness, parameter response).
2. For each plot:
   - Summarize **what parameters are varied**.  
   - Interpret **key trends or thresholds**.  
   - Highlight **differences across payoff mechanisms** (basic, redistributive, symbiotic).  
3. Suggest whether the plot belongs in the **main thesis body** or **appendix**.

---

## Notes
- Unless otherwise specified, baseline is **M=7 jurors**.  
- File naming ensures reproducibility and mapping back to simulations.  
