# Truss-Bridge-Model-Vibration-Benchmark-Dataset
## 📖 Overview

This dataset provides benchmark vibration data for a truss bridge model under two types of excitation. It can be used as a benchmark dataset for validating methods in moving load identification, modal identification, structural model updating, and structural anomaly detection, among others.

## Truss Bridge Model

A laboratory-scale steel truss bridge model was constructed for vibration testing. The bridge consists of a **6.0 m main span** and two **0.7 m approach spans**. All primary structural members are made of Q235 steel. The upper and lower chords have rectangular cross-sections of 150 mm × 5 mm, while the intermediate members have circular cross-sections with a diameter of 10 mm. The main span is simply supported, and the structural members are connected through bolted joints.

<img src="FIG/Fig1.jpg" width="600" alt="Truss Bridge Model">
<img src="FIG/Fig2.png" width="600" alt="Truss Bridge Model">
<p align="center">
  <em>Fig. 1. The truss bridge model.</em>
</p>

## Test scenarios

The bridge model is designed with easily detachable vertical members, allowing different anomaly locations and severities to be simulated by replacing members with different cross-sectional sizes. The structural anomaly cases are simulated by reducing the cross-sectional areas of selected vertical members. The easily detachable vertical members are designed with four different sizes, and their corresponding diameters and cross-sectional reduction ratios are illustrated in Fig. 3.

By sequentially replacing the vertical members at the five locations with the three reduced-section members, **15 damaged conditions (Cases 1–15)** are generated, together with one undamaged reference condition (Case 0).

<img src="FIG/Fig3.png" width="600" alt="Truss Bridge Model">
<p align="center">
  <em>Fig. 2. The detachable vertical members.</em>
</p>

## 📥 Dataset Download

The complete dataset is publicly available through the following platforms:

| Platform | Download |
|:---|:---|
|  **Baidu Netdisk** | [Download Dataset](https://pan.baidu.com/s/1VPeSs4PSzYhjfpAPyXlW-Q?pwd=u7tg) |
|  **Google Drive** | [Download Dataset](https://drive.google.com/drive/folders/1I5ez2_0RFDQFCa35PJ9AjpGVECRVmFLx?usp=sharing) |

## 📚 Citation

If you use this dataset in your research, **please cite the following publication**:

> Hua-Ping Wan, Yi-Kai Zhu, Can Wang, and Michael D. Todd.  
> **Multiscale pattern learning for vibration-based structural anomaly detection: A benchmark dataset and validation study.**  *Structural Health Monitoring*, 2026. DOI: [10.1177/14759217261499477](https://doi.org/10.1177/14759217261499477)



## 🔧 Structural Damage Simulation

Structural damage is simulated by **replacing detachable vertical members with members of reduced cross-sectional areas**. Five vertical members along the main span are selected as potential damage locations, labeled 1–5 from left to right.

For each damage scenario, **only one vertical member is replaced**, while the remaining members retain their original dimensions. The original member has a diameter of **10 mm**, and three replacement members with diameters of **8.7 mm, 7.1 mm, and 5.0 mm** are used to simulate cross-sectional area reductions of **25%, 50%, and 75%**, respectively.

By sequentially replacing the vertical members at the five locations with the three reduced-section members, **15 damaged conditions (Cases 1–15)** are generated, together with one undamaged reference condition (Case 0).

## 📊 Excitation and Data Acquisition

Two types of dynamic excitation are employed in the experiments:

- **Shaker-induced excitation:** White-noise excitation is applied using an MB Dynamics Modal 50 shaker at five designated locations along the main span.
- **Vehicle-induced excitation:** A scaled two-axle vehicle travels across the bridge under three different vehicle weights (**9.65 kg, 14.65 kg, and 19.65 kg**) to simulate moving loads.

The vibration responses are measured using **12 accelerometers and 5 displacement transducers**, with a sampling frequency of **512 Hz**. For shaker-induced tests, acceleration responses are recorded for 512 s, while vehicle-induced tests record both acceleration and displacement responses for 40 s.

All acquired data are stored in MATLAB (`.mat`) format and organized according to structural conditions and excitation configurations.
