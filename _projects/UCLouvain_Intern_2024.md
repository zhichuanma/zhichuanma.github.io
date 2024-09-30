---
title: "Multi-criteria analysis based on Life-cycle assessment of a positive energy district accounting for a country context – application to real case study"
collection: projects
toc: true
date: 2024-08-09
permalink: /projects/REHO_LCA/
period: Mar. 2024 - Sept 2024
abstract:   
excerpt: "<img src='/images/UCLouvain_intern_2024/district_documentation.svg' width='600px'>"
course: False
---

{% include base_path %}

* Research project at Institute of Mechanics, Materials and Civil Engineering([IMMC](https://uclouvain.be/en/research-institutes/immc)), UCLouvain, Belgium
* March. 2024 -- Sept. 2024
* Supervisor: [Prof. Herve Jeanmart](https://scholar.google.com/citations?user=cZ5224EAAAAJ&hl=en)
* Project Mentor: [Postdoc. Gauthier Limpens](https://scholar.google.fr/citations?user=rOP9mX4AAAAJ&hl=fr)
* Keywords: *LCA*, *Multi-objective optimization*, *Energy system*, *Dantzig–Wolfe decomposition*

## Introduction
---

This project is part of [InterPED](https://interped.eu/about/), an European commission project. InterPED aims to enable the concept of Positive Energy Districts (PEDs) via sector coupling, cross-vector integration, demand flexibility and consumer engagement, while improving utilisation of local renewable energy sources (RES), storage and excess/waste heat (E/WH) sources. 

To acheive the targets above, an energy system optimization tool called [REHO](https://reho.readthedocs.io/en/main/) (renewable energy hub optimizer) is adapted. Within this model, multiple technologies are taken into consideration and the problems (district optimization) are characerized into several sub-problems (house optimization) and one master problem as the figure below shows:

<div class="gallery">
    <a href="/images/UCLouvain_intern_2024/diagram_model.svg" data-lightbox="mygallery" data-title="Image 1 Description">
        <img src="/images/UCLouvain_intern_2024/diagram_model.svg" alt="Image 1" style="width: 100%; height: auto;">
    </a>
</div>

In this model, given EUD (end use demand) profiles (from the meteorological data and the buildings characteristics), the resources to which it has access to provide those EUDs, namely the grids and the equipments that can be used to convert those resources into the required services, it could conduct multi-objective optimization in different scenarios, based on AMPL. For more information, I highly recommend you to go to REHO's official website: [REHO](https://reho.readthedocs.io/en/main/). It's an open-source tool developped by EPFL and UCLouvain but there still plenty of places could be improved.

The primary objective of my task is to **integrate a comprehensive life-cycle assessment (LCA) framework into this model**. While the current model includes some aspects of life-cycle assessment, there are significant areas that require improvement. Specifically:

* Database Quality: The database currently used is not sufficiently robust or reliable, leading to inaccuracies in the assessment results.
* Methodological Rigor: The methodology employed in the existing model is not sufficiently rigorous or detailed, which undermines the overall effectiveness of the life-cycle assessment.

To address these issues, it is essential to create a completely new database and implement better methodology to ensure a more accurate and credible life-cycle assessment. Meanwhile, other tasks like **multi-objective optimization** and **real case studies for the pilots' sites** are also involved in this internship.

## Achievements
---

Since this internship is still ongoing. I have completed most of the works autonomously and independenly with few discussions.

The current achievements are:

* Implemented new LCA methodology from another energy system tool called [Energyscope](https://energyscope.readthedocs.io/en/master/);
* Generalized the LCA indicators with Brightway2 and integrated World IMPACT+ LCA methods into the database;
* Removed double counting for the datas from ecoinvent database
* Created mapping files with the machine learning methods (*eg. we need to map the technologies in REHO with the activities in Ecoinvent. The machine learning tool could read the technologies' text and map it to some most probable activities in Ecoinvent (highest similarities)*)
* Integrated the LCA framework into both the AMPL model and python scripts
* Did Normalization
* Conducted a Case study for Lugaritz community in Spain

## Final Results

Presentations can be seen by clicking [here](/images/UCLouvain_intern_2024/Internship_presentation_Zhichuan.pdf).

Final reports can be downloaded by clicking [here](/files/Master 2 Thesis.pdf)

