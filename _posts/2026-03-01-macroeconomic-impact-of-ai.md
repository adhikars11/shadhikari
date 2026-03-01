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
      padding: 1rem 1.5rem;
      font-family: var(--mono);
      font-size: 0.88rem;
      color: var(--ink);
      text-align: center;
      margin: 1.5rem 0 2rem;
      letter-spacing: 0.03em;
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
  <p class="subtitle">Replacing theoretical exposure with observed usage collapses the 10-year TFP estimate from 0.62% to 0.01%—a 60&times; gap that tells us exactly where we are in the AI diffusion cycle.</p>
  <p class="meta">Shisham Adhikari <span>&middot;</span> March 1, 2026</p>
</section>

<main>
<div class="container">

  <div class="takeaways-wrap">
    <div class="takeaways">
      <span class="kicker">Key Takeaways</span>
      <ul>
        <li><strong>Exposure ≠ Usage.</strong> The exposure index (Acemoglu 2024) assigns 18.7% of the GDP-weighted wage bill to AI-susceptible occupations. Replacing it with actual Claude usage data shrinks that to 0.25%—a 75&times; gap between AI's potential reach and current reality.</li>
        <li><strong>TFP estimates collapse under usage.</strong> Using Hulten's theorem: Exposure → 0.62% TFP over 10 years; Usage → 0.01%; Hybrid (usage where observed, exposure elsewhere) → 0.05%.</li>
        <li><strong>Labor cost weights matter.</strong> Exposed occupations carry a 53.5% labor share of income; usage-heavy occupations (concentrated in tech/professional services) carry 57.6%. The composition shift is small—the GDP-weighted scope is everything.</li>
        <li><strong>The gap is the finding.</strong> Current usage is overwhelmingly concentrated in software and professional services. Broad diffusion hasn't happened yet. The 75&times; shortfall is a snapshot of early adoption, not a ceiling.</li>
      </ul>
    </div>
  </div>

  <div class="prose">

    <h2>Motivation</h2>

    <p>Macroeconomists have become increasingly interested in AI's aggregate economic impact—but most forecasts rely on informal extrapolation rather than a disciplined bottom-up framework. The challenge: to go from task-level productivity gains to economy-wide TFP, you need a model of how individual task improvements aggregate across thousands of interdependent occupations and industries.</p>

    <p>Acemoglu (2024) provides exactly this: a task-based production model that yields a clean, empirically implementable formula for AI's TFP effect. This post replicates that calculation and then asks a sharper question—what happens when we replace the theoretical exposure index with observed AI usage data from Anthropic's Economic Index (AEI)?</p>

    <h2>The Task Framework</h2>

    <p>Modern automation models treat output as a combination of many distinct tasks—each potentially performed by labor or capital. AI shifts the margin: tasks once requiring human judgment become feasible for machines. Two structural features drive the aggregate implications:</p>

    <ul>
      <li><strong>Gross complementarity.</strong> Tasks are complements (σ &lt; 1)—automating one task faster doesn't proportionally raise total output if others remain bottlenecks. This puts a natural ceiling on aggregate gains from partial automation.</li>
      <li><strong>Heterogeneous exposure.</strong> Not all tasks are equally susceptible. Exposure is highest in routine cognitive work (coding, drafting, classification); lowest in physical, relational, and complex judgment tasks.</li>
    </ul>

    <p>The framework's key insight: you don't need a full general equilibrium model to estimate the first-order TFP effect. Hulten's theorem does the aggregation.</p>

    <h2>Hulten's Theorem (for Non-Economists)</h2>

    <p>Hulten's (1978) theorem states that the aggregate TFP impact of a productivity improvement in any sector equals that sector's <strong>share of GDP</strong> times the size of the improvement—regardless of second-order reallocation effects. Applied here:</p>

    <div class="formula">
      <span class="formula-line">TFP gain &asymp; s&#772;<sub>A</sub> &times; &phi; &times; s<sub>L</sub> &times; &pi;&#772;</span>
      <span class="formula-comment">
        s&#772;<sub>A</sub> = GDP-weighted share of AI-exposed labor tasks &nbsp;|&nbsp;
        &phi; = fraction feasibly automated (0.23) &nbsp;|&nbsp;
        s<sub>L</sub> = labor share of income in exposed industries &nbsp;|&nbsp;
        &pi;&#772; = avg. labor cost saving (0.27)
      </span>
    </div>

    <p>The formula has four ingredients. Three are fixed across our comparisons (&phi; = 0.23, s<sub>L</sub> ≈ 0.54–0.59, &pi;&#772; = 0.27). The one that changes is <strong>s&#772;<sub>A</sub></strong>—the GDP-weighted scope of AI activity. That single number swings the TFP estimate by two orders of magnitude depending on whether you use exposure or usage to define it.</p>

    <h2>Results</h2>

    <p>We compare three indices at the 6-digit SOC level, all fed into the same aggregation pipeline:</p>

    <ul>
      <li><strong>Exposure:</strong> per-occupation rate [0,1] from Eloundou et al. (2023), reflecting GPT-4 judgments of O*NET task susceptibility.</li>
      <li><strong>Usage:</strong> AEI share-of-pie—each occupation's fraction of total observed Claude interactions. Sums to 1.0; occupations absent from AEI get zero.</li>
      <li><strong>Hybrid:</strong> usage where AEI covers the occupation; exposure (automation) elsewhere.</li>
    </ul>

    <div class="table-wrap">
      <p class="table-caption">Table 1 &mdash; Aggregate estimates under three index assumptions (&phi; = 0.23, &pi;&#772; = 0.27)</p>
      <table>
        <thead>
          <tr>
            <th>Index</th>
            <th>GDP-Weighted Share (s&#772;<sub>A</sub>)</th>
            <th>Labor Share (s<sub>L</sub>)</th>
            <th>TFP (10-yr)</th>
          </tr>
        </thead>
        <tbody>
          <tr>
            <td>Exposure (Acemoglu baseline)</td>
            <td>18.70%</td>
            <td>53.51%</td>
            <td>0.62%</td>
          </tr>
          <tr class="highlight-row">
            <td>Usage (AEI, missing = 0)</td>
            <td>0.25%</td>
            <td>57.63%</td>
            <td>0.01%</td>
          </tr>
          <tr>
            <td>Hybrid (usage + exposure fill)</td>
            <td>1.47%</td>
            <td>58.72%</td>
            <td>0.05%</td>
          </tr>
        </tbody>
      </table>
    </div>

    <p>The labor share of exposed industries is slightly <em>higher</em> under usage (57.6%) than exposure (53.5%), because observed usage concentrates in professional services—a more labor-intensive sector than the broader exposed task pool. But this composition shift is a rounding error relative to the 75&times; collapse in s&#772;<sub>A</sub>, which drives TFP from 0.62% to 0.01%.</p>

    <p>The hybrid—granting full exposure credit to unobserved occupations—reaches only 1.47% GDP-weighted share and 0.05% TFP. Even the most generous benchmark is 12&times; below the exposure baseline.</p>

    <blockquote class="pullquote">
      <p>The 75&times; gap between exposure and usage is not a measurement artifact. It is a precise description of how early we are in the diffusion cycle.</p>
    </blockquote>

    <h2>Conclusion</h2>

    <p>Acemoglu's task-based framework is the right structure for this calculation. The debate should be about inputs, not the formula. And on inputs, the choice of index is decisive:</p>

    <ul>
      <li>Exposure measures AI's technological <em>potential</em>—broad, optimistic, and ahead of realized adoption.</li>
      <li>Usage measures where AI is <em>actually deployed</em> today—narrow, concentrated in tech and professional services, and honest about the diffusion gap.</li>
      <li>The 75&times; shortfall between them is the adoption work still ahead. As diffusion broadens, s&#772;<sub>A</sub> will grow—and with it, the macro impact. Tracking that convergence is the empirical question that matters most going forward.</li>
    </ul>

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
    <li><strong>Exposure index:</strong> Acemoglu (2024) via Eloundou et al. (2023). GPT-4 annotations of O*NET work activities aggregated to 6-digit SOC. 798 occupations; GDP-weighted using BLS OEWS (2019–2024).</li>
    <li><strong>AEI usage index:</strong> Anthropic Economic Index, September 2025. <code>aei_usage_pct / 100</code>, sums to 1.0 across 608 SOC codes. Used raw (no rescaling).</li>
    <li><strong>Wage &amp; employment:</strong> BLS OEWS national estimates, 2019–2024.</li>
    <li><strong>Industry labor shares:</strong> BEA NIPA industry accounts, averaged 2018–2022, matched via NAICS crosswalk.</li>
  </ul>

  <h3>C. Index Construction</h3>
  <p><strong>Exposure:</strong> per-occupation rate in [0,1]; missing = 0. <strong>Usage:</strong> <code>aei_usage_pct / 100</code> directly—a share-of-pie, not per-occupation rate; missing = 0. <strong>Hybrid:</strong> usage if available in AEI, else exposure. GDP-weighted share: <code>Σ(index_i × wagebill_share_i)</code>.</p>

  <h3>D. Limitations</h3>
  <ul>
    <li><strong>Platform selection.</strong> AEI captures Claude only. Usage of GPT-4, Gemini, Copilot is unobserved; cross-platform correlation is assumed but unverified.</li>
    <li><strong>Coverage gap.</strong> AEI covers 608 of ~800 SOC occupations. Zero imputation for missing occupations is conservative.</li>
    <li><strong>Scale mismatch.</strong> Exposure is a per-occupation rate; usage is a relative share. The two measure different things (potential vs. realized concentration) and should not be directly compared as levels.</li>
    <li><strong>Snapshot.</strong> Exposure reflects AI capabilities circa 2023; usage reflects AEI through late 2025. Diffusion speed—arguably the most important variable—is unobserved.</li>
  </ul>

  <h3>E. Full Results</h3>
  <div class="table-wrap">
    <p class="table-caption">Table A1 &mdash; All computed quantities by index</p>
    <table>
      <thead>
        <tr>
          <th>Quantity</th>
          <th>Exposure</th>
          <th>Usage</th>
          <th>Hybrid</th>
        </tr>
      </thead>
      <tbody>
        <tr><td>GDP-weighted share (s&#772;<sub>A</sub>)</td><td>18.70%</td><td>0.25%</td><td>1.47%</td></tr>
        <tr><td>Feasible share (s&#772;<sub>A</sub> &times; &phi;)</td><td>4.30%</td><td>0.06%</td><td>0.34%</td></tr>
        <tr><td>Labor share, exposed industries (s<sub>L</sub>)</td><td>53.51%</td><td>57.63%</td><td>58.72%</td></tr>
        <tr><td>TFP gain over 10 years</td><td>0.62%</td><td>0.01%</td><td>0.05%</td></tr>
        <tr><td>Implied annual TFP growth</td><td>0.062%/yr</td><td>0.001%/yr</td><td>0.005%/yr</td></tr>
      </tbody>
    </table>
  </div>
  <p>Fixed parameters across all three variants: &phi; = 0.23 (Svanberg et al. 2024), &pi;&#772; = 0.27 (Noy &amp; Zhang 2023; Brynjolfsson et al. 2023).</p>

  <h3>F. References</h3>
  <ul>
    <li>Acemoglu, D. (2024). <em>The Simple Macroeconomics of AI.</em> Economic Policy.</li>
    <li>Anthropic (2025). <em>Anthropic Economic Index.</em> September 2025 release.</li>
    <li>Brynjolfsson, E., D. Li, and L. R. Raymond (2023). "Generative AI at work." <em>NBER WP</em> 31161.</li>
    <li>Eloundou, T., S. Manning, P. Mishkin, and D. Rock (2023). "GPTs are GPTs." <em>NBER WP</em> 31255.</li>
    <li>Hulten, C. R. (1978). "Growth accounting with intermediate inputs." <em>Review of Economic Studies</em>, 45(3).</li>
    <li>Noy, S., and W. Zhang (2023). "Experimental evidence on the productivity effects of generative AI." <em>Science</em>, 381(6654).</li>
    <li>Svanberg, M., et al. (2024). Computer vision automation feasibility study. Referenced in Acemoglu (2024).</li>
  </ul>

</div>
</section>

<footer>
  Shisham Adhikari <span class="dot">&middot;</span> March 2026 <span class="dot">&middot;</span> AI &amp; Labor Markets
</footer>

</body>
</html>
