---
layout: distill
title: QM/ML for ML
description: and ML for QM/ML
img: /assets/img/dislo_electrons_with_vitek_scaled.png
importance: 2
category: work

bibliography: 2018-12-22-distill.bib
---

The [previous project](/projects/qm_dislocations) discussed the limitations *ab initio* methods when applied to study dislocations and how hybrid QM/MM methods can be used to overcome these limitations.
The fact that there is a lack of *ab initio* data for dislocations means that these structures are absent in the training databases used for interatomic potential development. Thus, while using these force fields for large scale simulations of dislocations the user largely rely on the predictive power of the potential <d-cite key="Unke2021"></d-cite>. On top of that, it is impossible to estimate the accuracy of the potentials in the extrapolation regime *once again* due to the lack of reference *ab initio* data.

This project explores how recent Machine Learning based force fields <d-cite key="goryaeva2019towards,PhysRevMaterials.5.103803"></d-cite> can be used in hybrid QM/ML (MM is replaced with ML for Machine Learning) to provide *ab initio* accurate data on dislocations.
The obtained QM/ML data serves as an important reference for testing the potentials in the extrapolation regime as well as (re)training of the potential allowing systematic improvement. In this way ML (embedding potential) is used for QM/ML and, in turn, QM/ML (data) is used for further improving ML potentials. This is what we called *synergistic coupling* in *ab inito*-machine learning simulations.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        <img class="img-fluid rounded z-depth-1" src="{{ '/assets/img/retraining_scheme_atoms.jpg' | relative_url }}" alt="" title="Synergistic QM/ML coupling"/>
    </div>
</div>
<div class="caption">
    Synergistic QM/ML coupling scheme.
</div>

Starting from a potential with correct elastic properties ($$\Theta_0$$), we evaluate properties of dislocations with standard QM/ML scheme (a). The resulting *ab initio* forces are then targeted in a novel retraining procedure, which exploits the linear parametric form to precisely match core structures whilst preserving elastic and other properties (b). Coupling to this retrained potential ($$\Theta$$) allows dislocations to cross the quantum/classical boundary of a spherical QM region centred on a point defect (c).  The QM/ML data from three dimensional simulation can be used for another round of retraining allowing the systematic improvement of interatomic potentials (c). This approach opens a vast range of previously inaccessible defect structures to *ab initio* investigation. You can find more details about the approach as well as the results regarding dislocation-defect interaction in tungsten in our recent paper <d-cite key="Grigorev2023"></d-cite>.
