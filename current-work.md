---
layout: page
title: Current Work
description: Research recreations, alpha research software, and portfolio cleanup in progress.
image: /assets/images/coding_room.jpg
nav-menu: true
show_tile: true
permalink: /current-work/
---

<!-- Main -->
<div id="main" class="alt">

<section id="one">
  <div class="inner current-work">
    <header class="major">
      <h1>Current Work</h1>
    </header>

    <p>I am using this site to show current engineering practice rather than only finished artifacts. These projects are works in progress, but they already demonstrate the kind of habits that matter in research and industry: scoped experiments, readable implementations, tests, notes, and honest status tracking.</p>

    <div class="work-grid">
      <article>
        <h3>Implicit Geometry Research</h3>
        <p>Educational reproductions of neural 3D representation methods, including DeepSDF, NeRF, NeuS, and NeuVAS-style experiments. The repository emphasizes method understanding, toy-data validation, and clear project-local notes before scaling to larger datasets.</p>
        <p><strong>Signals:</strong> PyTorch-style training loops, SDF/radiance-field modeling, mesh and slice visualization, reproducible toy experiments.</p>
      </article>

      <article>
        <h3>Finding Alpha</h3>
        <p>A research-only stock screener and alpha testing dashboard. It fetches historical market data, computes interpretable features, saves timestamped signal snapshots, and evaluates whether rankings predict forward returns. The project intentionally excludes live trading while the research loop is being validated.</p>
        <p><strong>Signals:</strong> Python package structure, provider interfaces, Parquet/DuckDB storage, Streamlit dashboard, tests, documented risk boundaries.</p>
      </article>

      <article>
        <h3>Portfolio Rebuild</h3>
        <p>A cleanup of this site so it reads like an active engineering portfolio instead of an archived student website. The first pass removes the stale resume, makes current work easy to find, and separates public project summaries from private progress notes.</p>
        <p><strong>Signals:</strong> clear writing, lightweight information architecture, maintenance discipline, deployment through GitHub Pages.</p>
      </article>
    </div>

    <h2>Near-Term Site Direction</h2>
    <p>The next useful step is adding short demos or screenshots for each active project: a DeepSDF reconstruction image, a NeRF render, a Finding Alpha dashboard screenshot, and a short explanation of what each demo proves technically.</p>
  </div>
</section>

</div>
