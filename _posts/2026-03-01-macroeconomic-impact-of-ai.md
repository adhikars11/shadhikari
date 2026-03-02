---
layout: none
title: 'Why Do Two Task-Based AI Productivity Estimates Diverge So Sharply?'
date: 2026-03-01
permalink: /posts/2026/03/macroeconomic-impact-ai/
---
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Why Do Two Task-Based AI Productivity Estimates Diverge So Sharply?</title>
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
  <h1>Why Do Two Task-Based AI Productivity Estimates Diverge So Sharply?</h1>
  <p class="subtitle">Acemoglu (2024) estimates a 0.06&nbsp;pp/yr labor productivity gain from AI. Anthropic's January 2026 Economic Index estimates 1.0&ndash;1.8&nbsp;pp/yr. Both rely on tasks and Hulten's theorem. This post traces exactly where they part ways.</p>
  <p class="meta">Shisham Adhikari <span>&middot;</span> March 1, 2026</p>
</section>

<main>
<div class="container">

  <div class="takeaways-wrap">
    <div class="takeaways">
      <span class="kicker">Key Takeaways</span>
      <ul>
        <li><strong>The scope of AI's reach is similar in both.</strong> Both approaches find that AI covers a meaningful share of occupational tasks, roughly 18–20% of the wage-bill–weighted task portfolio. This is not the source of disagreement.</li>
        <li><strong>The divergence is almost entirely about observed speedups.</strong> Controlled labor-market experiments—the basis for Acemoglu's gain parameter—find AI produces 1.2–1.6&times; speedups. Anthropic's observed real-world usage data shows 9–12&times; speedups for the same types of tasks. That difference, compounded through Hulten's formula, drives most of the gap.</li>
        <li><strong>A secondary driver is the feasibility filter.</strong> Acemoglu applies &phi;&nbsp;=&nbsp;0.23 to account for tasks where AI is capable but not yet cost-effective. Anthropic treats observed usage as evidence of feasibility, applying no such filter. Adjusting for task success rates and task complementarity narrows Anthropic's estimates to 0.6–1.2&nbsp;pp/yr.</li>
      </ul>
    </div>
  </div>

  <div class="prose">

    <h2>Motivation</h2>

    <p>How large is AI's impact on aggregate productivity? The answer depends critically on how you measure it. Two of the most careful attempts to date produce estimates separated by roughly an order of magnitude: Acemoglu (2024)—building on the task-based framework that partly underpins his 2024 Nobel Prize in Economics—implies a 10-year labor productivity gain of roughly 0.6%. Anthropic's January 2026 Economic Index (Appel, Massenkoff, McCrory et al., 2026) estimates 1.0–1.8&nbsp;percentage points of annual labor productivity growth—ten to thirty times larger.</p>

    <p>What makes this divergence interesting is what the two approaches share. Both treat tasks, not occupations or industries, as the right unit of analysis. Both invoke Hulten's theorem to aggregate task-level gains into an economy-wide estimate. Both draw on the same underlying O*NET task taxonomy. And yet they reach very different conclusions. This post traces exactly where they part ways—parameter by parameter, inside the same accounting identity.</p>

    <h2>Hulten's Theorem: A Shared Accounting Identity</h2>

    <p>Think of each job as a bundle of tasks—drafting, coding, advising, diagnosing, filing. AI changes the productivity of some subset of those tasks. Hulten (1978) provides a simple accounting identity for aggregating task-level gains into economy-wide output growth: if a task commands a wage-bill share &omega;<sub>t</sub> and becomes <em>speedup<sub>t</sub></em> times faster to complete, its contribution to aggregate labor productivity is &omega;<sub>t</sub>&nbsp;&times;&nbsp;log(speedup<sub>t</sub>). Sum across all AI-affected tasks and you have the aggregate gain.</p>

    <div class="formula">
      <span class="formula-line"><span class="formula-label">Hulten (general):</span>  &Delta;log Y &asymp; &Sigma;<sub>t</sub> &omega;<sub>t</sub> &times; log( speedup<sub>t</sub> )</span>
      <span class="formula-line" style="margin-top:0.55rem;"><span class="formula-label">Acemoglu (2024):</span>  &Delta;log Y &asymp; s&#772;<sub>A</sub> &times; &phi; &times; s<sub>L</sub> &times; &pi;&#772;</span>
      <span class="formula-line"><span class="formula-label">Anthropic (2026):</span>  &Delta;log Y &asymp; &Sigma;<sub>t</sub> ( task_wb_share<sub>t</sub> &times; log( speedup<sub>t</sub> ) )</span>
      <span class="formula-comment">
        s&#772;<sub>A</sub>&thinsp;= wage-bill–weighted share of AI-capable tasks &nbsp;|&nbsp;
        &phi;&thinsp;= fraction of capable tasks that are cost-effective &nbsp;|&nbsp;
        s<sub>L</sub>&thinsp;= labor income share (&asymp;0.65) &nbsp;|&nbsp;
        &pi;&#772;&thinsp;= average fraction of task time saved &nbsp;|&nbsp;
        speedup<sub>t</sub>&thinsp;= human-alone time / human-with-AI time
      </span>
    </div>

    <p>Anthropic applies the general Hulten identity directly at the task level. Acemoglu uses a linearized version of it: replacing log(speedup) with &pi;&#772; (the fraction of task time saved), and separating out the feasibility filter (&phi;) and labor income share (s<sub>L</sub>) as explicit parameters. The linearization is accurate when speedups are modest—1.1&times; to 1.6&times;—but it substantially understates gains when speedups are large. At a 10&times; speedup, &pi;&nbsp;=&nbsp;1&nbsp;&minus;&nbsp;1/10&nbsp;=&nbsp;0.9, while log(10)&nbsp;&asymp;&nbsp;2.3. These are not the same number.</p>

    <p>This formal difference matters less than what each team plugs into the identity. Both use the same theorem; they diverge on the inputs. Let us go through them one by one.</p>

    <h2>Same Theorem, Different Inputs</h2>

    <h3>Parameter 1: Task scope — surprisingly similar</h3>

    <p>In Acemoglu's formulation, task scope is s&#772;<sub>A</sub>: the wage-bill–weighted share of tasks AI is capable of performing. He constructs this from Eloundou, Manning, Mishkin, and Rock (2023): GPT-4 annotates each O*NET task as AI-capable or not, giving a binary exposure score for every occupation. Aggregated across the wage bill, roughly 18–19% of wage-bill–weighted labor falls in AI-capable tasks.</p>

    <p>Anthropic's scope is defined by what Claude is actually used for: tasks observed in their Claude.ai conversation sample with at least 200 observations. Coverage is similarly concentrated—about 18–20% of wage-bill–weighted tasks appear with meaningful Claude usage. Two independent methods, measuring different things (potential versus actual), land on nearly the same number.</p>

    <p>Task scope is not the source of the disagreement.</p>

    <h3>Parameter 2: Gain per task — where almost all of the gap lives</h3>

    <p>This is the sharpest divergence between the two approaches, and it deserves careful attention.</p>

    <p><strong>Acemoglu's &pi;&#772;&nbsp;=&nbsp;0.27</strong> comes from averaging two controlled experiments. Noy and Zhang (2023) randomized professional writers into GPT-4 access and found output produced roughly 40% faster (&pi;&nbsp;&asymp;&nbsp;0.37, speedup &asymp;&nbsp;1.6&times;). Brynjolfsson, Li, and Raymond (2023) gave a customer-service AI tool to call-center workers and measured a 14% productivity gain (&pi;&nbsp;&asymp;&nbsp;0.14, speedup &asymp;&nbsp;1.16&times;). The midpoint gives &pi;&#772;&nbsp;=&nbsp;0.27. When plugged into Hulten's linearized identity, this acts as the average log(speedup) across all AI-affected tasks.</p>

    <p><strong>Anthropic's task-level speedups</strong> are measured differently—and are much larger. For each task observed in Claude usage, Claude estimates (i) how many <em>hours</em> a competent professional would need to complete it <em>without</em> AI (human-only time), and (ii) how many <em>minutes</em> that same task took <em>with</em> Claude assistance in the actual conversation (human-with-AI time). Speedup is then human-only time (in minutes) divided by human-with-AI time. Anthropic reports average speedups of 9&times; for tasks requiring a high-school level of expertise and 12&times; for tasks requiring a college degree. Across the full distribution, the implied mean task-level saving is around 90% of task time—and log(10)&nbsp;&asymp;&nbsp;2.3, versus Acemoglu's effective log(speedup) &asymp;&nbsp;0.31.</p>

    <p>The magnitude of this difference—roughly six to eight times more gain per task—is the primary driver of the gap in aggregate estimates. Both approaches cover a similar slice of the wage bill. But one inputs log-speedups of 0.2–0.5 and the other inputs log-speedups of 2.2–2.5.</p>

    <h3>Parameter 3: Feasibility — a meaningful secondary driver</h3>

    <p>Acemoglu applies an explicit feasibility filter &phi;&nbsp;=&nbsp;0.23, drawing on Svanberg et al. (2024): even where AI is technically capable, only about a quarter of those tasks are currently cost-effective at prevailing wages and AI subscription prices. This acts as a 4&times; downscale on the scope estimate.</p>

    <p>Anthropic applies no explicit feasibility filter. Their implicit argument: if workers are bringing tasks to Claude and completing them, the cost-effectiveness threshold has already been crossed. Usage is revealed preference. One can argue this is more accurate for estimating current, at-the-margin impact, but it does not generalize to the full set of AI-capable tasks not yet adopted. When Anthropic's analysts adjust for task-level success rates—multiplying each log-speedup by the fraction of attempts Claude actually completes successfully—the estimate falls from 1.8 to 1.0–1.2&nbsp;pp/yr. Accounting further for task complementarity (some tasks AI cannot do become bottlenecks) brings it to 0.7–0.9&nbsp;pp/yr.</p>

    <h2>The Resulting Estimates</h2>

    <div class="table-wrap">
      <p class="table-caption">Table 1 &mdash; Parameter inputs and headline estimates compared</p>
      <table>
        <thead>
          <tr>
            <th>Input</th>
            <th>Acemoglu (2024)</th>
            <th>Anthropic AEI (Jan 2026)</th>
          </tr>
        </thead>
        <tbody>
          <tr class="section-row"><td colspan="3">Scope</td></tr>
          <tr>
            <td>Task scope data source</td>
            <td>GPT-4 capability annotations of O*NET tasks (potential exposure)</td>
            <td>Observed Claude usage; tasks with &ge;200 observations in 1M conversations</td>
          </tr>
          <tr>
            <td>Wage-bill–weighted coverage</td>
            <td>&sim;18–19%</td>
            <td>&sim;18–20%</td>
          </tr>
          <tr class="section-row"><td colspan="3">Task-level productivity gain</td></tr>
          <tr>
            <td>Measurement approach</td>
            <td>Average of controlled experiments: professional writing and customer service</td>
            <td>Observed speedups from Claude conversations: Claude estimates human-alone time (hrs) and human-with-AI time (min) per task</td>
          </tr>
          <tr>
            <td>Observed speedup range</td>
            <td>1.16&times; (customer service) to 1.59&times; (professional writing)</td>
            <td>9&times; (high school tasks) to 12&times; (college-level tasks)</td>
          </tr>
          <tr>
            <td>Gain parameter in formula</td>
            <td>&pi;&#772;&nbsp;=&nbsp;0.27 (fraction of task time saved)</td>
            <td>log(speedup<sub>t</sub>) per task; mean &asymp; 2.3–2.5 (equivalent to &pi;&nbsp;&asymp;&nbsp;0.90)</td>
          </tr>
          <tr class="section-row"><td colspan="3">Feasibility &amp; aggregation</td></tr>
          <tr>
            <td>Feasibility filter</td>
            <td>&phi;&nbsp;=&nbsp;0.23 (Svanberg et al. 2024: cost-effective tasks only)</td>
            <td>None; usage = revealed feasibility</td>
          </tr>
          <tr>
            <td>Success rate adjustment</td>
            <td>Not applied</td>
            <td>Applied: multiplies log(speedup) by task-specific success rate before aggregating</td>
          </tr>
          <tr>
            <td>Aggregation formula</td>
            <td>s&#772;<sub>A</sub> &times; &phi; &times; s<sub>L</sub> &times; &pi;&#772;</td>
            <td>&Sigma;<sub>t</sub>(task_wb_share<sub>t</sub> &times; log(speedup<sub>t</sub>)); CES treatment for task complementarity</td>
          </tr>
          <tr class="section-row"><td colspan="3">Results</td></tr>
          <tr>
            <td>Baseline estimate</td>
            <td>0.62% over 10 years (0.06 pp/yr)</td>
            <td>18% over 10 years (1.8 pp/yr)</td>
          </tr>
          <tr class="highlight-row">
            <td>Conservative / adjusted range</td>
            <td>0.31–0.62% (sensitivity to &pi;&#772; and &phi;)</td>
            <td>7–12% over 10 years (0.7–1.2 pp/yr) — success-adjusted; with task complementarity (&sigma;&nbsp;=&nbsp;0.5)</td>
          </tr>
        </tbody>
      </table>
    </div>

    <p>Anthropic's own sensitivity analysis narrows the range considerably. When task-level speedups are multiplied by task-specific success rates—an important correction, since Claude does not always succeed—implied productivity growth falls from 1.8 to 1.0–1.2&nbsp;pp/yr. When the analysis also accounts for task complementarity (some tasks that AI cannot do become bottlenecks), the estimate falls further to 0.7–0.9&nbsp;pp/yr.</p>

    <blockquote class="pullquote">
      <p>Both approaches agree that AI covers a similar slice of the economy's task portfolio. The entire spread between their estimates comes from two places: how fast AI speeds up tasks, and whether to apply a cost-effectiveness discount to capability.</p>
    </blockquote>

    <h2>Why Are the Speedup Estimates So Different?</h2>

    <p>This is the most important open question in the literature. At least three explanations are plausible, and they are not mutually exclusive.</p>

    <p><strong>Selection into Claude usage.</strong> Workers bring tasks to Claude that they expect it to help with. If users systematically avoid tasks where they expect failure, the observed speedup in Claude data reflects a selected sample—tasks where AI performs well—not the full distribution of tasks AI might encounter in broad deployment. Controlled experiments assign tasks randomly, avoiding this selection. Anthropic acknowledges this directly: "observed success rates reflect not just model capability but also user judgment about what will work."</p>

    <p><strong>Self-assessment bias.</strong> Anthropic's speedup estimates come from asking Claude itself to estimate how long tasks would take with and without AI. This is a novel data source with no precedent in the experimental literature, and it is difficult to benchmark externally. An AI system estimating its own productivity gain may overstate it. Anthropic validates these estimates against external benchmarks where possible, but direct calibration against controlled trials remains limited.</p>

    <p><strong>Genuine model capability differences.</strong> Acemoglu's framework was calibrated primarily on GPT-3/GPT-4-era evidence, mostly from 2022–2023 experiments. Anthropic's data reflects Claude usage in November 2025. If frontier model capabilities have improved substantially in the intervening two to three years—which most benchmarks suggest they have—the speedup difference may partly reflect genuine improvement rather than measurement artifacts. The right comparison may be between today's models and experimental estimates benchmarked on today's models.</p>

    <p>Disentangling these explanations would require controlled experiments on current frontier models, run at scale, using the same task categories that appear in Anthropic's usage data. That evidence does not yet exist.</p>

    <h2>Conclusion</h2>

    <p>Two serious, task-based analyses of AI's aggregate productivity impact—both applying Hulten's theorem, both drawing on O*NET tasks, both run by researchers who have thought carefully about the measurement problem—produce estimates separated by roughly an order of magnitude. That is itself informative. The theorem is not what is in dispute. The data on scope is not what is in dispute. The gap sits almost entirely in one number: how fast AI makes tasks when it reaches them.</p>

    <p>Ask what you would have to believe for each estimate to be right. For Acemoglu's 0.06&nbsp;pp/yr to be correct, you would have to believe that the 9–12&times; speedups Anthropic observes in real usage are systematically biased upward—by selection (users bring only their best-fit tasks to Claude), by self-assessment (Claude overestimates how slow the human-alone baseline would be), or both—and that the 1.2–1.6&times; speedups from 2022–2023 controlled experiments are the right population parameter for the full set of AI-deployable tasks today. For Anthropic's 1.8&nbsp;pp/yr to be correct, you would have to believe the opposite: that controlled experiments dramatically undersample the tasks where AI excels, and that a frontier model in late 2025 is simply much faster, on a much wider range of tasks, than GPT-4 was in a call center in 2023.</p>

    <p>Both are defensible. But they carry very different policy implications. If Acemoglu is right, AI's disruption is real but measured—comparable in pace to earlier waves of automation, affecting perhaps 10–15% of workers substantially over a decade. The policy toolkit of retraining programs and workforce support was designed for disruption at that scale. If Anthropic's central estimate (even after adjusting for success rates and task complementarity: 0.7–1.2&nbsp;pp/yr) is right, we are in the middle of a productivity shock that rivals the full-span IT revolution compressed into a few years. The same policy toolkit would be undersized by an order of magnitude.</p>

    <p>The most pointed observation from this comparison is not which estimate to believe—it is that the central unknown is not scope. AI already reaches deep into the economy's task portfolio: both teams find it covers roughly 18–20% of the wage-bill–weighted task distribution. The question is entirely about what it does when it gets there. The fact that two sophisticated teams, starting from the same theorem and the same task taxonomy, cannot agree on whether that number is 0.3 or 2.3 in log-speedup units is the strongest argument for the one study that does not yet exist: a large-scale randomized experiment, run on current frontier models, covering the full distribution of tasks that actually appear in real AI usage. That study would not resolve everything. But it would tell us whether the right unit of productivity gain is "modest and controlled" or "large and revealed"—and that single distinction is what separates the two worldviews on AI's economic future.</p>

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
