---
layout: none
title: 'From Potential to Practice: Measuring AI''s Aggregate Economic Impact'
date: 2026-03-01
permalink: /posts/2026/03/macroeconomic-impact-ai/
---
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>From Potential to Practice: Measuring AI's Aggregate Economic Impact</title>
  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
  <link href="https://fonts.googleapis.com/css2?family=DM+Sans:ital,wght@0,300;0,400;0,500;0,600;1,400&family=DM+Serif+Display:ital@0;1&display=swap" rel="stylesheet">
  <style>
    *, *::before, *::after { box-sizing: border-box; margin: 0; padding: 0; }
    :root {
      --accent:      #2C5F8A;
      --accent-light:#EBF3FA;
      --accent-mid:  #A8C8E2;
      --bg:          #FFFFFF;
      --surface:     #F4F6F9;
      --ink:         #0F1923;
      --ink-mid:     #3D4F61;
      --ink-muted:   #7A8FA6;
      --rule:        #E2E8EF;
      --link:        #2C5F8A;
      --mono:        'JetBrains Mono', 'Fira Mono', monospace;
    }
    html { font-size: 18px; scroll-behavior: smooth; }
    body {
      font-family: 'DM Sans', system-ui, sans-serif;
      background: var(--bg);
      color: var(--ink);
      line-height: 1.75;
    }
    .topbar { background: var(--accent); height: 4px; }

    /* Header */
    .site-header {
      padding: 1.1rem 2rem;
      display: flex;
      align-items: center;
      justify-content: space-between;
      border-bottom: 1px solid var(--rule);
      background: var(--bg);
    }
    .site-header .wordmark {
      font-family: 'DM Serif Display', serif;
      font-size: 1rem;
      color: var(--ink-muted);
      letter-spacing: 0.01em;
    }
    .site-header .section-label {
      font-size: 0.62rem;
      font-weight: 500;
      letter-spacing: 0.16em;
      text-transform: uppercase;
      color: var(--accent);
      font-family: var(--mono);
    }

    /* Hero */
    .hero {
      background: var(--surface);
      border-bottom: 1px solid var(--rule);
      padding: 4.5rem 2rem 4rem;
      text-align: center;
    }
    .hero .topic-tag {
      display: inline-block;
      font-family: var(--mono);
      font-size: 0.62rem;
      letter-spacing: 0.2em;
      text-transform: uppercase;
      color: var(--accent);
      border: 1px solid var(--accent-mid);
      padding: 0.22em 0.9em;
      border-radius: 2px;
      margin-bottom: 1.5rem;
      background: var(--accent-light);
    }
    .hero h1 {
      font-family: 'DM Serif Display', serif;
      font-size: clamp(2rem, 4.5vw, 3.2rem);
      font-weight: 400;
      line-height: 1.18;
      max-width: 780px;
      margin: 0 auto 1.2rem;
      color: var(--ink);
      letter-spacing: -0.02em;
    }
    .hero .subtitle {
      font-size: 1.05rem;
      font-weight: 300;
      color: var(--ink-mid);
      max-width: 640px;
      margin: 0 auto 2.25rem;
      line-height: 1.65;
    }
    .hero .meta {
      font-family: var(--mono);
      font-size: 0.68rem;
      color: var(--ink-muted);
      letter-spacing: 0.07em;
    }
    .hero .meta span { margin: 0 0.5em; color: var(--accent-mid); }

    /* Layout */
    .container { max-width: 780px; margin: 0 auto; padding: 0 1.5rem; }

    /* Takeaways */
    .takeaways-wrap { padding: 3rem 0 0; }
    .takeaways {
      background: var(--accent-light);
      border: 1px solid var(--accent-mid);
      border-left: 4px solid var(--accent);
      border-radius: 0 6px 6px 0;
      padding: 1.75rem 2.25rem;
    }
    .takeaways .kicker {
      font-family: var(--mono);
      font-size: 0.62rem;
      letter-spacing: 0.2em;
      text-transform: uppercase;
      color: var(--accent);
      margin-bottom: 1rem;
      display: block;
    }
    .takeaways ul { padding-left: 1.2rem; list-style: disc; }
    .takeaways li {
      margin-bottom: 0.55rem;
      font-size: 0.95rem;
      color: var(--ink);
      line-height: 1.55;
    }
    .takeaways li:last-child { margin-bottom: 0; }
    .takeaways li strong { font-weight: 600; }

    /* Prose */
    .prose { padding: 2.75rem 0 3rem; }
    .prose h2 {
      font-family: 'DM Serif Display', serif;
      font-size: 1.6rem;
      font-weight: 400;
      color: var(--ink);
      margin: 3.25rem 0 1rem;
      padding-top: 2rem;
      border-top: 1px solid var(--rule);
      letter-spacing: -0.01em;
      line-height: 1.25;
    }
    .prose h2:first-child { margin-top: 0; padding-top: 0; border-top: none; }
    .prose p {
      margin-bottom: 1.3rem;
      font-size: 1rem;
      font-weight: 300;
      color: var(--ink-mid);
      line-height: 1.8;
    }
    .prose p strong { color: var(--ink); font-weight: 500; }
    .prose ul {
      padding-left: 1.4rem;
      margin-bottom: 1.3rem;
    }
    .prose ul li {
      font-size: 1rem;
      font-weight: 300;
      color: var(--ink-mid);
      line-height: 1.7;
      margin-bottom: 0.4rem;
    }
    .prose ul li strong { color: var(--ink); font-weight: 500; }

    /* Formula */
    .formula {
      background: var(--surface);
      border: 1px solid var(--rule);
      border-radius: 6px;
      padding: 0.75rem 1rem;
      font-family: var(--mono);
      font-size: 0.8rem;
      color: var(--ink);
      text-align: center;
      margin: 1.5rem 0 2rem;
      letter-spacing: 0.01em;
      white-space: nowrap;
      overflow-x: auto;
    }
    .formula .formula-line {
      display: block;
      margin-bottom: 0.35rem;
    }
    .formula .formula-line:last-child { margin-bottom: 0; }
    .formula .formula-comment {
      display: block;
      font-size: 0.72rem;
      color: var(--ink-muted);
      letter-spacing: 0.04em;
      margin-top: 0.6rem;
    }

    /* Tables */
    .table-wrap { margin: 2rem 0; overflow-x: auto; }
    .table-caption {
      font-family: var(--mono);
      font-size: 0.62rem;
      letter-spacing: 0.12em;
      text-transform: uppercase;
      color: var(--ink-muted);
      margin-bottom: 0.6rem;
    }
    table { width: 100%; border-collapse: collapse; font-size: 0.88rem; }
    thead tr { background: var(--ink); }
    thead th {
      font-family: var(--mono);
      font-size: 0.62rem;
      letter-spacing: 0.1em;
      text-transform: uppercase;
      padding: 0.75rem 1rem;
      text-align: left;
      font-weight: 500;
      color: #f5f4f0;
    }
    tbody tr:nth-child(even) { background: var(--surface); }
    tbody tr:hover { background: var(--accent-light); transition: background 0.15s; }
    tbody td {
      padding: 0.65rem 1rem;
      border-bottom: 1px solid var(--rule);
      color: var(--ink-mid);
      font-weight: 300;
    }
    tbody td:first-child { color: var(--ink); font-weight: 400; }
    .highlight-row td { background: var(--accent-light) !important; color: var(--ink) !important; font-weight: 400 !important; }

    /* Pull quote */
    blockquote.pullquote {
      margin: 2.75rem 0;
      padding: 0 0 0 1.5rem;
      border-left: 3px solid var(--accent);
    }
    blockquote.pullquote p {
      font-family: 'DM Serif Display', serif;
      font-size: 1.2rem;
      font-style: italic;
      color: var(--ink);
      line-height: 1.5;
      margin: 0;
    }

    /* Appendix */
    .appendix {
      background: var(--surface);
      border-top: 1px solid var(--rule);
      margin-top: 2rem;
      padding: 3.5rem 0 4rem;
    }
    .appendix h2 {
      font-family: 'DM Serif Display', serif;
      font-size: 1.45rem;
      font-weight: 400;
      color: var(--ink);
      margin-bottom: 0.4rem;
    }
    .appendix .app-intro {
      font-size: 0.92rem;
      color: var(--ink-muted);
      font-weight: 300;
      margin-bottom: 2rem;
    }
    .appendix h3 {
      font-family: var(--mono);
      font-size: 0.65rem;
      letter-spacing: 0.18em;
      text-transform: uppercase;
      color: var(--accent);
      margin: 2.5rem 0 0.75rem;
    }
    .appendix p {
      font-size: 0.9rem;
      color: var(--ink-mid);
      font-weight: 300;
      margin-bottom: 0.85rem;
      line-height: 1.7;
    }
    .appendix ul, .appendix ol { padding-left: 1.5rem; margin-bottom: 1rem; }
    .appendix li {
      font-size: 0.9rem;
      color: var(--ink-mid);
      font-weight: 300;
      margin-bottom: 0.45rem;
      line-height: 1.65;
    }
    .appendix strong { color: var(--ink); font-weight: 500; }
    .appendix code {
      font-family: var(--mono);
      font-size: 0.8rem;
      background: var(--bg);
      border: 1px solid var(--rule);
      padding: 0.05em 0.35em;
      border-radius: 3px;
      color: var(--accent);
    }
    .appendix table { font-size: 0.85rem; }
    .appendix thead tr { background: #0F2740; }
    .appendix .table-caption { margin-top: 1.5rem; }

    footer {
      text-align: center;
      padding: 2rem 1rem 2.5rem;
      font-family: var(--mono);
      font-size: 0.62rem;
      color: var(--ink-muted);
      letter-spacing: 0.08em;
      border-top: 1px solid var(--rule);
    }
    footer .dot { color: var(--accent); margin: 0 0.4em; }

    a { color: var(--link); text-decoration: underline; text-decoration-color: var(--accent-mid); }
    a:hover { text-decoration-color: var(--link); }

    @media (max-width: 600px) {
      html { font-size: 16px; }
      .hero { padding: 3rem 1.25rem 2.5rem; }
      .site-header { padding: 1rem 1.25rem; }
      .takeaways { padding: 1.5rem 1.25rem; }
    }
  </style>
</head>
<body>

<div class="topbar"></div>

<header class="site-header">
  <span class="wordmark">Shisham Adhikari</span>
  <span class="section-label">AI &amp; Labor Markets</span>
</header>

<section class="hero">
  <span class="topic-tag">AI Economics</span>
  <h1>From Potential to Practice: Measuring AI's Aggregate Economic Impact</h1>
  <p class="subtitle">Replacing theoretical exposure with observed usage collapses the 10-year Total Factor Productivity (TFP) estimate from 0.62% to 0.04%.</p>
  <p class="meta">Shisham Adhikari <span>&middot;</span> March 1, 2026</p>
</section>

<main>
<div class="container">

  <div class="takeaways-wrap">
    <div class="takeaways">
      <span class="kicker">Key Takeaways</span>
      <ul>
        <li><strong>There's a gap between AI's potential reach and actual use.</strong> Exposure-based models assign 18.7% of the GDP-weighted wage bill to AI-susceptible occupations. Real Claude usage data puts that at just 0.25%.</li>
        <li><strong>That gap sharply reduces estimated productivity gains.</strong> Exposure-based estimates imply a 0.62% boost to economy-wide productivity over ten years. Usage-based estimates imply just 0.01%.</li>
        <li><strong>The composition of AI users is a minor factor.</strong> Labor shares differ modestly between exposed (53.5%) and actually-using (57.6%) occupations. What drives the gap is simply how narrow current AI adoption is.</li>
      </ul>
    </div>
  </div>

  <div class="prose">

    <h2>Motivation</h2>

    <p>What is AI's actual impact on the economy today? It's one of the most important questions in economics right now and surprisingly hard to answer. Most estimates of AI's economic impact are built on theoretical exposure scores: models that predict which jobs AI <em>could</em> affect based on task descriptions. But exposure isn't the same as adoption, and the difference matters enormously for any serious estimate of economy-wide impact.</p>

    <p>I build on Acemoglu (2024), which provides a principled framework for estimating how productivity gains at the task level add up across occupations and industries into aggregate economic growth. I then ask what happens when I replace the theoretical exposure index with observed AI usage data from Anthropic's Economic Index (AEI)?</p>

    <h2>The Task Framework</h2>

    <p>Think of the economy as a collection of tasks—writing, coding, analyzing, building, advising—each performed by workers or machines. AI expands what machines can do, shifting some of those tasks away from human labor. But how much that shift matters for the broader economy depends on two things.</p>

    <p>First, tasks are complements, not substitutes. Automating one step in a process doesn't multiply output if other steps remain bottlenecks. A lawyer who drafts twice as fast still needs client meetings, review cycles, and court dates. This places a natural ceiling on how much partial automation can lift aggregate output. Second, AI doesn't affect all tasks equally. Its reach is greatest in routine cognitive work like coding, drafting, and classification, and weakest in tasks requiring physical presence, interpersonal judgment, or contextual reasoning.</p>

    <h2>Hulten's Theorem</h2>

    <p>To translate task-level gains into an economy-wide number, Hulten's theorem says the aggregate TFP impact of a productivity improvement equals that sector's share of GDP times the size of the improvement. Applied to AI:</p>

    <div class="formula">
      <span class="formula-line">TFP gain &asymp; task scope &times; feasibility &times; labor share &times; productivity gain per task</span>
      <span class="formula-line" style="color: var(--ink-muted); font-size: 0.8rem;">&asymp; s&#772;<sub>A</sub> &nbsp;&times;&nbsp; &phi; &nbsp;&times;&nbsp; s<sub>L</sub> &nbsp;&times;&nbsp; &pi;&#772;</span>
    </div>

    <p>Here s&#772;<sub>A</sub> is the GDP-weighted share of AI-exposed labor tasks; &phi; is the fraction of those tasks feasibly automated; s<sub>L</sub> is the labor share of income in AI-affected industries; and &pi;&#772; is the average labor cost saving per automated task.</p>

    <p>All four inputs vary across models—most substantially s̄<sub>A</sub>, which changes with index choice. φ differs by design (0.23 for exposure, 1 for usage and hybrid); s<sub>L</sub> shifts modestly with industry composition. π̄ is held constant in the main table and varied as a robustness check in Table 2.</p>

    <h2>Results</h2>

    <p>I compare three indices at the 6-digit SOC level, all fed into the same aggregation pipeline:</p>

    <ul>
      <li><strong>Exposure (Acemoglu 2024):</strong> Derived from Eloundou, Manning, Mishkin, and Rock (2023). Uses GPT-4 annotations of O*NET occupational task descriptions to measure AI susceptibility at the occupation level. Covers 798 occupations; GDP-weighted using BLS wage and employment data.</li>
      <li><strong>Usage (AEI, Anthropic 2025):</strong> Maps observed Claude interactions to O*NET occupational categories, capturing where workers are actively using AI today. Covers 608 occupations; occupations not in AEI receive zero.</li>
      <li><strong>Hybrid:</strong> Assigns usage values to occupations covered by AEI; falls back to the exposure index for the rest. An upper bound under the assumption that absence from AEI reflects data coverage rather than genuine non-adoption.</li>
    </ul>

    <p>One methodological adjustment: exposure measures potential susceptibility, so φ = 0.23 (Svanberg et al. 2024) applies. Usage captures tasks already being used—feasibility is revealed by adoption—so I set φ = 1 for usage and hybrid models.</p>

    <div class="table-wrap">
      <p class="table-caption">Table 1 &mdash; Main results under three index assumptions</p>
      <table>
        <thead>
          <tr>
            <th>Index</th>
            <th>s&#772;<sub>A</sub></th>
            <th>&phi;</th>
            <th>s<sub>L</sub></th>
            <th>TFP (10-yr)</th>
          </tr>
        </thead>
        <tbody>
          <tr>
            <td>Exposure (Acemoglu baseline)</td>
            <td>18.70%</td>
            <td>0.23</td>
            <td>53.51%</td>
            <td>0.62%</td>
          </tr>
          <tr class="highlight-row">
            <td>Usage (AEI, φ = 1)</td>
            <td>0.25%</td>
            <td>1</td>
            <td>57.63%</td>
            <td>0.04%</td>
          </tr>
          <tr>
            <td>Hybrid (usage + exposure fill, φ = 1)</td>
            <td>1.47%</td>
            <td>1</td>
            <td>58.72%</td>
            <td>0.23%</td>
          </tr>
        </tbody>
      </table>
    </div>

    <p>Labor shares differ modestly across models (53–59%); the TFP gap is driven by s̄<sub>A</sub>.</p>

    <h3>Sensitivity to the productivity gain parameter</h3>

    <p>The baseline π̄ = 0.27 averages writing and customer-service experiments (Noy and Zhang 2023; Brynjolfsson, Li, and Raymond 2023). Since AEI usage is concentrated in software development (see <a href="/shadhikari/posts/2026/02/ai-exposure-vs-usage/">previous post</a>), Table 2 varies π̄ using task-type-specific estimates from the literature.</p>

    <div class="table-wrap">
      <p class="table-caption">Table 2 &mdash; TFP sensitivity to π̄ (usage and hybrid)</p>
      <table>
        <thead>
          <tr>
            <th>Source</th>
            <th>Task type</th>
            <th>&pi;&#772;</th>
            <th>Usage TFP</th>
            <th>Hybrid TFP</th>
          </tr>
        </thead>
        <tbody>
          <tr>
            <td>Brynjolfsson, Li, and Raymond (2023)</td>
            <td>Customer service</td>
            <td>0.14</td>
            <td>0.02%</td>
            <td>0.12%</td>
          </tr>
          <tr class="highlight-row">
            <td>Acemoglu (2024) baseline</td>
            <td>Mixed average</td>
            <td>0.27</td>
            <td>0.04%</td>
            <td>0.23%</td>
          </tr>
          <tr>
            <td>Noy and Zhang (2023)</td>
            <td>Professional writing</td>
            <td>0.40</td>
            <td>0.06%</td>
            <td>0.35%</td>
          </tr>
          <tr>
            <td>Peng, Kalliamvakou, Cihon, and Demirer (2023)</td>
            <td>Coding tasks</td>
            <td>0.55</td>
            <td>0.08%</td>
            <td>0.47%</td>
          </tr>
        </tbody>
      </table>
    </div>

    <p>Even at π̄ = 0.55 (Peng, Kalliamvakou, Cihon, and Demirer 2023, coding), usage TFP reaches 0.08% and hybrid 0.47%—both below the 0.62% exposure baseline. The gap is driven by s̄<sub>A</sub>, not by which experiment calibrates π̄.</p>

    <blockquote class="pullquote">
      <p>The gap is almost entirely driven by the scope of AI adoption—how many tasks it is currently reaching—not by disagreement about how productive it is within those tasks.</p>
    </blockquote>

    <h2>Conclusion</h2>

    <p>A task-based framework is a useful, microfounded way to think about AI's aggregate macroeconomic impact. It forces precision: the headline number depends on how broadly AI is deployed, how many of those tasks cross the feasibility threshold, the labor intensity of affected industries, and how much productivity it delivers per task. Right now, actual deployment is narrow. The gap between what AI could reach and where it is actually being used accounts for nearly all the difference between the optimistic and realistic estimates.</p>

    <p>Going forward, the actual impact will depend on how each of these pieces evolves—how widely AI adoption spreads across occupations, what share of exposed tasks prove cost-effective at scale, the labor share of industries where diffusion runs deepest, and whether productivity gains generalize beyond the domains studied so far. Tracking those changes carefully, as AI diffuses, is what will determine whether the aggregate estimate moves toward the upper or lower end of the range.</p>

  </div>

</div><!-- /container -->
</main>

<section class="appendix">
<div class="container">

  <h2>Appendix</h2>
  <p class="app-intro">Technical details on data, construction, and limitations.</p>

  <h3>A. TFP Formula</h3>
  <p>Follows from Hulten (1978) applied to Acemoglu's (2024) task-based model with gross complementarity (σ &lt; 1). To first order: <code>d ln TFP = s&#772;_A &times; &phi; &times; s_L &times; &pi;&#772;</code>. The product <code>s&#772;_A &times; &phi;</code> is the "feasible share"—the fraction of total labor GDP that AI can realistically displace near-term.</p>

  <h3>B. Data Sources</h3>
  <ul>
    <li><strong>Exposure index:</strong> Acemoglu (2024) via Eloundou, Manning, Mishkin, and Rock (2023). GPT-4 annotations of O*NET work activities aggregated to 6-digit SOC. 798 occupations; GDP-weighted using BLS OEWS (2019–2024).</li>
    <li><strong>AEI usage index:</strong> Anthropic Economic Index, September 2025. Maps observed Claude interactions to O*NET occupational categories. 608 SOC occupations covered. Used as <code>aei_usage_pct / 100</code> without rescaling.</li>
    <li><strong>Wage &amp; employment:</strong> BLS OEWS national estimates, 2019–2024.</li>
    <li><strong>Industry labor shares:</strong> BEA NIPA industry accounts, averaged 2018–2022, matched via NAICS crosswalk.</li>
  </ul>

  <h3>C. Parameter Choices and Rationale</h3>
  <p><strong>φ (feasibility of automation).</strong> Acemoglu (2024) sets φ = 0.23 based on Svanberg et al. (2024), who estimate the fraction of AI-exposed tasks that are cost-effective at current prices. This filter is appropriate for the exposure model, where s̄<sub>A</sub> captures potential susceptibility. For the usage and hybrid models, the AEI data reflects tasks that workers have actively chosen to use AI for—revealed adoption is evidence that the feasibility threshold has been crossed. Applying φ = 0.23 on top of usage would double-discount. I set φ = 1 for these models.</p>
  <p><strong>π̄ (average labor cost saving).</strong> Acemoglu (2024) uses 0.27, averaged from Noy and Zhang (2023) at approximately 0.40 (professional writing) and Brynjolfsson, Li, and Raymond (2023) at approximately 0.14 (customer service). I hold π̄ = 0.27 as the baseline across all models for comparability, and separately report sensitivity to alternative values in Table 2. The direction of potential bias for the usage model is noted: if usage is software-development-heavy, the appropriate π̄ is likely higher than 0.27, which would increase the usage TFP estimate but not close the gap with the exposure baseline.</p>
  <p><strong>Index construction.</strong> Exposure: occupation-level AI susceptibility from Eloundou, Manning, Mishkin, and Rock (2023), aggregated to 6-digit SOC; missing occupations receive zero. Usage: <code>aei_usage_pct / 100</code> applied directly; occupations not in AEI receive zero. Hybrid: usage if available in AEI, else exposure; missing in both receive zero. GDP-weighted share: <code>Σ(index_i × wagebill_share_i)</code>.</p>

  <h3>D. Limitations</h3>
  <ul>
    <li><strong>Platform selection.</strong> AEI captures Claude interactions only. Usage of GPT-4, Gemini, Copilot, and open-source models is unobserved. If cross-platform usage is correlated in its occupational distribution, relative rankings may be stable but absolute levels of s̄<sub>A</sub> are understated.</li>
    <li><strong>Coverage gap.</strong> AEI covers 608 of approximately 800 detailed SOC occupations. Uncovered occupations receive zero in the usage model and the exposure value in the hybrid. The zero imputation is conservative; the exposure fill is optimistic.</li>
    <li><strong>π̄ task-mix mismatch.</strong> The baseline π̄ = 0.27 was estimated from writing and customer-service experiments. Usage is concentrated in software development, for which Peng, Kalliamvakou, Cihon, and Demirer (2023) report higher gains. Table 2 makes this sensitivity transparent.</li>
    <li><strong>Temporal snapshot.</strong> Exposure reflects AI capabilities circa 2023; AEI reflects usage through late 2025. Diffusion dynamics—how s̄<sub>A</sub> under usage evolves as adoption broadens—are unobserved and are arguably the most economically important variable going forward.</li>
  </ul>

  <h3>E. Full Results</h3>
  <div class="table-wrap">
    <p class="table-caption">Table A1 &mdash; All computed quantities by index (π̄ = 0.27)</p>
    <table>
      <thead>
        <tr>
          <th>Quantity</th>
          <th>Exposure</th>
          <th>Usage (φ=1)</th>
          <th>Hybrid (φ=1)</th>
        </tr>
      </thead>
      <tbody>
        <tr><td>GDP-weighted share (s&#772;<sub>A</sub>)</td><td>18.70%</td><td>0.25%</td><td>1.47%</td></tr>
        <tr><td>Feasibility parameter (&phi;)</td><td>0.23</td><td>1</td><td>1</td></tr>
        <tr><td>Feasible share (s&#772;<sub>A</sub> &times; &phi;)</td><td>4.30%</td><td>0.25%</td><td>1.47%</td></tr>
        <tr><td>Labor share, AI-affected industries (s<sub>L</sub>)</td><td>53.51%</td><td>57.63%</td><td>58.72%</td></tr>
        <tr><td>TFP gain, 10 years (π̄ = 0.27)</td><td>0.62%</td><td>0.04%</td><td>0.23%</td></tr>
        <tr><td>TFP gain, 10 years (π̄ = 0.55, Peng, Kalliamvakou, Cihon, and Demirer 2023)</td><td>—</td><td>0.08%</td><td>0.47%</td></tr>
        <tr><td>Implied annual TFP growth (π̄ = 0.27)</td><td>0.062%/yr</td><td>0.004%/yr</td><td>0.023%/yr</td></tr>
      </tbody>
    </table>
  </div>

  <h3>F. References</h3>
  <ul>
    <li>Acemoglu, D. (2024). <em>The Simple Macroeconomics of AI.</em> Economic Policy.</li>
    <li>Anthropic (2025). <em>Anthropic Economic Index.</em> September 2025 release.</li>
    <li>Brynjolfsson, E., D. Li, and L. R. Raymond (2023). "Generative AI at work." <em>NBER WP</em> 31161.</li>
    <li>Dell'Acqua, F., et al. (2023). "Navigating the jagged technological frontier." <em>Harvard Business School WP</em> 24-013.</li>
    <li>Eloundou, T., S. Manning, P. Mishkin, and D. Rock (2023). "GPTs are GPTs." <em>NBER WP</em> 31255.</li>
    <li>Hulten, C. R. (1978). "Growth accounting with intermediate inputs." <em>Review of Economic Studies</em>, 45(3).</li>
    <li>Noy, S., and W. Zhang (2023). "Experimental evidence on the productivity effects of generative AI." <em>Science</em>, 381(6654).</li>
    <li>Peng, S., E. Kalliamvakou, P. Cihon, and M. Demirer (2023). "The impact of AI on developer productivity: Evidence from GitHub Copilot." <em>arXiv</em> 2302.06590.</li>
    <li>Svanberg, M., et al. (2024). Computer vision automation feasibility study. Referenced in Acemoglu (2024).</li>
  </ul>

</div>
</section>

<footer>
  Shisham Adhikari <span class="dot">&middot;</span> March 2026 <span class="dot">&middot;</span> AI &amp; Labor Markets
</footer>

</body>
</html>
