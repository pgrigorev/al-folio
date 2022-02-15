---
layout: page
title: QM/ML for ML
description: and ML for QM/ML
img: /assets/img/QMML_preview.png
importance: 2
category: work
---

*Ab initio* simulations of extended defects such as dislocation and cracks require system sizes at or beyond existing limits. Hybrid simulations coupling *ab initio* to linear machine learning potentials can be used to overcome these limitations. The method allows arbitrary sub-regions of large scale simulations to be treated with *ab initio* accuracy. The obtained QM/ML data can be used for the retraining of the potential allowing systematic improvement. In this way ML (embedding potential) is used for QM/ML and, in turn, QM/ML (data) is used for further improving ML potentials. This is what we called *synergistic coupling* in *ab inito*-machine learning simulations.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        <img class="img-fluid rounded z-depth-1" src="{{ '/assets/img/retraining_scheme_atoms.jpg' | relative_url }}" alt="" title="Synergistic QM/ML coupling"/>
    </div>
</div>
<div class="caption">
    Synergistic QM/ML coupling scheme.
</div>

Starting from a potential with correct elastic properties ($$\Theta_0$$), we evaluate properties of dislocations with standard QM/ML scheme (a). The resulting *ab initio* forces are then targeted in a novel retraining procedure, which exploits the linear parametric form to precisely match core structures whilst preserving elastic and other properties (b). Coupling to this retrained potential ($$\Theta$$) allows dislocations to cross the quantum/classical boundary (c).  The QM/ML data from three dimensional simulation can be used for another round of retraining allowing the systematic improvement of interatomic potentials (c). This approach opens a vast range of previously inaccessible defect structures to *ab initio* investigation. You can find more details about the approach as well as the results regarding dislocation-defect interaction in tungsten in our [recent preprint](https://arxiv.org/abs/2111.11262).
