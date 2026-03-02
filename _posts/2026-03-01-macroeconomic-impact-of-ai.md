---
layout: none
title: 'The AI Productivity Gap: Why Exposure and Usage Estimates Diverge'
date: 2026-03-01
permalink: /posts/2026/03/macroeconomic-impact-ai/
---
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>The AI Productivity Gap: Why Exposure and Usage Estimates Diverge</title>
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
    body { font-family: 'DM Sans', system-ui, sans-serif; background: var(--bg); color: var(--ink); line-height: 1.75; }
    .topbar { background: var(--accent); height: 4px; }

    .site-header { padding: 1.1rem 2rem; display: flex; align-items: center; justify-content: space-between; border-bottom: 1px solid var(--rule); background: var(--bg); }
    .site-header .wordmark { font-family: 'DM Serif Display', serif; font-size: 1rem; color: var(--ink-muted); letter-spacing: 0.01em; }
    .site-header .section-label { font-size: 0.62rem; font-weight: 500; letter-spacing: 0.16em; text-transform: uppercase; color: var(--accent); font-family: var(--mono); }

    .hero { background: var(--surface); border-bottom: 1px solid var(--rule); padding: 4.5rem 2rem 4rem; text-align: center; }
    .hero .topic-tag { display: inline-block; font-family: var(--mono); font-size: 0.62rem; letter-spacing: 0.2em; text-transform: uppercase; color: var(--accent); border: 1px solid var(--accent-mid); padding: 0.22em 0.9em; border-radius: 2px; margin-bottom: 1.5rem; background: var(--accent-light); }
    .hero h1 { font-family: 'DM Serif Display', serif; font-size: clamp(2rem, 4.5vw, 3.2rem); font-weight: 400; line-height: 1.18; max-width: 780px; margin: 0 auto 1.2rem; color: var(--ink); letter-spacing: -0.02em; }
    .hero .subtitle { font-size: 1.05rem; font-weight: 300; color: var(--ink-mid); max-width: 640px; margin: 0 auto 2.25rem; line-height: 1.65; }
    .hero .meta { font-family: var(--mono); font-size: 0.68rem; color: var(--ink-muted); letter-spacing: 0.07em; }
    .hero .meta span { margin: 0 0.5em; color: var(--accent-mid); }

    .container { max-width: 780px; margin: 0 auto; padding: 0 1.5rem; }

    .takeaways-wrap { padding: 3rem 0 0; }
    .takeaways { background: var(--accent-light); border: 1px solid var(--accent-mid); border-left: 4px solid var(--accent); border-radius: 0 6px 6px 0; padding: 1.75rem 2.25rem; }
    .takeaways .kicker { font-family: var(--mono); font-size: 0.62rem; letter-spacing: 0.2em; text-transform: uppercase; color: var(--accent); margin-bottom: 1rem; display: block; }
    .takeaways ul { padding-left: 1.2rem; list-style: disc; }
    .takeaways li { margin-bottom: 0.55rem; font-size: 0.95rem; color: var(--ink); line-height: 1.55; }
    .takeaways li:last-child { margin-bottom: 0; }
    .takeaways li strong { font-weight: 600; }

    .prose { padding: 2.75rem 0 3rem; }
    .prose h2 { font-family: 'DM Serif Display', serif; font-size: 1.6rem; font-weight: 400; color: var(--ink); margin: 3.25rem 0 1rem; padding-top: 2rem; border-top: 1px solid var(--rule); letter-spacing: -0.01em; line-height: 1.25; }
    .prose h2:first-child { margin-top: 0; padding-top: 0; border-top: none; }
    .prose h3 { font-family: var(--mono); font-size: 0.68rem; letter-spacing: 0.16em; text-transform: uppercase; color: var(--accent); margin: 2.5rem 0 0.85rem; }
    .prose p { margin-bottom: 1.3rem; font-size: 1rem; font-weight: 300; color: var(--ink-mid); line-height: 1.8; }
    .prose p strong { color: var(--ink); font-weight: 500; }
    .prose ul { padding-left: 1.4rem; margin-bottom: 1.3rem; }
    .prose ul li { font-size: 1rem; font-weight: 300; color: var(--ink-mid); line-height: 1.7; margin-bottom: 0.5rem; }
    .prose ul li strong { color: var(--ink); font-weight: 500; }

    .formula { background: var(--surface); border: 1px solid var(--rule); border-radius: 6px; padding: 0.85rem 1.25rem; font-family: var(--mono); font-size: 0.8rem; color: var(--ink); margin: 1.5rem 0 2rem; letter-spacing: 0.01em; overflow-x: auto; }
    .formula .formula-line { display: block; margin-bottom: 0.4rem; }
    .formula .formula-line:last-child { margin-bottom: 0; }
    .formula .formula-label { display: inline-block; width: 11rem; color: var(--ink-muted); font-size: 0.75rem; }
    .formula .formula-comment { display: block; font-size: 0.72rem; color: var(--ink-muted); letter-spacing: 0.04em; margin-top: 0.65rem; border-top: 1px solid var(--rule); padding-top: 0.55rem; }

    .table-wrap { margin: 2rem 0; overflow-x: auto; }
    .table-caption { font-family: var(--mono); font-size: 0.62rem; letter-spacing: 0.12em; text-transform: uppercase; color: var(--ink-muted); margin-bottom: 0.6rem; }
    table { width: 100%; border-collapse: collapse; font-size: 0.88rem; }
    thead tr { background: var(--ink); }
    thead th { font-family: var(--mono); font-size: 0.62rem; letter-spacing: 0.1em; text-transform: uppercase; padding: 0.75rem 1rem; text-align: left; font-weight: 500; color: #f5f4f0; }
    tbody tr:nth-child(even) { background: var(--surface); }
    tbody tr:hover { background: var(--accent-light); transition: background 0.15s; }
    tbody td { padding: 0.65rem 1rem; border-bottom: 1px solid var(--rule); color: var(--ink-mid); font-weight: 300; }
    tbody td:first-child { color: var(--ink); font-weight: 400; }
    .highlight-row td { background: var(--accent-light) !important; color: var(--ink) !important; font-weight: 400 !important; }
    .section-row td { background: var(--surface) !important; font-family: var(--mono); font-size: 0.6rem; letter-spacing: 0.12em; text-transform: uppercase; color: var(--ink-muted) !important; padding: 0.4rem 1rem; font-weight: 500 !important; }

    blockquote.pullquote { margin: 2.75rem 0; padding: 0 0 0 1.5rem; border-left: 3px solid var(--accent); }
    blockquote.pullquote p { font-family: 'DM Serif Display', serif; font-size: 1.2rem; font-style: italic; color: var(--ink); line-height: 1.5; margin: 0; }

    .appendix { background: var(--surface); border-top: 1px solid var(--rule); margin-top: 2rem; padding: 3.5rem 0 4rem; }
    .appendix h2 { font-family: 'DM Serif Display', serif; font-size: 1.45rem; font-weight: 400; color: var(--ink); margin-bottom: 0.4rem; }
    .appendix .app-intro { font-size: 0.92rem; color: var(--ink-muted); font-weight: 300; margin-bottom: 2rem; }
    .appendix h3 { font-family: var(--mono); font-size: 0.65rem; letter-spacing: 0.18em; text-transform: uppercase; color: var(--accent); margin: 2.5rem 0 0.75rem; }
    .appendix p { font-size: 0.9rem; color: var(--ink-mid); font-weight: 300; margin-bottom: 0.85rem; line-height: 1.7; }
    .appendix ul, .appendix ol { padding-left: 1.5rem; margin-bottom: 1rem; }
    .appendix li { font-size: 0.9rem; color: var(--ink-mid); font-weight: 300; margin-bottom: 0.45rem; line-height: 1.65; }
    .appendix strong { color: var(--ink); font-weight: 500; }
    .appendix code { font-family: var(--mono); font-size: 0.8rem; background: var(--bg); border: 1px solid var(--rule); padding: 0.05em 0.35em; border-radius: 3px; color: var(--accent); }
    .appendix table { font-size: 0.85rem; }
    .appendix thead tr { background: #0F2740; }
    .appendix .table-caption { margin-top: 1.5rem; }

    footer { text-align: center; padding: 2rem 1rem 2.5rem; font-family: var(--mono); font-size: 0.62rem; color: var(--ink-muted); letter-spacing: 0.08em; border-top: 1px solid var(--rule); }
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
  <h1>The AI Productivity Gap: Why Exposure and Usage Estimates Diverge</h1>
  <p class="subtitle">Acemoglu (2024) and Anthropic's Economic Index apply the same theorem to the same task taxonomy—and reach estimates 30&times; apart. A parameter-by-parameter breakdown.</p>
  <p class="meta">Shisham Adhikari <span>&middot;</span> March 1, 2026</p>
</section>

<main>
<div class="container">

  <div class="takeaways-wrap">
    <div class="takeaways">
      <span class="kicker">Key Takeaways</span>
      <ul>
        <li><strong>Scope isn't the problem.</strong> Both find AI reaches roughly 18–20% of the wage-bill–weighted task portfolio. That number is not in dispute.</li>
        <li><strong>The gap is almost entirely in one number: speedup.</strong> Controlled experiments find 1.2–1.6&times;. Anthropic's observed usage data finds 9–12&times;. Run those through Hulten's formula and you get estimates 30&times; apart.</li>
        <li><strong>The policy stakes are asymmetric.</strong> If Acemoglu is right, AI is a modest automation episode. If Anthropic's conservative range holds (0.7–1.2 pp/yr), we are in the largest U.S. productivity surge since the late 1990s.</li>
      </ul>
    </div>
  </div>

  <div class="prose">

    <h2>Motivation</h2>

    <p>Productivity growth is the long-run engine of rising living standards. In the United States, labor productivity grew at roughly 2.8% per year from 1995 to 2004—driven by the IT boom—and has averaged barely 1.4% since. AI reopens the question of whether a new general-purpose technology can break that trend. Reasonable people disagree—not just on values or politics, but empirically. The best available estimates of AI's aggregate impact are separated by an order of magnitude.</p>

    <p>The two most careful answers come from opposite ends of the research ecosystem. Acemoglu (2024)—whose task-based framework partly underpins his 2024 Nobel Prize in Economics—estimates AI adds 0.06 percentage points per year to labor productivity. Anthropic's January 2026 Economic Index (Appel et al., 2026), built on a year of real Claude.ai usage data, estimates 1.0–1.8 pp/yr. Both work from the same theoretical scaffold—tasks as the unit of analysis, Hulten's theorem as the aggregator, O*NET as the task taxonomy—and reach very different conclusions. This post traces exactly where they part ways.</p>

    <h2>The Task-Based Framework</h2>

    <p>Think of the economy as a collection of tasks—writing, coding, analyzing, building, advising—each performed by workers or machines. AI expands what machines can do, shifting some of those tasks away from human labor. But how much that shift matters for the broader economy depends on two things.</p>

    <p>First, tasks are complements, not substitutes. Automating one step in a process doesn't multiply output if other steps remain bottlenecks. A lawyer who drafts twice as fast still needs client meetings, review cycles, and court dates. This places a natural ceiling on how much partial automation can lift aggregate output. Second, AI doesn't affect all tasks equally. Its reach is greatest in routine cognitive work—coding, drafting, classification—and weakest in tasks requiring physical presence, interpersonal judgment, or contextual reasoning.</p>

    <h2>Hulten's Theorem</h2>

    <p>To translate task-level gains into an economy-wide number, Hulten's (1978) theorem says the aggregate productivity impact of an improvement equals that sector's wage-bill share times the log size of the improvement. Applied to AI:</p>

    <div class="formula">
      <span class="formula-line">TFP gain &asymp; task scope &times; feasibility &times; labor share &times; productivity gain per task</span>
      <span class="formula-line" style="color: var(--ink-muted); font-size: 0.8rem;">&asymp; s&#772;<sub>A</sub> &nbsp;&times;&nbsp; &phi; &nbsp;&times;&nbsp; s<sub>L</sub> &nbsp;&times;&nbsp; &pi;&#772;</span>
      <span class="formula-comment">
        s&#772;<sub>A</sub>&thinsp;= wage-bill–weighted share of AI-capable tasks &nbsp;|&nbsp;
        &phi;&thinsp;= fraction of capable tasks that are cost-effective &nbsp;|&nbsp;
        s<sub>L</sub>&thinsp;= labor income share (&asymp;0.65) &nbsp;|&nbsp;
        &pi;&#772;&thinsp;= average fraction of task time saved
      </span>
    </div>

    <p>Acemoglu applies this formula directly. Anthropic applies a more general form—summing log speedups at the task level rather than using the linearized &pi;&#772;—which is mathematically equivalent for small speedups but materially different for large ones. At a 10&times; speedup, the linearized &pi;&nbsp;=&nbsp;0.9, while log(10)&nbsp;&asymp;&nbsp;2.3. Both approaches use the same theorem; they diverge on what gets plugged in.</p>

    <h2>Same Theorem, Different Inputs</h2>

    <h3>Task scope — not the disagreement</h3>

    <p>Acemoglu measures scope as the wage-bill–weighted share of O*NET tasks GPT-4 is capable of performing—a potential exposure measure. This puts roughly 18–19% of wage-bill–weighted labor in AI-capable tasks. Anthropic measures scope as the share of tasks workers actually bring to Claude (requiring at least 200 observations for stability). That also lands at roughly 18–20%. Two independent methods, measuring potential versus actual reach, arrive at nearly the same number. Scope is not the source of disagreement.</p>

    <h3>Gain per task — where the gap lives</h3>

    <p><strong>Acemoglu's &pi;&#772;&nbsp;=&nbsp;0.27</strong> averages two controlled experiments. Noy and Zhang (2023) found professional writers were 40% faster with GPT-4 (speedup &asymp;&nbsp;1.6&times;); Brynjolfsson et al. (2023) found a 14% gain for customer-service workers with an AI tool (speedup &asymp;&nbsp;1.16&times;). The midpoint: &pi;&#772;&nbsp;=&nbsp;0.27, or an effective log-speedup of about 0.31.</p>

    <p><strong>Anthropic's speedups are measured differently—and are far larger.</strong> For each task in Claude usage, Claude estimates (i) hours a professional would need <em>without</em> AI and (ii) minutes spent completing the task <em>with</em> Claude. Speedup = human-alone time ÷ human-with-AI time. Anthropic reports 9&times; for high-school-level tasks and 12&times; for college-level tasks—a mean log-speedup of roughly 2.3–2.5. That difference, run through Hulten's formula over a similar wage-bill share, produces almost the entire gap in headline estimates.</p>

    <h3>Feasibility — a secondary driver</h3>

    <p>Acemoglu applies &phi;&nbsp;=&nbsp;0.23: even where AI is capable, only about a quarter of those tasks are currently cost-effective at prevailing wages and AI prices. Anthropic applies no explicit filter—if workers are completing tasks with Claude, the cost-effectiveness threshold has already been crossed. When Anthropic's analysts multiply each log-speedup by the task-specific success rate and then account for task complementarity (&sigma;&nbsp;=&nbsp;0.5), the estimate narrows from 1.8 to 0.7–1.2&nbsp;pp/yr.</p>

    <h2>The Numbers Side by Side</h2>

    <div class="table-wrap">
      <p class="table-caption">Table 1 &mdash; Key inputs and results</p>
      <table>
        <thead>
          <tr>
            <th>Parameter</th>
            <th>Acemoglu (2024)</th>
            <th>Anthropic AEI (Jan 2026)</th>
          </tr>
        </thead>
        <tbody>
          <tr>
            <td>Task scope (wage-bill weight)</td>
            <td>&sim;18–19% — GPT-4 exposure of O*NET tasks</td>
            <td>&sim;18–20% — observed Claude usage, &ge;200 obs.</td>
          </tr>
          <tr>
            <td>Speedup data source</td>
            <td>Randomized experiments, GPT-4, 2022–23</td>
            <td>Observed Claude conversations, Nov 2025</td>
          </tr>
          <tr>
            <td>Observed speedup range</td>
            <td>1.16&times; – 1.59&times;</td>
            <td>9&times; – 12&times;</td>
          </tr>
          <tr>
            <td>Gain parameter</td>
            <td>&pi;&#772;&nbsp;=&nbsp;0.27 &nbsp;(log-speedup &asymp; 0.31)</td>
            <td>log(speedup<sub>t</sub>) per task &asymp; 2.3–2.5</td>
          </tr>
          <tr>
            <td>Feasibility filter</td>
            <td>&phi;&nbsp;=&nbsp;0.23 (cost-effective tasks only)</td>
            <td>None — usage = revealed feasibility</td>
          </tr>
          <tr class="highlight-row">
            <td>Baseline / adjusted estimate</td>
            <td>0.62% over 10 yr &nbsp;(0.06 pp/yr)</td>
            <td>1.8 pp/yr baseline &rarr; 0.7–1.2 pp/yr adjusted</td>
          </tr>
        </tbody>
      </table>
    </div>

    <blockquote class="pullquote">
      <p>Both approaches agree AI covers a similar slice of the economy's task portfolio. The entire spread comes from one place: how fast AI speeds up the tasks it reaches.</p>
    </blockquote>

    <h2>Why Are the Speedups So Different?</h2>

    <p>Three explanations are plausible, and they aren't mutually exclusive. First, <strong>selection</strong>: workers bring tasks to Claude where they expect success. If users self-select the easiest fits, observed speedups reflect the best of the distribution, not the full one. Controlled experiments avoid this by assigning tasks randomly. Second, <strong>self-assessment bias</strong>: Anthropic's speedup estimates come from asking Claude to judge how long tasks take with and without AI—a novel approach with no precedent in the experimental literature. An AI evaluating its own productivity gain may be optimistic. Anthropic validates against external benchmarks where possible, but direct calibration against controlled trials remains limited.</p>

    <p>Third—and perhaps most important—<strong>genuine model improvement</strong>. Acemoglu's framework was calibrated on GPT-3/4-era experiments from 2022–2023. Anthropic's data reflects Claude usage in late 2025. If frontier capabilities have improved substantially in two to three years—which most benchmarks suggest they have—the speedup gap may partly be real, not artifactual. The right test would be randomized experiments on current frontier models, using the same task categories that appear in actual usage data. That evidence does not yet exist.</p>

    <h2>Conclusion</h2>

    <p>Two careful, task-based analyses—same theorem, same taxonomy—produce estimates 30&times; apart. The theorem is not in dispute. Scope is not in dispute. The gap sits almost entirely in how fast AI completes tasks once it reaches them: a log-speedup of 0.3 versus 2.3.</p>

    <p>The policy implications hinge entirely on which is right. If Acemoglu is correct, AI's economic disruption is real but measured—comparable in pace to earlier automation waves, manageable with existing workforce policy tools. If Anthropic's conservative range (0.7–1.2 pp/yr) is correct, the U.S. economy is in the early stages of a productivity acceleration that would rival the full IT revolution of the 1990s compressed into a few years—and the standard policy toolkit would be undersized by an order of magnitude.</p>

    <p>The most important thing the two estimates agree on: scope is not the binding constraint. AI already reaches deep into the economy's task portfolio. The open question—entirely—is what it does when it gets there. Settling that question requires the study that doesn't yet exist: a large-scale randomized experiment on current frontier models, across the full distribution of tasks workers actually bring to AI. Until then, the gap between these two estimates is itself the most informative data point we have.</p>

  </div>

</div><!-- /container -->
</main>

<section class="appendix">
<div class="container">

  <h2>Appendix</h2>
  <p class="app-intro">Technical notes on methodology, data sources, and the earlier Sep 2025 usage-concentration exercise.</p>

  <h3>A. Hulten's Theorem and the Two Formulas</h3>
  <p>Hulten (1978) states that the TFP impact of a productivity improvement in a sector equals that sector's GDP share times the log size of the improvement: <code>d log TFP = revenue_share &times; d log A</code>. Applied at the task level, this gives the aggregate labor productivity gain as the wage-bill–weighted sum of log speedups across all AI-affected tasks.</p>
  <p>Acemoglu (2024) uses a linearized version of this for small productivity gains: replacing <code>log(speedup)</code> with <code>&pi;&#772;</code> (fraction of task time saved), and incorporating feasibility (&phi;) and labor income share (s<sub>L</sub>) to yield <code>&Delta;log Y &asymp; s&#772;<sub>A</sub> &times; &phi; &times; s<sub>L</sub> &times; &pi;&#772;</code>. This linearization is accurate for small speedups (1.1&ndash;1.6&times;) but understates gains for large speedups (9&ndash;12&times;), where <code>log(speedup)</code> is substantially larger than <code>1 &minus; 1/speedup</code>.</p>
  <p>Anthropic (2026) applies Hulten directly: <code>&Delta;log Y = &Sigma;<sub>t</sub>(task_wb_share<sub>t</sub> &times; log(speedup<sub>t</sub>))</code> for the baseline case (&sigma;&nbsp;=&nbsp;1). For &sigma;&nbsp;&ne;&nbsp;1, they use a CES aggregator within occupations first, then apply Hulten across occupations. Footnote 9 of their report describes this in detail.</p>

  <h3>B. Anthropic's Speedup Measurement</h3>
  <p>For each O*NET task observed in Claude usage, Anthropic asks Claude to estimate: (i) how many <em>hours</em> a competent professional would need to complete the task <em>without</em> AI (human-only time), and (ii) how many <em>minutes</em> the user spent completing it <em>with</em> Claude (human-with-AI time). Speedup is then:</p>
  <p style="font-family: var(--mono); font-size: 0.82rem; padding: 0.5rem 1rem; background: var(--surface); border: 1px solid var(--rule); border-radius: 4px; margin-bottom: 1rem;">
    speedup = (human-only time &times; 60) / human-with-AI time
  </p>
  <p>A task taking 1 hour alone and 10 minutes with AI gives a speedup of 6&times;. This is confirmed by Anthropic directly in their report: "reducing a 1 hour task to 10 minutes would give a 6x speedup." Across the tasks in their January 2026 data with at least 200 observations, the mean speedup is in the range of 9&ndash;12&times; depending on task complexity. The threshold of 200 observations is chosen to replicate their earlier results and to avoid inflating the aggregate by including very rare tasks with noisy speedup estimates. Without the threshold, the implied productivity gain would be around 5 pp/yr—much higher than their headline figure.</p>

  <h3>C. The Sep 2025 AEI Usage-Concentration Exercise</h3>
  <p>An earlier version of this analysis used the September 2025 AEI release, which reports <code>aei_usage_pct</code>: each O*NET task's share of total Claude interactions summing to 100%. This is a <em>concentration</em> measure, not an intensity measure—it records market share, not per-occupation task penetration. When aggregated to the occupation level and plugged into Hulten's s&#772;<sub>A</sub> slot, the result is a GDP-weighted share of about 0.25%, roughly 75 times smaller than the exposure index. The resulting TFP estimate of 0.04% reflects the structural mismatch between a concentration measure and an intensity slot, not any substantive finding about AI's economic impact. The January 2026 release resolves this by providing task-level speedup data that can be properly aggregated.</p>

  <h3>D. Data Sources</h3>
  <ul>
    <li><strong>Exposure index:</strong> Eloundou, Manning, Mishkin, and Rock (2023), via Acemoglu (2024). GPT-4 annotations of O*NET work activities, aggregated to 6-digit SOC. GDP-weighted using BLS OEWS 2019&ndash;2024.</li>
    <li><strong>AEI speedup data:</strong> Anthropic Economic Index, January 2026 release (Appel, Massenkoff, McCrory et al., 2026). Raw data available at the AEI Hugging Face repository. 3,169 O*NET tasks with speedup estimates in the Claude.ai global sample.</li>
    <li><strong>Wage &amp; employment:</strong> BLS OEWS national estimates, 2019&ndash;2024.</li>
    <li><strong>Industry labor shares:</strong> BEA NIPA industry accounts, averaged 2018&ndash;2022.</li>
  </ul>

  <h3>E. References</h3>
  <ul>
    <li>Acemoglu, D. (2024). "The Simple Macroeconomics of AI." <em>Economic Policy</em>.</li>
    <li>Appel, R., M. Massenkoff, P. McCrory, M. McCain, R. Heller, T. Neylon, and A. Tamkin (2026). <em>Anthropic Economic Index: Economic Primitives.</em> Anthropic, January 15, 2026.</li>
    <li>Brynjolfsson, E., D. Li, and L. R. Raymond (2023). "Generative AI at work." <em>NBER Working Paper</em> 31161.</li>
    <li>Eloundou, T., S. Manning, P. Mishkin, and D. Rock (2023). "GPTs are GPTs: An early look at the labor market impact potential of large language models." <em>NBER Working Paper</em> 31255.</li>
    <li>Hulten, C. R. (1978). "Growth accounting with intermediate inputs." <em>Review of Economic Studies</em>, 45(3), 511&ndash;518.</li>
    <li>Noy, S., and W. Zhang (2023). "Experimental evidence on the productivity effects of generative artificial intelligence." <em>Science</em>, 381(6654), 187&ndash;192.</li>
    <li>Svanberg, M., et al. (2024). Computer vision automation feasibility study. Referenced in Acemoglu (2024).</li>
  </ul>

</div>
</section>

<footer>
  Shisham Adhikari <span class="dot">&middot;</span> March 2026 <span class="dot">&middot;</span> AI &amp; Labor Markets
</footer>

</body>
</html>
