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
  <p class="subtitle">Same theorem, same task taxonomy, estimates roughly 16&times; apart. What Acemoglu (2024) and Anthropic’s Economic Index actually disagree on.</p>
  <p class="meta">Shisham Adhikari <span>&middot;</span> March 1, 2026</p>
</section>

<main>
<div class="container">

  <div class="takeaways-wrap">
    <div class="takeaways">
      <span class="kicker">Key Takeaways</span>
      <ul>
        <li><strong>Scope: agreed.</strong> Both find AI reaches roughly 18–20% of total wages. Not the source of the gap.</li>
        <li><strong>Speedup: not agreed.</strong> Lab experiments find 1.2–1.6×. Real-world usage data shows 9–12×. That single difference drives a huge gap in aggregate impacts.</li>
        <li><strong>Policy stakes: high either way.</strong> At 0.06 percentage points per year (pp/yr), AI is a gradual automation wave. At 0.7–1.2 pp/yr, it is the largest U.S. productivity surge since the 1990s.</li>
      </ul>
    </div>
  </div>

  <div class="prose">

    <h2>Motivation</h2>

<p>What is AI's actual impact on the economy today? It is one of the most important questions in economics right now, and surprisingly hard to answer. Two research teams looked at this same question and got answers roughly 16 times apart. MIT economist Daron Acemoglu estimated AI will add about 0.06 percentage points to annual productivity growth over the next decade. Anthropic's Economic Index, using real-world usage data from Claude, put the number at 0.7 to 1.8 percentage points per year. Same theoretical foundation. Same accounting framework. Very different conclusions.</p>

<p>The gap is not a mistake. It reflects a genuine disagreement about what AI actually does when people use it. This post walks through how each estimate is built, what they agree on, and where they part ways.</p>

    <h2>The Task-Based Framework</h2>

<p><strong>Both methods rest on the same theoretical foundation.</strong> Start with a simple idea: the economy is a bundle of tasks (writing, coding, analyzing, building, advising) performed by people and, increasingly, machines. AI expands what machines can do, shifting some tasks away from human labor. The question is how that shift translates into economy-wide productivity.</p>

<p>Two forces matter. First, tasks are complements, not standalone pieces. Speeding up one step does not raise total output one-for-one if other steps remain bottlenecks. A lawyer who drafts twice as fast still needs client meetings, review cycles, and court dates. That interdependence puts a ceiling on what partial automation can do. Second, AI’s impact is uneven across tasks: it tends to help most with routine cognitive work (drafting, coding, classification) and least where physical presence, interpersonal judgment, or deep context are essential.</p>

    <h2>Hulten's Theorem</h2>

<p>Both teams use the same accounting framework to turn task-level observations into an economy-wide number. The idea is simple: if AI makes a set of tasks faster, the gain in total factor productivity (TFP is the efficiency with which inputs are turned into output, and is often used as a proxy for economy-wide productivity) depends on two things: how large a slice of the economy those tasks represent, and how much faster AI makes them. This framework, known as Hulten’s theorem, can be written as:</p>

<div class="formula" style="padding: 0.55rem 1rem; margin-bottom: 0.65rem;">
  <span class="formula-line">TFP gain &asymp; task scope &times; feasibility &times; labor share &times; productivity gain per task</span>
  <span class="formula-line" style="color: var(--ink-muted); font-size: 0.8rem;">&asymp; s&#772;<sub>A</sub> &nbsp;&times;&nbsp; &phi; &nbsp;&times;&nbsp; s<sub>L</sub> &nbsp;&times;&nbsp; &pi;&#772;</span>
