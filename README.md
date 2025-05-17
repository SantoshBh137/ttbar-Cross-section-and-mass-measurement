# 🧪 CMS Top Quark Analysis — 7 TeV 

This project performs a measurement of the **top quark pair production cross section** and **top quark mass** using a small fraction (50 pb⁻¹) of real LHC proton-proton collision data collected by the **CMS detector at √s = 7 TeV** during 2011.

---

## 📂 Data and Simulation

The analysis uses both real and simulated CMS datasets in the form of ROOT ntuples, including:

- **Data**: 469,384 triggered events with single isolated muons (pₜ > 24 GeV)
- **Signal MC**: Top pair production (tt̄)
- **Background MCs**: W+jets, DY, QCD, single top, WW, WZ, ZZ

All Monte Carlo samples are normalized to an integrated luminosity of 50 pb⁻¹ and reweighted for pile-up.

---

## 🧭 Analysis Strategy

### ✔️ Event Selection

- Semi-leptonic tt̄ decay topology with:
  - ≥1 isolated muon
  - ≥4 jets (2 b-tagged)
  - Missing transverse energy (MET)
- Event variables studied:
  - Jet and lepton multiplicities
  - Transverse momenta
  - B-tag scores
  - Angular distributions

### 🎯 Signal Optimization

- Optimize selection cuts to maximize signal-to-background (S/B) ratio
- Apply selection to data and compare to MC
- Estimate selection efficiency and acceptance using simulation

---

## 📊 Measurements

### 1. Top Quark Cross Section

The cross section is extracted via:
- **N_obs**: Number of selected events in data
- **N_bkg**: Estimated background from MC
- **ε_trig**: Trigger efficiency (from MC)
- **ε_acc**: Acceptance × reconstruction efficiency (from MC)
- **L**: Integrated luminosity (50 pb⁻¹)

### 2. Top Quark Mass

- Reconstruct the top quark mass from detector objects using both the hadronic and leptonic decay branches
- Use kinematic constraints (e.g., W mass, MET) to solve for neutrino pₓ, pᵧ, p_z
- Compare reconstructed mass distributions between data and simulation

---

## 📁 File Structure


---

## 🛠️ Tools and Technologies

- Python (with uproot, awkward-array, numpy, matplotlib)
- ROOT (for tree inspection and plotting)
- CMS Open Data / PHYS565 Analysis Framework

---

## 📚 Reference

This project is part of the Purdue PHYS565 course: *Experimental Particle Physics*.


