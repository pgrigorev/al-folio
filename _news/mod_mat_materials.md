---
layout: distill

date: 2024-08-29
inline: false
title: Tutorials from 'Modélisation des Matériaux' summer school are available online.

bibliography: 2018-12-22-distill.bib
---

This august together with [Arnaud Allera](https://arn-all.github.io/) and [Martin Uhrin](https://digitalbaker.net/) I contributed to machine learning part of the ['Modélisation des Matériaux'](https://www.cinam.univ-mrs.fr/site/modmat/banyuls/index.php?page=programme) summer school. We developed three interactive tutorials on python ecosystem for materials modelling, introduction to descriptors of atomic environments with neighbors map <d-cite key="Allera2024"></d-cite> and on the structural analysis employing neighbors maps and several machine learning techniques. The tutorials are available on the [github page](https://github.com/pgrigorev/ModMatEcole) and can be run via Binder or Google Colab. Please go to the [github repo](https://github.com/pgrigorev/ModMatEcole) for the links as well as instructions on how to run the notebooks locally if you wish to do so. Do not hesitate to [contact me](mailto:petr.y.grigorev@gmail.com) if you have any questions and/or suggestions. 

<iframe src="/assets/html/Fe_cell.html"
    sandbox="allow-same-origin allow-scripts"
    width="100%"
    height="300"
    scrolling="no"
    seamless="seamless"
    frameborder="0">
</iframe>

<div style="display: flex; justify-content: center;">
    <iframe src="/assets/html/neighbours_map.html"
        style="display: flex; margin: auto;" 
        width="100%"
        height="410"
        seamless="seamless"
        frameborder="0">
    </iframe>
</div>

What you see above is an example of an interactive visualisation of the neighbors map construction used in the second tutorial. First you see the 9 atoms cell of perfect BCC iron with highlighted four distances between the atoms. Then the graph representation and of the atomic environment of the central atom with index 1 (left) and the resulting neighbors map (right) are shown. Every node of the graph represents an atom and every line of the pixels on the neighbors map image correspond to sorted distances between an atom and all his neighbors (here we have chosen 8 neighbors). If you click on a node, all connected edges are highlighted together with corresponding line on the neighbors map image. Try to explore this interactive visulasation to understand the relation between 3D atomic structure, graph representation and the resulting descriptor image. When you hover over nodes, pixels or atoms there is additional information displayed in order to help you. Note that an attention factor is applied on the lines of the image, that do not correspond to the central atom. This is why the color of the pixels on the first row is not the same as on the first column, while the distances are the same (hover over pixels to verify). Attention factors are not applied on the graph. For more details and more complex scenarios together with applications and source code please [visit the github repository](https://github.com/pgrigorev/ModMatEcole).
