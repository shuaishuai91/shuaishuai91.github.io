---
permalink: /
title: "Biography"
author_profile: true
redirect_from:
  - /about/
  - /about.html
---

I am a Postdoctoral Researcher in the School of Civil and Environmental Engineering at Cornell University, working with Professors Qi Li and John D. Albertson. I received my Ph.D. in Mechanical Engineering from Arizona State University in 2024, where I worked with Professor Mohamed Houssem Kasbaoui. Before that, I earned an M.S. in Mechanical Engineering from Washington University in St. Louis in 2017 and a B.S. in Mechanical Engineering from Shanghai Jiao Tong University in 2014.

My research focuses on the dynamics of particle-laden flows, combining high-fidelity numerical simulations and mathematical analysis to understand particle transport and particle–fluid interactions. During my Ph.D., I investigated how particle inertia and two-way coupling influence vortex dynamics and flow instability, leading to three first-author publications in *Journal of Fluid Mechanics*. At Cornell, I study inertial-particle transport and preferential deposition in atmospheric boundary-layer flows, as well as the rotational dynamics and preferential orientation of non-spherical particles under the effects of turbulence, inertia, and gravitational settling.

My broader research interests include computational fluid dynamics, multiphase flows, and geophysical and environmental fluid mechanics.

## Research

### Particle-Laden Vortex Flow

<style>
.particle-vortex-video-stack {
  display: flex;
  flex-direction: column;
  align-items: flex-start;
  gap: 1rem;
  margin: 1.2rem 0 1.5rem;
}
.particle-vortex-video-stack figure {
  margin: 0;
  width: 100%;
  max-width: 350px;
}
.particle-vortex-video-stack video {
  display: block;
  width: 100%;
  height: auto;
}
.particle-vortex-video-stack figcaption {
  color: #666;
  font-size: 0.85em;
  text-align: center;
  margin-top: 0.4rem;
}
</style>

<div class="particle-vortex-video-stack">
  {% assign evolution_video = site.static_files | where: "path", "/files/evolution.mp4" | first %}
  {% if evolution_video %}
  <figure>
    <video autoplay muted loop playsinline controls preload="metadata" aria-label="Evolution of an inertial-particle-laden vortex">
      <source src="{{ '/files/evolution.mp4' | relative_url }}" type="video/mp4">
      Your browser does not support HTML5 video.
    </video>
    <figcaption>Evolution of an inertial-particle-laden vortex.</figcaption>
  </figure>
  {% endif %}
  {% assign merger_video = site.static_files | where: "path", "/files/merger.mp4" | first %}
  {% if merger_video %}
  <figure>
    <video autoplay muted loop playsinline controls preload="metadata" aria-label="Merger of co-rotating vortices in dusty flows">
      <source src="{{ '/files/merger.mp4' | relative_url }}" type="video/mp4">
      Your browser does not support HTML5 video.
    </video>
    <figcaption>Merger of co-rotating vortices in dusty flows.</figcaption>
  </figure>
  {% endif %}
</div>

My research examines how suspended inertial particles influence the dynamics of coherent vortices through preferential concentration and two-way momentum coupling. Using Eulerian–Lagrangian simulations, I showed that particles migrating outward from a Lamb–Oseen vortex form concentrated clusters and substantially accelerate vortex decay compared with viscous diffusion alone. In co-rotating vortex pairs, particle feedback can fundamentally change the merger process: particles with moderate inertia temporarily push the vortices apart to nearly twice their initial separation, whereas higher particle inertia can cause vortex-core stretching and splitting. I also use scaling analysis to identify the characteristic time scales governing particle redistribution and vortex evolution.

**Related publications:** [DOI: 10.1017/jfm.2022.50](https://doi.org/10.1017/jfm.2022.50) · [DOI: 10.1017/jfm.2024.67](https://doi.org/10.1017/jfm.2024.67)

### Flow Stability Analysis

<style>
.flow-stability-layout {
  display: grid;
  grid-template-columns: minmax(0, 1fr) minmax(0, 1fr);
  align-items: start;
  column-gap: 1.5rem;
  max-width: 750px;
  margin: 1.2rem 0 1.5rem;
}
.flow-stability-layout figure {
  margin: 0;
  max-width: 350px;
  min-width: 0;
}
.flow-stability-layout video {
  display: block;
  width: 100%;
  height: auto;
}
.flow-stability-layout figcaption {
  margin-top: 0.5rem;
  color: #666;
  font-size: 0.85em;
  text-align: center;
}
.flow-stability-layout .stability-description p {
  margin-top: 0;
}
@media (max-width: 700px) {
  .flow-stability-layout {
    grid-template-columns: minmax(0, 1fr);
    row-gap: 1rem;
  }
}
</style>

<div class="flow-stability-layout">
  <figure>
    <video autoplay muted loop playsinline controls preload="metadata" aria-label="Evolution of unstable azimuthal modes m equals 3 through 6">
      <source src="{{ '/files/stability.mp4' | relative_url }}" type="video/mp4">
      Your browser does not support HTML5 video.
    </video>
    <figcaption>Evolution of unstable azimuthal modes (m = 3–6) in a particle-laden vortex.</figcaption>
  </figure>
  <div class="stability-description">
    <p>I investigate how particle–fluid interactions can destabilize flows that would otherwise remain stable without particles. Combining linear stability analysis with Eulerian–Lagrangian simulations, I studied a particle-laden Rankine vortex and identified an instability driven by two-way momentum coupling. Even non-inertial particles can destabilize the vortex through a mechanism analogous to centrifugal Rayleigh–Taylor instability. Finite particle inertia further expands the range of unstable modes. The theoretical analysis provides criteria for instability and predictions of mode growth rates, which agree with numerical simulations. Beyond the linear stage, the instability develops into spiral structures in the particle concentration and vorticity fields.</p>
  </div>
</div>

**Related publication:** [DOI: 10.1017/jfm.2022.687](https://doi.org/10.1017/jfm.2022.687)

### Geophysical and Environmental Fluid Dynamics with Particle Transport

I apply numerical modeling to investigate inertial-particle transport and deposition in environmental flows, particularly dust transport in atmospheric boundary layers. Using large-eddy simulation (LES) coupled with a Lagrangian stochastic particle model, I examine how vegetation barriers modify turbulent flow structures and redistribute airborne particles. The simulations show that canopy-generated wakes can promote preferential concentration and downward transport, resulting in locally enhanced particle deposition downstream of the barrier. The enhancement becomes stronger with increasing particle inertia. This work provides physical insight into how vegetation-induced flow structures influence particle transport and ground deposition, with implications for the assessment of dust-control barriers.

**Related manuscript (under review):** [Preprint](https://doi.org/10.21203/rs.3.rs-9164043/v1)
