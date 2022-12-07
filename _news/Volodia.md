---
layout: distill
date: 2022-11-21 10:00:00-0300
title: "Extremely proud to be a part of an amazing achievement of my brother Volodia! :trophy:"
inline: False

bibliography: 2018-12-22-distill.bib
---

An article titled **"Optically Triggered Néel Vector Manipulation of a Metallic Antiferromagnet Mn$$_2$$Au under Strain"** has been accepted for publication in **ACS Nano** journal and is now [avialable online](https://pubs.acs.org/doi/full/10.1021/acsnano.2c07453). My brother **Vladimir Grigorev** is the first author of this publication! The article demonstrates the manipulation of direction of the staggered magnetization of a sample using combination of strain and laser pulses. The motivation of the study is testing the capabilities of the material for future ultra fast high-density memory spintronic devices.

The experimental results are backed up by a profound theoretical analysis as well as computational modelling. The article represents an extraordinary example of successful collaboration between few teams with various backgrounds. My humble role was to perform Density Functional Theory calculations of _magneto-elastic coupling constant_ $$B_{me}$$ that shows how preferable orientation of magnetic moments of the atoms changes with applied strain.

Mn$$_2$$Au is a metallic collinear antiferromagnet with body central tetragonal crystall structure. Easy directions are along $$\langle 110 \rangle$$ axis, this means that in the ground state magnetic moments of Mn atoms lie in $$(001)$$ plane and are oriented along one of the $$\langle 110 \rangle $$ direction as shown on the figure. If a tensile strain along one of these easy directions (say $$\varepsilon _{110}$$) is applied does it favour the spin orientation along the strain $$[110]$$ or perpendicular $$[\bar110]$$? It is possible to answer this question by comparing the energy of strained configurations with two spin orientation $$\Delta E = E([\bar110]) - E([110])$$ as schematically shown below.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        <img class="img-fluid rounded z-depth-1" src="{{ '/assets/img/delta_E.png' | relative_url }}" alt="" title="Magneto-elastic coupling constant estimation scheme"/>
    </div>
</div>
<div class="caption">
    Magneto-elastic coupling constant estimation scheme.
</div>


If the $$ \Delta E $$ is positive, it means that the structure with magnetic moments parallel to the strain has lower energy and thus is more favourable. If the value is negative, then the orientation of magnetic moments perpendicular to the strain is preferred. As can be seen from the plot below, $$\Delta E$$ is negative for the positive values of strain along $$[110]$$ direction $$\varepsilon _{110}$$. This means that the tensile strain favours perpendicular orientation of magnetic moments. By making a linear fit of this results we obtain the magneto elastic constant of $$ B_{me}$$ = -0.92 meV per formula unit (one unit cell). This value means that one percent of strain results in 9.2 $$\mu$$eV of magnetic anisotropy per formula unit between easy directions $$\langle 110 \rangle$$. 

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        <img class="img-fluid rounded z-depth-1" src="{{ '/assets/img/smaller_strain_magnetostriction_pages.png' | relative_url }}" alt="" title="Magneto-elastic coupling constant estimation results"/>
    </div>
</div>
<div class="caption">
    Magneto-elastic coupling constant estimation results.
</div>
