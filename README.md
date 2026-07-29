# ROP vs Hydraulics Trade-off Analysis - Drilling Optimization

## Objective
Optimize Rate of Penetration (ROP) without compromising hole cleaning or exceeding fracture gradient. Hydraulics analysis for vertical well.

## Methodology
- Variables: Flow Rate (300-600 gpm), ROP (20-80 ft/hr), ECD, dP_ann
- Models: Moore & Chien for cuttings transport
- Safety Criteria: dP_ann < 150 psi, ECD < 10.5 ppg, Cutting Conc. < 5%

## Results Dashboard
![Dashboard](e8561ea0-b351-40c6-be00-11cf28137a9e.jpg)

## Analysis of the 4 Charts

### 1. ROP vs Annular Pressure Loss
dP_ann increases exponentially after 60 ft/hr. At 60 ft/hr = 125 psi (safe), at 70 ft/hr = 160 psi (exceeds 150 psi limit). High risk of pack-off.

### 2. Flow Rate vs ECD
With 400-500 gpm, ECD stays at 10.1-10.45 ppg (below frac gradient 10.5 ppg). At 550+ gpm, ECD rises to 10.7-11.0 ppg = risk of lost circulation.

### 3. ROP vs Cutting Concentration
Up to 60 ft/hr, cutting concentration < 5% (optimal). At 70 ft/hr it rises to 6.5% and at 80 ft/hr to 8% = cuttings bed formation.

### 4. Optimization Window (Key Chart)
Integrates all variables. The green dashed box is the Sweet Spot where all 3 criteria are met simultaneously.

## Final Conclusion
Operational sweet spot identified at **50-60 ft/hr with 450 gpm**, delivering:
- **ECD: 10.29 - 10.45 ppg** (below fracture gradient)
- **dP_ann: 102 - 125 psi** (below 150 psi limit)
- **Cutting Conc: < 5%** (hole cleaning assured)

This optimization maximizes ROP while maintaining wellbore safety and reduces NPT from hole cleaning issues by an estimated 30%.

## Tools
Python, pandas, matplotlib, Hydraulics Modeling

---
**Author:** Jose | Petroleum Engineer | Drilling Optimization
**Location:** Cartagena, Colombia
