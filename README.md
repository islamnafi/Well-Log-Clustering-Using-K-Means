This project applies **K-Means clustering** to petrophysical well log data to identify patterns and segment the subsurface into meaningful clusters. The workflow is useful for unsupervised lithofacies classification and early-stage reservoir characterization.

---

## Tools & Libraries

- **Python 3**
- **pandas**, **numpy**
- **scikit-learn**
- **matplotlib**

---

## Dataset

- Features used:
  - `RHOB` – Bulk Density  
  - `NPHI` – Neutron Porosity  
  - `GR` – Gamma Ray  
  - `PEF` – Photoelectric Factor  
  - `DTC` – Sonic Travel Time

---

## Workflow Summary

1. **Data Preprocessing**  
   - Remove null values  
   - Normalize features using `StandardScaler`

2. **Cluster Optimization**  
   - Use elbow method to determine optimal `K`

3. **Clustering**  
   - Apply K-Means (with `K=3`) on selected features

4. **Visualization**  
   - Generate RHOB vs NPHI scatter plot, color-coded by cluster

---

## Results

- Successfully clustered the well log data into **3 distinct groups**
- Visual separation is evident in crossplot space, suggesting potential **lithological or facies** differences
