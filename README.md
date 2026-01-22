
## Home

### Welcome

Welcome to the **Half Lab** at **King's College London**. We are a multidisciplinary research group focused on advancing neuroimaging methods and their application to brain development, health, and disease, with a particular emphasis on **ultra-low-field (ULF) MRI** and equitable global research.

Our work spans methodological development, quantitative analysis, and translational research, aiming to make advanced neuroimaging tools more accessible and reproducible across diverse settings.

### Research Themes

* Ultra-low-field MRI acquisition, reconstruction, and super-resolution
* Structural similarity networks and brain connectivity
* Reproducibility and reliability of neuroimaging measures
* Neurodevelopment across diverse populations
* Open, scalable, and reproducible neuroimaging workflows

### News

* **November 2025** – Lab member *Ula* joined the group!
* **September 2025** - Paper accepted to Imaging Neuroscience https://doi.org/10.1162/IMAG.a.930
* **September 2025** – Levi won first place in the MICCAI 2025 Challenge: Enhancing Ultra-Low-Field MRI with Paired High-Field MRI Comparisons for Brain Imaging (ULF-EnC) 

---

## Research

### Overview

Our research combines **neuroimaging physics**, **computational analysis**, and **developmental neuroscience**. We focus on methods that are robust to hardware constraints and scalable to low-resource environments.

### Key Projects

#### Project 1
Description

#### Project 2
Description

#### F.R.A.M.E: Feasibility, Reproducibility, and Application of MRI-derived brain networks for Early childhood development
This project investigates whether structural similarity networks derived from ultra-low-field MRI retain biologically meaningful information, and how these networks compare to those derived from conventional field strengths. Through collaborations in low- and middle-income countries, we explore how portable neuroimaging can support research into healthy brain development and neurological risk.

#### Ultra-low field Neuroimaging In The Elderly-UNITE
The project involves the assessment of the ultra-low field MRI acceptability and its potential in detecting dementia biomarkers such as brain volumetric changes and vascular abnormalities.
This will be achieved by collecting conventional MRI scans and ultra-low field MRI scans, and developing pipelines with imaging analysis tools and deep learning implementation to improve ultra-low field scan quality.
---

## People

---
layout: default
title: People
---

## Principal Investigator

{% for person in site.people %}
  {% if person.group == "PI" %}
    <div class="person-block">
      <img src="{{ person.photo }}" alt="Photo of {{ person.name }}">
      <h3>{{ person.name }}</h3>
      <p><strong>{{ person.role }}</strong><br>{{ person.affiliation }}</p>
      <p>{{ person.content | markdownify }}</p>
    </div>
  {% endif %}
{% endfor %}

## Lab Members

<div class="people-grid">
{% for person in site.people %}
  {% if person.group == "member" %}
    <div class="person-card">
      <img src="{{ person.photo }}" alt="Photo of {{ person.name }}">
      <h4>{{ person.name }}</h4>
      <p><strong>{{ person.role }}</strong></p>

      {% if person.interests.size > 0 %}
      <ul>
        {% for interest in person.interests %}
          <li>{{ interest }}</li>
        {% endfor %}
      </ul>
      {% endif %}
    </div>
  {% endif %}
{% endfor %}
</div>


### Alumni

No one has left yet!

---

## Publications

### Selected Publications

* **František Váša**, Carly Bennallick, Niall J. Bourke, Francesco Padormo, Levente Baljer, Ula Briski, Paul Cawley, Tomoki Arichi, Tobias C. Wood, David J. Lythgoe, Flavio Dell’Acqua, Thomas C. Booth, Ashwin V. Venkataraman, Emil Ljungberg, Sean C.L. Deoni, Rosalyn J. Moran, Robert Leech, Steven C.R. Williams (2025). *Ultra-low-field brain MRI morphometry: Test–retest reliability and correspondence to high-field MRI*. Imaging Neuroscience. [DOI](https://doi.org/10.1162/IMAG.a.930)

* **Levente Baljer**, Yiqi Zhang, Niall J. Bourke, Kirsten A. Donald, Layla E. Bradford, Jessica E. Ringshaw, Simone R. Williams, Sean C. L. Deoni, Steven C. R. Williams, Khula SA Study Team, František Váša, Rosalyn J. Moran (2024). *Ultra-Low-Field Paediatric MRI in Low- and Middle-Income Countries: Super-Resolution Using a Multi-Orientation U-Net*. Human Brain Mapping. [DOI](https://doi.org/10.1002/hbm.70112)

### Preprints

* **Levente Baljer**, Ula Briski, Robert Leech, Niall J Bourke, Kirsten A Donald, Layla E Bradford, Simone R Williams, Sadia Parkar, Sidra Kaleem, Salman Osmani, Sean CL Deoni, Steven CR Williams, Rosalyn J Moran, Emma C Robinson, Frantisek Vasa (2025). *GAMBAS: Generalised-Hilbert Mamba for Super-resolution of Paediatric Ultra-Low-Field MRI*. arXiv

* **Ula Briski**, Niall J. Bourke, Kirsten A. Donald, Layla E. Bradford, Simone R. Williams, Michal R. Zieff, Sean C.L. Deoni, Steven C.R. Williams, Khula South Africa Study Team, Rosalyn J. Moran, Levente Baljer, František Váša (2025). *Deep learning super-resolution of paediatric ultra-low-field MRI without paired high-field scans*. bioRXiv

---

## Software & Data

We strongly support **open science**. When possible, our software and derived data products are released openly.

### Software

* **shared-utils** – This repository will contain functions commonly used by the Half Lab members for processing and analysis.
[Github](https://github.com/haflab/shared-utils)

### Data & Workflows

* Reproducible pipelines using Flywheel, Docker, and Jupyter
* Documented batch-processing scripts for non–command-line users

---

## Join the Lab

<!-- ### Prospective Students

We welcome applications from motivated students with backgrounds in neuroscience, engineering, physics, computer science, or related fields. Prior experience with MRI is **not required**. -->

### Collaborations

We are always interested in collaborating with researchers and clinicians, particularly those working in global health and low-resource settings.

If you are interested, please contact František **frantisek.vasa@kcl.ac.uk**.

---

## Contact

**HALF Lab**
Neuroimaging
King's College London
London, United Kingdom

Email: frantisek.vasa@kcl.ac.uk
GitHub: https://github.com/haflab
