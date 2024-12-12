---
layout: archive
title: "Research"
permalink: /research/
author_profile: true
---

My research goals are to understand and model the evolution of ice shelves (the floating extensions of ice sheets) and the icebergs that calve (break off) from them.

Ice-shelf and iceberg meltwater can influence ocean circulation, sea-ice formation, and biological productivity. Furthermore, ice-shelf weakening due to thinning and damage (e.g. crevassing, calving, etc.) can cause upstream non-floating ice to flow more rapidly into the ocean, resulting in sea-level rise.

I aim to develop models that can simulate centuries of ice evolution, with enough accuracy to capture observed phenomena.

## Icebergs

I am a developer of the GFDL iceberg module, which comprises two modeling frameworks:

The first framework represents each iceberg (or a group of icebergs) as a single "point particle". For this approach, I recently parameterized the calving of small icebergs from the edges of larger bergs, which enables realistic representation of large tabular icebergs and their meltwater distribution. See [manuscript](https://doi.org/10.1029/2021MS002869).

The second iceberg modeling framework, the [improved Kinematic Iceberg Dynamics model (iKID)](https://www.gfdl.noaa.gov/modeling-tabular-icebergs/), represents each berg as a group of particles connected by numerical bonds. An iKID simulation of the breakup of iceberg A68 revealed a previously-unknown breakup mechanism, whereby part of the iceberg was caught in stronger currents than the rest of the berg, creating enough tension along the iceberg body to break it into pieces. See the animation below, the [GFDL summary](https://www.gfdl.noaa.gov/iceberg-a68a/), or the [manuscript](https://doi.org/10.1126/sciadv.abq6974).


<iframe width="480" height="270"
src="/files/A68a_obs_sim.mp4"
frameborder="0"
allow="accelerometer; autoplay; encrypted-media; gyroscope; picture_in_picture"
allowfullscreen></iframe>
Observed and simulated breakup of iceberg A68a

## Ice sheets

I am a developer of MOM6-IS, the ice-sheet component of GFDL coupled models that is embedded within the ocean model MOM6 (publication in prep).

I am also working on methods to simulate calving of large icebergs. These methods combine [damage mechanics](https://doi.org/10.1029/2020MS002292) and the particle-based [material point method](https://doi.org/10.1029/2020MS002277) (which was more famously used for animating snow in Disney's *Frozen*). Here, damage captures crevassing and full-thickness fracturing (rifting) that can lead to calving. I recently simulated the calving of iceberg A68 from the Larsen C ice shelf (see below). Subsequent simulations revealed how ice mélange and contact between rift flanks can control where rifts propagate, and therefore, the size of any resulting icebergs. See [manuscript](https://doi.org/10.1017/jog.2023.71).

![](/images/obs_sim_a68_calving.png)
Observed and simulated rifting and calving of iceberg A68.

{% include base_path %}
