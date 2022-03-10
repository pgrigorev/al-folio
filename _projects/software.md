---
layout: distill
title: open source
description: scientific software development
img: /assets/img/code_snapshot.png
importance: 3
category: work

bibliography: 2018-12-22-distill.bib

---

The problem of software reliability and reproducibility of the results in computational science was recognised a while ago <d-cite key="merali2010computational,Baker2016"></d-cite>. I am committed to incorporate the best practices of open and reproducible research <d-cite key="Mesirov2010, manifesto"></d-cite> in scientific software development and share my codes within these open source projects:

- `ASE`- [Atomic Simulation Environment: A Python library for working with atoms](https://wiki.fysik.dtu.dk/ase/).

    I developed an interface for [force based QM/MM](https://wiki.fysik.dtu.dk/ase/ase/calculators/qmmm.html?highlight=qmmm#force-based-qm-mm) coupling in a form of standard [ASE calculator](https://wiki.fysik.dtu.dk/ase/ase/calculators/calculators.html#module-ase.calculators). I also contributed to the development of few minimisation algorithms as well as to testing of various parts of ASE.

- `matscipy` - [Python materials science tools built around the ASE](https://github.com/libAtoms/matscipy)

    Here my main contribution is a [set of tools](https://github.com/libAtoms/matscipy/blob/master/matscipy/dislocation.py) for manipulation and analysis of atomistic configurations containing various types of dislocations in cubic crystals.

Normally for every publication I provide a link to a repository containing raw data and analysis pipelines. Execution of these pipelines requires installation of `ASE` and `matscipy` and can be done by following instructions in README files. If you struggle with using these codes or have any other feedback please do not hesitate to [contact me](mailto:Petr.Y.Grigorev@gmail.com).
