---
layout: distill
date: 2022-07-01 10:00:00-0300
title: "Our QM/MM implementation is used to learn grain-boundary segregation from first principles."
inline: False

bibliography: 2018-12-22-distill.bib
---

Recent Physical Review Letters paper <d-cite key="Wagih2022"></d-cite> published by Malik Wagih and Christopher A. Schuh describes a novel approach to build a machine learning based model of grain boundary segregation energies of a  solute atom in a metal polycrystal. The framework learns directly on the _ab initio_ data, thus, bypassing the need for accurate interatomic potentials. To showcase the power of the approach the results of 36 solutes in Al are presented.

QM/MM method is used to provide _ab initio_ accurate data on solute segregation energy for a given grain boundary, which is otherwise inaccessible by standard DFT methods due to system size limitations. [Our force mixing scheme](https://wiki.fysik.dtu.dk/ase/ase/calculators/qmmm.html?highlight=qmmm#force-based-qm-mm) is used for relaxation of the system while final segregation is obtained from energy mixing scheme <d-cite key="Huber2016, Huber2017"></d-cite>.

These are very exciting results that show the power of combination of the QM/MM and machine learning to build _ab initio_ accurate models of solute interaction with extended defects and microstructural features. It opens vast opportunities to study fundamental properties of metals and alloys. We employ similar philosophy in our [QM/ML project to study interaction of point defects in dislocations](/projects/qmml).
