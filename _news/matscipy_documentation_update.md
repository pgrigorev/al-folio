---
layout: post
date: 2023-11-09 
inline: false
title: Check out new functionality and updated documentation of matscipy.
---

We have been working recently on an update of documentation and tutorials for the `matscipy.dislocation` module. Below you can see few examples of atomistic dislocations that can be created using the module: 1/2<110>{110} screw dislocation in BCC and dissociated 1/2<110>{111} in FCC and Diamond Cubic systems. These are not just pictures, they are interactive! Feel free to spin it around, zoom and hover the mouse over the atoms to get more information about the system. The tutorial on [building cylindrical configurations with dislocations](https://libatoms.github.io/matscipy/applications/cylinder_configurations.html) explains in detail how they were created using `matscipy.dislocation` and how it can be used for atomistic simulations of dislocations. 

On top of that, thanks to the efforts of [Thomas Rocke](https://github.com/thomas-rocke), the functionality of the module was extended beyond single species systems. The [multi-species dislocation systems tutorial](https://libatoms.github.io/matscipy/applications/multispecies_dislocations.html) demonstrates the new features taking Zincblende structure and $$\text{In}_{0.5} \text{Ga}_{0.5} \text{As}$$ alloy as an example. The result for a partial 1/6<112> $$\beta$$-$$90^\circ$$ dislocation is shown bellow.


<div style="display: flex; justify-content: space-between;">
    <div style="width: 50%; text-align: center;">BCC: 1/2<111> screw in W </div>
    <div style="width: 50%; text-align: center;">FCC: dissociated 1/2<110> screw in Ni</div>
</div>

<iframe src="/assets/html/W_Ni_demo.html"
    sandbox="allow-same-origin allow-scripts"
    width="100%"
    height="300"
    scrolling="no"
    seamless="seamless"
    frameborder="0">
</iframe>

<div style="display: flex; justify-content: space-between;">
    <div style="width: 50%; text-align: center;">Diamond: dissociated 1/2<110> 90&deg; screw in Si </div>
    <div style="width: 50%; text-align: center;">Zincblende: partial 1/6<112> &beta;-90&deg; in In<sub>0.5</sub>Ga<sub>0.5</sub>As</div>
</div>

<iframe src="/assets/html/Si_GaAs_demo.html"
    sandbox="allow-same-origin allow-scripts"
    width="100%"
    height="300"
    scrolling="no"
    seamless="seamless"
    frameborder="0">
</iframe>
