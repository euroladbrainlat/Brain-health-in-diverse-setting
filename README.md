<p align="center">
  <img src="images/header.png" width="400" alt="Cabecera">
</p>


# <p align="center">Brain health in diverse setting: How age, demographics and cognition shape brain function</p>


## Summary

This repository contains the codes and databases necessary for the results of the study: "Brain health in diverse settings: How age, demographics, and cognition shape brain function". Below are descriptions of the databases and scripts provided.

## Folder hierarchy
- **main_results/**
  - **Data/** `Databases required for analysis. They are described in more detail in the following section.`

  - **ROIs/** `Databases required for analysis. They are described in more detail in the following section.`

  - **Results/**
       - **Images/** `Databases required for analysis. They are described in more detail in the following section.`
    
  
       - **Models/**
         - **Aperiodic/**
           
         - **Complexity/**

         - **Connectivity/**

         - **Frequency/**



## Databases
The metric group databases used in the study (Power spectrum metrics, Aperiodic metrics, Complexity metrics, and Connectivity metrics) are available in the repository. Below are descriptions of each database:

### Main results:
- main_results/Data/aperiodic_cognition.xlsx
- main_results/Data/aperiodic_total_sample.xlsx
- main_results/Data/complexity_cognition.xlsx
- main_results/Data/complexity_total_sample.xlsx
- main_results/Data/frequency_cognition.xlsx
- main_results/Data/frequency_total_sample.xlsx
- main_results/Data/connectivity_cognition.xlsx
- main_results/Data/connectivity_total_sample.xlsx
---
### Supplementary results:
- supp_results/Data/aperiodic_cognition.xlsx
- supp_results/Data/aperiodic_total_sample.xlsx
- supp_results/Data/complexity_cognition.xlsx
- supp_results/Data/complexity_total_sample.xlsx
- supp_results/Data/frequency_cognition.xlsx
- supp_results/Data/frequency_total_sample.xlsx
- supp_results/Data/connectivity_cognition.xlsx
- supp_results/Data/connectivity_total_sample.xlsx

### General Description:
Each database includes subjects' age, sex, and education years. Those databases containing cognition data also provide subjects' Mini-Mental State Examination (MMSE) scores. Databases in the main_result directory encompass all subjects utilized in the study, while those located in the supp_results directory pertain to subjects recorded solely with eyes closed. The databases with the suffix *_cognition* contain cognition data, while the one with the *_total* suffix includes all subjects.

#### Power spectrum metrics:

Power spectrum analyses were conducted in both the canonical EEG frequency bands and subject-specific EEG frequency bands (92). The canonical frequency bands were defined as follows: 

- Delta (𝛿): 1.5-6 Hz
- Theta (𝛳): 6.5-8.0 Hz
- Alpha1 (𝛼1): 8.5-10 Hz
- Alpha2 (𝛼2): 10.5-12.0 Hz
- Beta1 (𝛽1): 12.5-18.0 Hz
- Beta2 (𝛽2): 18.5-21.0 Hz
- Beta3 (𝛽3): 21.5-30.0 Hz
- Gamma (𝛾): 30.0-40.0 Hz

Subject-specific frequency bands were determined using the individual alpha frequency peak (IAF), defined as the frequency with maximum power in the alpha-frequency band, and the theta/alpha-frequency transition (TF), defined as the frequency with minimum power in the second half of the theta frequency range. The subject-specific frequency bands are defined as follows: 

- Delta (TF-4 to TF-2)
- Theta (TF-2 to TF)
- Alpha low (TF to IAF)
- Alpha high (IAF to IAF+2) (92)

The beta and gamma frequency bands corresponded to the canonical division.

#### Aperiodic metrics:

Aperiodic components of the EEG power spectral density (PSD) were computed using the FOOOF algorithm. The components were: the 1/f slope (a), knee (k), and offset (b).

#### Complexity metrics:

We adopt a complexity definition in which signals with greater complexity display increased irregularity. To quantify this, we utilized fractal dimension estimation (FD), permutation entropy (PE), Wiener entropy (WE), and spectral structure variability (SSV).

#### Connectivity metrics:

We computed four weighted graph metrics: global efficiency, transitivity, small-worldness, and density. These metrics were derived from weighted matrices obtained using three functional connectivity metrics (mutual information, conditional mutual information, and organizational information).

