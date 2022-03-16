---
layout: distill
title: dislocations
description: towards QM accuracy
img: /assets/img/QMML_preview.png
importance: 1
category: work

bibliography: 2018-12-22-distill.bib
---

Dislocations are extended line defects which carry plastic deformation in crystalline materials <d-cite key="Hirth"></d-cite>. Understanding and optimizing dislocation behaviour by characterising dislocation interaction with point defects is a central topic in computational metallurgy <d-cite key="leyson2010quantitative"></d-cite>.  For this task, *ab initio* calculations, specifically density functional theory (DFT) <d-cite key="Martin"></d-cite>, are essential to capture dislocation core structures and complex bonding to impurity elements. However, the computational cost of DFT typically scales as $$\mathcal{O}(N^3)$$ for metallic systems,  which limits its direct applicability to the study of extended defects. Within this project I develop and apply hybrid QM/MM methods <d-cite key="bernstein2009hybrid,Kermode_Swinburne_2017"></d-cite> which allow to study unfeasibly large systems with *ab initio* accuracy.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        <img class="img-fluid rounded z-depth-1" src="{{ '/assets/img/qm_ml_coupling.png' | relative_url }}" alt="" title="QM/MM coupling scheme"/>
    </div>
</div>
<div class="caption">
    QM/MM coupling scheme.
</div>

Hybrid QM/MM coupling scheme practically requires running two simulations in parallel: [`LAMMPS`](https://www.lammps.org/) for MM part and [`VASP`](https://www.vasp.at/) for DFT cell while the coupling is implemented with python [`ASE`](https://wiki.fysik.dtu.dk/ase/ase/calculators/qmmm.html?highlight=qmmm#force-based-qm-mm) interface. The QM/MM forcs $$\bf F_{\mathrm{QM/MM}}$$ is obtained by mixing MM force $$\bf F_{\mathrm{LAMMPS}}$$ with *ab initio* force $$\bf F_\mathrm{VASP}$$ with simple relation:  

$$
    \bf F_{\mathrm{QM/MM}} =
         \begin{cases}
         \bf F_{\mathrm{VASP}} , & \bf X \in \mathrm{QM} \\
         \bf F_{\mathrm{LAMMPS}}, & \mathrm{otherwise}
         \end{cases}
$$

where $$\bf X$$ is atomic coordinates vector and $$\mathrm{QM}$$ denotes QM region shown with blue color. The position of the atoms are then updated according to the QM/MM force $$\bf F_{\mathrm{QM/MM}}$$ during ionic minimisation.
An important aspect of hybrid QM/MM simulations is the need to have a buffer of sacrificial DFT atoms (shown with orange color), suitably large to protect the target cluster from electronic free surface effects.

This method provides a unique tool to study dislocations with *ab initio* accuracy <d-cite key="QMMM_H_SD"></d-cite>. Moreover, further extension of the capabilities is possible by combination of the method with recent developments in machine learning based force fields <d-cite key="PhysRevMaterials.5.103803"></d-cite>. Exploration of this possibility is the main topic of [this project](/projects/qmml).  