</div>
<ul style="list-style: disc; padding-left: 1.4rem; margin: 0 0 2rem; line-height: 1.8;">
  <li style="font-size: 1rem; font-weight: 300; color: var(--ink-mid); margin-bottom: 0.5rem;"><strong style="color: var(--ink); font-weight: 500;">task scope</strong> (s&#772;<sub>A</sub>): wage-bill–weighted share of tasks AI can do</li>
  <li style="font-size: 1rem; font-weight: 300; color: var(--ink-mid); margin-bottom: 0.5rem;"><strong style="color: var(--ink); font-weight: 500;">feasibility</strong> (&phi;): share of those tasks where AI is cost-effective in practice</li>
  <li style="font-size: 1rem; font-weight: 300; color: var(--ink-mid); margin-bottom: 0.5rem;"><strong style="color: var(--ink); font-weight: 500;">labor share</strong> (s<sub>L</sub>): labor income share (&asymp;0.65)</li>
  <li style="font-size: 1rem; font-weight: 300; color: var(--ink-mid); margin-bottom: 0.5rem;"><strong style="color: var(--ink); font-weight: 500;">productivity gain per task</strong> (&pi;&#772;): average fraction of task time saved</li>
</ul>

<p>Both approaches plug their data into this same formula. The scope and labor share inputs are nearly identical across both studies. The entire gap comes from one place: “productivity gain per task.” Acemoglu draws on controlled lab experiments; Anthropic draws on real usage data. That single input is where the two estimates diverge.</p>

    <h2>Where the Two Estimates Diverge</h2>

    <h3>How broadly does AI reach?</h3>

    <p>Both studies find that AI-capable tasks account for roughly 18–20% of total wages paid across the economy. Acemoglu asks which tasks a current AI model can do in principle; Anthropic looks at which tasks workers actually use Claude for. They measure different things (potential versus actual reach) and land at nearly the same number. Scope is not where the two estimates diverge.</p>

    <h3>How much does AI help when it's used?</h3>

    <p>This is where the gap opens up, and it is large.</p>

    <p>Acemoglu draws on two carefully run experiments from 2022–2023. In one, professional writers using GPT-4 finished tasks about 40% faster than those working without it. In another, call-center workers with an AI tool resolved 14% more issues per hour. Averaging those two studies, AI cuts task time by roughly 27%, meaning a task that took an hour now takes about 45 minutes.</p>

    <p>Anthropic's data tells a very different story. For each task that appears in Claude usage, the model estimates how long the task would take a professional without AI (in hours) and how long it actually took with Claude in the conversation (in minutes). Across thousands of tasks, Anthropic finds speedups of 9–12×: what took an hour without AI takes around 6–7 minutes with it. That difference, multiplied across the same 18–20% slice of the wage bill, produces almost the entire gap in headline estimates.</p>

    <h3>Is cost-effectiveness assumed?</h3>

    <p>Acemoglu applies a discount: even where AI can do a task, only about 1 in 4 of those tasks are worth doing with AI given current wages and subscription costs. Think of a paralegal earning $40/hr being asked to use an AI tool for a 20-minute drafting task. If the AI saves 5 minutes but requires setup time and error review, the economics may not favor it. Anthropic skips this calculation entirely. Their reasoning: if a worker is already using Claude for something, they have already decided it is worth it. When Anthropic's analysts do apply adjustments — accounting for tasks where Claude fails or where automating one step creates new bottlenecks elsewhere — the estimate narrows from 1.8 to 0.7–1.2 percentage points per year.</p>

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
            <td>How scope is measured</td>
            <td>Which tasks GPT-4 can do in principle (potential exposure)</td>
            <td>Which tasks workers actually use Claude for (observed usage)</td>
          </tr>
          <tr>
            <td>Share of wage bill covered</td>
            <td>&sim;18–19%</td>
            <td>&sim;18–20%</td>
          </tr>
          <tr>
            <td>How speedups are measured</td>
            <td>Randomized experiments, 2022–23</td>
            <td>Observed Claude conversations, late 2025</td>
          </tr>
          <tr>
            <td>Observed speedup range</td>
            <td>1.2&times; – 1.6&times; (task takes ~45 min instead of 1 hr)</td>
            <td>9&times; – 12&times; (task takes ~6 min instead of 1 hr)</td>
          </tr>
          <tr>
            <td>Cost-effectiveness filter</td>
            <td>Applied: only ~1 in 4 capable tasks used in practice</td>
            <td>Not applied: usage itself is the evidence of cost-effectiveness</td>
          </tr>
          <tr class="highlight-row">
            <td>Headline / adjusted estimate</td>
            <td>0.62% over 10 years &nbsp;(0.06 pp/yr)</td>
            <td>1.8 pp/yr baseline &rarr; 0.7–1.2 pp/yr after adjustments</td>
          </tr>
        </tbody>
      </table>
    </div>

    <blockquote class="pullquote">
      <p>Both approaches agree AI covers a similar slice of the economy's task portfolio. The entire spread comes from one place: how fast AI speeds up the tasks it reaches.</p>
    </blockquote>

    <h2>Why Are the Speedups So Different?</h2>

    <p>The honest answer is that we do not know yet, but three explanations are probably all partially right. The most straightforward is <strong>selection</strong>. People use Claude for tasks where they expect it to help. If workers naturally lean toward their AI's strengths, the tasks that show up in usage data will be the ones where AI performs best. Controlled experiments sidestep this by randomly assigning tasks, including the hard ones where AI underperforms.</p>

    <p>A second issue is <strong>self-reporting</strong>: Anthropic's speedup estimates come from asking Claude to judge how long tasks take with and without AI assistance. An AI system evaluating its own contribution is not an independent auditor. Third, and perhaps most hopeful: <strong>models may have genuinely improved</strong>. The experiments Acemoglu relies on used GPT-4 in 2022–2023. Anthropic's data reflects Claude in late 2025. If frontier AI capabilities have grown substantially in that time (and most benchmarks suggest they have), part of the speedup gap could be real. That would mean the true productivity impact sits somewhere between the two estimates, not at either extreme.</p>

    <h2>Conclusion</h2>

    <p>The theorem is not in dispute. The scope of AI's reach is not in dispute. The gap sits almost entirely in one question: when AI handles a task, how much faster does it actually get done? That single input determines whether AI is a gradual automation wave manageable with existing workforce policy, or the largest U.S. productivity surge since the 1990s compressed into a few years. Those two futures call for very different responses.</p>

    <p>Settling the question requires an experiment that does not yet exist: a large, randomized study on current frontier models, across the full range of tasks workers actually bring to AI today. Until then, the gap between these two estimates is itself the most informative number we have. The next time you see an AI productivity headline, the right question to ask is not "what share of jobs does AI cover?" — both studies agree on that. Ask instead: "how fast does it actually make things when it's used?"</p>

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
  <p>A task taking 1 hour alone and 10 minutes with AI gives a speedup of 6&times;. This is confirmed by Anthropic directly in their report: "reducing a 1 hour task to 10 minutes would give a 6x speedup." Across the tasks in their January 2026 data with at least 200 observations, the mean speedup is in the range of 9&ndash;12&times; depending on task complexity. The threshold of 200 observations is chosen to replicate their earlier results and to avoid inflating the aggregate by including very rare tasks with noisy speedup estimates. Without the threshold, the implied productivity gain would be around 5 pp/yr, much higher than their headline figure.</p>

  <h3>C. The Sep 2025 AEI Usage-Concentration Exercise</h3>
  <p>An earlier version of this analysis used the September 2025 AEI release, which reports <code>aei_usage_pct</code>: each O*NET task's share of total Claude interactions summing to 100%. This is a <em>concentration</em> measure, not an intensity measure: it records market share, not per-occupation task penetration. When aggregated to the occupation level and plugged into Hulten's s&#772;<sub>A</sub> slot, the result is a GDP-weighted share of about 0.25%, roughly 75 times smaller than the exposure index. The resulting TFP estimate of 0.04% reflects the structural mismatch between a concentration measure and an intensity slot, not any substantive finding about AI's economic impact. The January 2026 release resolves this by providing task-level speedup data that can be properly aggregated.</p>

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
