---
layout: page
title: Current Work
description: Research recreations, alpha research software, and engineering notes in progress.
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

    <p>These projects show how I apply production engineering habits to research and exploratory software: clear system boundaries, reproducible workflows, readable implementations, documented tradeoffs, and tests around the behavior that matters.</p>

    <div class="work-grid">
      <article>
        <h3>Implicit Geometry Research</h3>
        <p>Educational reproductions of neural 3D representation methods, including DeepSDF, NeRF, NeuS, and NeuVAS-style experiments. The repository emphasizes method understanding, toy-data validation, and clear project-local notes before scaling to larger datasets.</p>
        <p><strong>Signals:</strong> PyTorch-style training loops, SDF/radiance-field modeling, mesh and slice visualization, reproducible toy experiments.</p>
      </article>

      <article>
        <h3><a href="{% link Projects/finding_alpha.md %}">Finding Alpha</a></h3>
        <p>A research-first equity screening and alpha-validation platform with a hosted Streamlit demo. It fetches historical market data, computes interpretable features, saves timestamped signal snapshots, and evaluates whether ranked technical setups predict forward returns. The project intentionally excludes live trading while the research loop is being validated.</p>
        <p><strong>Signals:</strong> Python package structure, provider interfaces, Parquet/DuckDB storage, Streamlit dashboard, tests, documented risk boundaries.</p>
        <ul class="actions small">
          <li><a href="{% link Projects/finding_alpha.md %}" class="button small">Case Study</a></li>
          <li><a href="https://findingalpha.streamlit.app/" class="button small" target="_blank" rel="noopener">Demo</a></li>
        </ul>
      </article>

      <article>
        <h3>OpenClaw Agentic Assistants</h3>
        <p>Practical agent systems built with OpenClaw, an open-source framework for orchestrating AI agents as personal technical assistants. My work focuses on codebase exploration, research support, workflow automation, memory systems, browser and shell tool use, and safe delegation between specialist agents.</p>
        <p><strong>Signals:</strong> TypeScript/Node.js agent orchestration, LLM tool use, local memory and vector search, GitHub and browser automation, approval boundaries, privacy-aware operations, and coding-agent workflows that augment human engineering judgement.</p>
      </article>
    </div>
  </div>
</section>

</div>
