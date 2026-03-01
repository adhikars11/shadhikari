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
    .takeaways ol { padding-left: 1.4rem; list-style: decimal; }
    .takeaways li {
      margin-bottom: 0.6rem;
      font-size: 0.95rem;
      color: var(--ink);
      line-height: 1.6;
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
    .prose h3 {
      font-family: 'DM Serif Display', serif;
      font-size: 1.15rem;
      font-style: italic;
      font-weight: 400;
      color: var(--ink);
      margin: 2.25rem 0 0.7rem;
    }
    .prose p {
      margin-bottom: 1.3rem;
      font-size: 1rem;
      font-weight: 300;
      color: var(--ink-mid);
      line-height: 1.8;
    }
    .prose p strong { color: var(--ink); font-weight: 500; }

    /* Stat row */
    .stat-row {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(155px, 1fr));
      gap: 1rem;
      margin: 2.5rem 0;
    }
    .stat-box {
      background: var(--surface);
      border: 1px solid var(--rule);
      border-radius: 6px;
      padding: 1.25rem 1rem 1rem;
      text-align: center;
    }
    .stat-box .num {
      font-family: 'DM Serif Display', serif;
      font-size: 2.1rem;
      color: var(--accent);
      display: block;
      line-height: 1;
      margin-bottom: 0.4rem;
    }
    .stat-box .desc {
      font-family: var(--mono);
      font-size: 0.62rem;
      letter-spacing: 0.1em;
      text-transform: uppercase;
      color: var(--ink-muted);
    }

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

    /* Figures */
    .figure-block { margin: 2.25rem 0; }
    .figure-block .fig-label {
      font-family: var(--mono);
      font-size: 0.62rem;
      letter-spacing: 0.12em;
      text-transform: uppercase;
      color: var(--accent);
      margin-bottom: 0.4rem;
      display: block;
    }
    .figure-block .fig-title {
      font-size: 0.92rem;
      font-weight: 500;
      color: var(--ink);
      margin-bottom: 0.75rem;
    }
    .figure-block img {
      width: 100%;
      border-radius: 6px;
      border: 1px solid var(--rule);
      display: block;
    }
    .figure-block .fig-note {
      font-size: 0.78rem;
      color: var(--ink-muted);
      margin-top: 0.6rem;
      font-style: italic;
      line-height: 1.5;
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

    /* Step boxes */
    .steps { margin: 2rem 0; display: flex; flex-direction: column; gap: 0.75rem; }
    .step {
      display: flex;
      gap: 1.25rem;
      align-items: flex-start;
      padding: 1rem 1.25rem;
      background: var(--surface);
      border: 1px solid var(--rule);
      border-radius: 6px;
    }
    .step-num {
      font-family: 'DM Serif Display', serif;
      font-size: 1.4rem;
      color: var(--accent);
      line-height: 1;
      flex-shrink: 0;
      width: 1.6rem;
      text-align: center;
    }
    .step-body { flex: 1; }
    .step-body .step-label {
      font-family: var(--mono);
      font-size: 0.62rem;
      letter-spacing: 0.14em;
      text-transform: uppercase;
      color: var(--accent);
      display: block;
      margin-bottom: 0.3rem;
    }
    .step-body p {
      font-size: 0.92rem;
      color: var(--ink-mid);
      font-weight: 300;
      margin: 0;
      line-height: 1.65;
    }
    .step-body p strong { color: var(--ink); font-weight: 500; }

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
  <p class="subtitle">A task-based framework puts AI's 10-year TFP gain at roughly 0.6% under the most favorable assumptions. When we substitute theoretical exposure for observed usage, that number drops below 0.1%. The gap between the two is the story.</p>
  <p class="meta">Shisham Adhikari <span>&middot;</span> March 1, 2026</p>
</section>

<main>
<div class="container">

  <div class="takeaways-wrap">
    <div class="takeaways">
      <span class="kicker">Key Takeaways</span>
      <ol>
        <li><strong>A clean aggregation result.</strong> Using Hulten's theorem, AI's macroeconomic impact reduces to three empirical ingredients: what share of labor tasks AI touches, what fraction of those can be profitably automated, and how much labor cost those automations save. Multiplied together, the implied 10-year TFP gain is roughly 0.5–0.7%—modest relative to popular forecasts.</li>
        <li><strong>Exposure and usage tell very different stories.</strong> A wage-bill-weighted measure of AI-susceptible tasks assigns about 18.7% of total labor costs to AI-exposed occupations. Replacing that with observed Claude usage data drops the GDP-weighted share to 0.25%—a 75&times; gap between where AI could go and where it currently is.</li>
        <li><strong>The hybrid is the generous bound.</strong> Granting full exposure credit to occupations with no observed usage—while keeping raw usage values for those that appear in AEI data—yields a GDP-weighted share of 1.5% and a 10-year TFP gain of about 0.05%.</li>
        <li><strong>The gap is informative, not discouraging.</strong> The 75&times; shortfall between theoretical exposure and observed usage shows how early and concentrated current adoption still is. The diffusion story is in its first chapter.</li>
      </ol>
    </div>
  </div>

  <div class="prose">

    <h2>The Right Question</h2>

    <p>People argue about how much AI will change the economy with remarkable confidence for a topic that resists easy measurement. Optimistic forecasts—some from major investment banks—project GDP gains of 7% or more. More cautious analysts suggest the impact will be no larger than previous general-purpose technologies. Both camps are often speaking without a shared framework for what "impact" even means at the aggregate level.</p>

    <p>The honest answer is that aggregating task-level productivity improvements to economy-wide outcomes requires a chain of non-trivial steps: you need to know which tasks AI improves, by how much, and how improvements in individual tasks map to total output. Get any link wrong and your estimate is off by an order of magnitude. This is where the theoretical work matters.</p>

    <p>This post walks through a framework for answering the question rigorously—built on Acemoglu's (2024) task-based model—and then asks what happens when we replace the theoretical exposure index at its core with something sharper: actual observed AI usage.</p>

    <h2>Tasks All the Way Down</h2>

    <p>The starting point for modern economic analysis of automation is the <strong>task framework</strong>. Rather than modeling production as a single aggregate process, it treats an economy's output as the result of combining many distinct tasks—drafting a memo, reconciling a balance sheet, diagnosing a rash, welding a seam. Each task can be performed by either labor or capital (machines, software, AI systems), and different tasks favor different inputs.</p>

    <p>AI enters by changing which tasks capital can perform. When a language model can write a first draft that would previously have required a human, that task moves from the labor side to the capital side of the ledger. When AI assists a radiologist in reading scans without replacing them outright, it raises labor productivity within the task rather than substituting for the person entirely.</p>

    <p>The critical structural feature of this model is that tasks are <strong>gross complements</strong>: in a production process, you generally need all the tasks done, and doing any single one faster has a bounded impact on total output. Think of a complex product like a car: automating the paint booth doesn't help much if the engine assembly is the bottleneck. This complementarity is what keeps aggregate AI impacts in check even when individual task-level productivity gains are large. The economy is not a single task waiting to be accelerated—it is thousands of interdependent tasks, and moving one does not move all of them proportionally.</p>

    <p>This insight sets an upper bound on what any automation technology can deliver. But it also provides the key to making the calculation tractable.</p>

    <h2>The Aggregation Shortcut: Hulten's Theorem</h2>

    <p>Once you accept the task framework, an elegant result from public economics does most of the heavy lifting. <strong>Hulten's theorem</strong> says that to first order, the impact of a productivity improvement in a sector (or task) on aggregate output is proportional to that sector's <em>share of GDP</em>, not its share of employment or any other metric.</p>

    <p>Applied to AI, this means you don't need a fully solved general equilibrium model to estimate the economy-wide TFP effect. You need three things:</p>

    <div class="steps">
      <div class="step">
        <span class="step-num">1</span>
        <div class="step-body">
          <span class="step-label">Scope</span>
          <p>What <strong>share of total labor tasks</strong> (weighted by their contribution to GDP) does AI plausibly affect? Call this <em>s&#772;<sub>A</sub></em>.</p>
        </div>
      </div>
      <div class="step">
        <span class="step-num">2</span>
        <div class="step-body">
          <span class="step-label">Feasibility</span>
          <p>Of those exposed tasks, what <strong>fraction can be profitably automated</strong> today—meaning the cost of running AI is less than the labor cost saved? Call this <em>&phi;</em>.</p>
        </div>
      </div>
      <div class="step">
        <span class="step-num">3</span>
        <div class="step-body">
          <span class="step-label">Depth</span>
          <p>For tasks that are feasibly automated, <strong>how large is the labor cost saving</strong> on average? This is an industry-adjusted figure—the share of income paid to labor in exposed sectors, times the fraction by which AI cuts that labor cost. Call this <em>s<sub>L</sub> &times; &pi;&#772;</em>.</p>
        </div>
      </div>
    </div>

    <p>Multiply all three together and you have an estimate of the total factor productivity (TFP) gain—the efficiency improvement that accrues to the whole economy, independent of how much capital you subsequently invest. Formally:</p>

    <div class="formula">
      <span class="formula-line">TFP gain &asymp; s&#772;<sub>A</sub> &times; &phi; &times; s<sub>L</sub> &times; &pi;&#772;</span>
      <span class="formula-comment">s&#772;<sub>A</sub> = GDP-weighted exposed share &nbsp;|&nbsp; &phi; = fraction feasibly automated &nbsp;|&nbsp; s<sub>L</sub> = labor share of income in exposed industries &nbsp;|&nbsp; &pi;&#772; = avg. labor cost saving</span>
    </div>

    <p>What makes this tractable is that each ingredient can be estimated independently from different bodies of empirical work—occupation surveys, laboratory experiments, industry accounts—and then combined. The framework does not require you to model how firms will adjust capital, how wages will respond, or how workers will reallocate. Those are important second-order questions, but they don't change the first-order TFP accounting.</p>

    <h2>The Baseline Numbers</h2>

    <p>Acemoglu (2024) plugs in estimates that represent a reasonable reading of the literature. The exposure measure comes from Eloundou et al. (2023), who used GPT-4 judgments to classify which occupational tasks are susceptible to large language model assistance. Aggregated across the US workforce and weighted by wage bills, this gives a GDP-weighted exposed share of roughly <strong>19–20%</strong>.</p>

    <p>The feasibility parameter—what fraction of those tasks can actually be automated profitably—draws on Svanberg et al.'s (2024) analysis of computer vision, which suggests about <strong>23%</strong> of exposed tasks clear the cost-benefit bar at current AI prices. The cost savings estimate comes from averaging results from two controlled experiments that measured how much faster workers performed tasks with AI assistance: roughly <strong>27%</strong> labor cost reduction on average.</p>

    <p>Plugging into the formula, and adjusting the cost savings for the labor share of income in exposed industries (about 53–54%, since high-exposure sectors are slightly less labor-intensive than the economy as a whole):</p>

    <div class="formula">
      <span class="formula-line">TFP &asymp; 0.187 &times; 0.23 &times; 0.535 &times; 0.27 &asymp; <strong>0.62%</strong> over 10 years</span>
      <span class="formula-comment">Replication of Acemoglu (2024) using exposure-based index; calculated from BLS and BEA data</span>
    </div>

    <div class="stat-row">
      <div class="stat-box">
        <span class="num">18.7%</span>
        <span class="desc">GDP-weighted exposed share</span>
      </div>
      <div class="stat-box">
        <span class="num">4.3%</span>
        <span class="desc">Feasible share (×0.23)</span>
      </div>
      <div class="stat-box">
        <span class="num">53.5%</span>
        <span class="desc">Labor share, exposed industries</span>
      </div>
      <div class="stat-box">
        <span class="num">0.62%</span>
        <span class="desc">TFP gain over 10 years</span>
      </div>
    </div>

    <p>To put that in perspective: this is roughly one-tenth of what Goldman Sachs projected and about one-twentieth of what some optimistic technology forecasters have suggested. A 0.62% TFP gain over a decade is real and meaningful—but it is not the kind of growth shock that reshapes distributional dynamics or requires fundamentally new macroeconomic frameworks. And this is the <em>optimistic</em> version of the calculation.</p>

    <p>The paper goes further by distinguishing between <em>easy-to-learn</em> tasks (those with clear success metrics, like drafting, classifying, or computing, where AI can train effectively because what "good" looks like is unambiguous) and <em>hard-to-learn</em> tasks (those with no simple outcome metric, like giving complex legal counsel or supervising a team). Adjusting for the mix of easy and hard tasks—about 73% easy among exposed tasks—brings the 10-year TFP estimate down to approximately 0.53%.</p>

    <blockquote class="pullquote">
      <p>The gap between what AI could plausibly do and what it is currently doing is not a rounding error. It is 75 times the actual signal.</p>
    </blockquote>

    <h2>What Actual Usage Tells Us</h2>

    <p>Everything above rests on the exposure index: a measure of which tasks AI is <em>capable of</em> affecting, scored by annotators or language models looking at O*NET task descriptions. This is the natural starting point when forecasting AI's potential scope. But it is not the same as observing what AI is <em>actually doing</em> in the economy today.</p>

    <p>The Anthropic Economic Index (AEI) provides something closer to the latter: a dataset mapping observed Claude interactions to occupations, capturing where people are actually asking AI to help with work tasks. Rather than measuring what AI <em>could</em> do, it measures what workers are currently doing with it. Plugging it into the same aggregation framework yields a very different answer.</p>

    <p>The AEI usage measure is a <em>share-of-pie</em>: each occupation's score reflects what fraction of total Claude interactions belong to that occupation. By construction it sums to 100% across the 608 covered occupations. The top occupation—software developers (SOC 15-1251)—accounts for about 7.6% of all usage. Retail salespersons, which exposure models often flag as moderately susceptible, barely appear.</p>

    <p>Critically, this is not a per-occupation rate like the exposure index—it is a relative concentration measure. For occupations not observed in AEI data (the majority of the roughly 800 occupations in the wage data), the usage score is zero: they contribute nothing to observed Claude usage. This is the hardline lower bound: if an occupation doesn't appear in the data, we do not grant it any AI activity credit.</p>

    <p>Running the same aggregation pipeline with this index produces:</p>

    <div class="formula">
      <span class="formula-line">TFP (usage-based) &asymp; 0.0025 &times; 0.23 &times; 0.576 &times; 0.27 &asymp; <strong>0.01%</strong> over 10 years</span>
      <span class="formula-comment">GDP-weighted share collapses to 0.25% when exposure is replaced with observed AEI usage</span>
    </div>

    <p>The GDP-weighted share drops from 18.7% to 0.25%—a 75-fold reduction. The labor share of income ticks up slightly (to 57.6%), because observed usage is concentrated in professional services and technology sectors that are somewhat more labor-intensive than the broader exposed task pool. But the dominant force is the collapse in the GDP-weighted share, which carries the TFP estimate from 0.62% to 0.01%.</p>

    <p>A third model splits the difference. The <strong>hybrid approach</strong> assigns actual usage values to occupations that appear in AEI, and falls back to the exposure index for those that do not. This operationalizes a "benefit of the doubt" assumption: occupations not yet observed using AI are credited with full potential exposure, while those that are observed are held to actual usage. The logic is that absence in the AEI is not evidence of absence—workers in non-tech occupations may be using AI in ways not captured in this dataset.</p>

    <div class="table-wrap">
      <p class="table-caption">Table 1 &mdash; Aggregate impact estimates under three index assumptions</p>
      <table>
        <thead>
          <tr>
            <th>Index</th>
            <th>GDP-Weighted Share</th>
            <th>Feasible Share</th>
            <th>Labor Share (exposed)</th>
            <th>TFP (10-yr)</th>
          </tr>
        </thead>
        <tbody>
          <tr>
            <td>Exposure (Acemoglu baseline)</td>
            <td>18.70%</td>
            <td>4.30%</td>
            <td>53.51%</td>
            <td>0.62%</td>
          </tr>
          <tr class="highlight-row">
            <td>Usage (AEI, missing = 0)</td>
            <td>0.25%</td>
            <td>0.06%</td>
            <td>57.63%</td>
            <td>0.01%</td>
          </tr>
          <tr>
            <td>Hybrid (usage + exposure fill)</td>
            <td>1.47%</td>
            <td>0.34%</td>
            <td>58.72%</td>
            <td>0.05%</td>
          </tr>
        </tbody>
      </table>
    </div>

    <p>The hybrid lands at a GDP-weighted share of 1.47% and a 10-year TFP gain of 0.05%—better than the pure usage estimate, but still about 12 times smaller than the exposure baseline. All three productivity and TFP figures use the same assumptions (&phi; = 0.23, &pi;&#772; = 0.27) across all three index variants. The only thing changing is the index that defines which occupations are covered and by how much.</p>

    <h2>Reading the Gap</h2>

    <p>A 75-fold gap between what the exposure index predicts and what usage data observes could be read as a failure of one or the other measure. But the more productive interpretation is that the two measures are asking different questions, and the distance between their answers is itself informative.</p>

    <p>The exposure index is a measure of <em>technological potential</em>: given what AI systems can do as of their training date, which task descriptions could plausibly be AI-assisted or AI-replaced? It is silent on price, workflow integration, trust, institutional barriers, or the simple friction of adoption.</p>

    <p>The usage index is a measure of <em>current realized adoption</em> among Anthropic's users: where are people who are actively using Claude concentrating their usage? It captures adoption among a self-selected population of early adopters, and is almost entirely concentrated in technology and professional services. Fields with high exposure but currently low adoption—clerical work, retail, healthcare support—appear nearly absent.</p>

    <p>This concentration pattern matches what we know about technology diffusion more broadly. Early adoption is always frontier-led: the sectors with the lowest switching costs, the most digitally-native workflows, and the clearest immediate return are always first. Broad-based diffusion follows over years, not months. The 0.25% GDP-weighted share from usage data is not a ceiling—it is a snapshot of where the frontier currently sits.</p>

    <p>The hybrid's 1.47% is perhaps the most intellectually honest of the three estimates. It says: if we take observed usage at face value where we see it, and grant that unexplored occupations are at full potential where we don't, we still get an implied TFP gain well below even Acemoglu's already-modest baseline. That gap—between 1.47% and 18.7%—is the adoption work that still needs to happen for theoretical exposure to translate into realized economic impact.</p>

    <blockquote class="pullquote">
      <p>Usage data shows where AI currently works. Exposure data shows where AI could eventually work. The 12&times; gap between them is a map of what diffusion still has to accomplish.</p>
    </blockquote>

    <h2>What This Means Going Forward</h2>

    <p>Several things follow from this exercise. First, <strong>the framework is right even if the inputs are not</strong>. Hulten's theorem is a clean, assumption-lean way to aggregate task-level impacts to economy-wide TFP. Any serious estimate of AI's macro impact should be doing something like this calculation, not extrapolating from sector-level revenue projections or survey-based expectations. The debate should be about what goes in, not about the structure of the formula.</p>

    <p>Second, <strong>the right index matters enormously</strong>. Swapping exposure for usage—while holding everything else constant—moves the TFP estimate by two orders of magnitude. This means debates about what AI is doing to the economy hinge critically on which measure of AI activity you take as the input. Exposure measures tell you about the frontier of what is possible; usage measures tell you about current reality. Both are useful, but they answer different questions and should not be conflated.</p>

    <p>Third, <strong>the gap between potential and reality is the diffusion question</strong>. The 75-fold shortfall between exposure and usage is not a criticism of AI; it is a description of where we are in the adoption cycle. The economy-wide impact of AI will grow as usage diffuses from early-adopting technology and professional services workers to the broader workforce. Tracking how that gap closes over time—using precisely this kind of index comparison—is one of the more useful empirical exercises for understanding how transformative AI will turn out to be.</p>

    <p>Finally, <strong>the modest baseline should recalibrate expectations, not dampen ambition</strong>. A 0.62% TFP gain over 10 years is real progress—comparable to a meaningful fraction of historical TFP growth rates. But it is a long way from the claims that AI will produce GDP growth of 7% or reorient the trajectory of economic development. Those claims require AI to move far beyond the easy-to-learn tasks where current performance is strongest, to automate a much larger share of exposed tasks than current cost structures allow, and to diffuse across the workforce at a pace that historical technology adoption rarely achieves. Each of those steps is possible. None of them is guaranteed.</p>

  </div>

</div><!-- /container -->
</main>

<section class="appendix">
<div class="container">

  <h2>Appendix</h2>
  <p class="app-intro">Technical details on the calculations, data sources, and limitations discussed in the main text.</p>

  <h3>A. The TFP Formula in Detail</h3>
  <p>The core aggregation result follows from Hulten's (1978) theorem applied to a task-based model of production. In Acemoglu (2024), final output is produced by combining a continuum of tasks with elasticity of substitution &sigma; &lt; 1 (tasks are gross complements). Each task is produced using either capital or labor with task-specific productivity advantages. AI enters by shifting the margin of automation—tasks previously performed by labor become feasible for capital—and by raising labor productivity in the remaining tasks.</p>
  <p>To first order, the TFP effect of automation is:</p>
  <p><code>d ln TFP = s&#772;_A &times; &phi; &times; s_L &times; &pi;&#772;</code></p>
  <p>where <strong>s&#772;_A</strong> is the wage-bill-weighted share of tasks exposed to AI automation, <strong>&phi;</strong> is the fraction of those tasks for which automation is cost-effective at current AI prices, <strong>s_L</strong> is the GDP-weighted labor share of income in industries where exposed tasks are concentrated, and <strong>&pi;&#772;</strong> is the average fractional reduction in labor cost from AI assistance in the automatable tasks. The product <strong>s&#772;_A &times; &phi;</strong> gives the "feasible share"—the fraction of the overall GDP contribution of labor that AI can realistically displace in the near term.</p>

  <h3>B. Data Sources</h3>
  <ul>
    <li><strong>Occupation-level exposure index:</strong> Acemoglu (2024), derived from Eloundou, Manning, Mishkin, and Rock (2023). Task-level GPT-4 annotations of O*NET work activities, aggregated to 6-digit SOC occupations. Covers 798 occupations with nonzero automation scores. GDP-weighted using BLS Occupational Employment and Wage Statistics (OEWS), years 2019–2024.</li>
    <li><strong>AEI usage index:</strong> Anthropic Economic Index (AEI), September 2025 release. Maps observed Claude API and product interactions to O*NET occupational categories. <code>aei_usage_pct</code> is normalized to sum to 100 across the 608 covered SOC codes (a share-of-pie measure). Used here as <code>usage = aei_usage_pct / 100</code>.</li>
    <li><strong>Wage and employment data:</strong> BLS OEWS, national estimates, years 2019–2024. Employment-weighted average annual mean wages used to construct GDP shares at the 6-digit SOC level, averaged across years for stability.</li>
    <li><strong>Industry labor shares:</strong> BEA National Income and Product Accounts. Wage and salary income plus an adjustment for self-employment labor income (using CPS hours data), divided by value added net of production taxes. Averaged over 2018–2022. Industries at the 14-sector BEA level matched to NAICS codes via crosswalk.</li>
    <li><strong>Industry-occupation crosswalk:</strong> BLS industry-occupation employment matrix (OES). Used to map occupation-level exposure/usage scores to industry-level weighted averages for the labor share calculation.</li>
  </ul>

  <h3>C. Index Construction and the Hybrid Model</h3>
  <p>Three occupation-level indices are constructed at the 6-digit SOC level:</p>
  <ul>
    <li><strong>Exposure:</strong> The <code>automation</code> variable from Acemoglu (2024), a per-occupation rate in [0, 1] reflecting the share of tasks in that occupation judged susceptible to AI automation. Missing occupations receive zero. Sums to approximately 127 across 798 occupations (average ~0.16 per occupation).</li>
    <li><strong>Usage:</strong> <code>aei_usage_pct / 100</code> directly, without rescaling. Each occupation's value is its share of total observed Claude usage (0–0.076 for the top occupation). Sums to 1.0 across 608 occupations. Occupations not in AEI receive zero. Scales differ from exposure by construction—this is intentional and reflects the difference between a per-occupation rate and a share-of-pie measure.</li>
    <li><strong>Hybrid:</strong> For each occupation, take <code>usage</code> if available in AEI, otherwise fall back to <code>automation</code> (exposure). Missing values in both receive zero. This mixes two scales: observed usage values (0–0.076) for covered occupations and per-occupation exposure rates (0–1) for uncovered ones.</li>
  </ul>
  <p>The GDP-weighted share is computed as <code>sum(index_i &times; emp_share_i)</code> over all occupations, where <code>emp_share_i</code> is occupation <em>i</em>'s share of the total annual wage bill. The industry labor share is calculated by distributing each occupation's index value across industries using the BLS crosswalk, computing industry-weighted averages, and then computing the industry-share-weighted average of BEA labor shares.</p>

  <h3>D. Limitations of the Usage Index</h3>
  <ul>
    <li><strong>Selection into Anthropic usage.</strong> AEI captures interactions with Claude specifically. Workers using GPT-4, Gemini, Copilot, or open-source models are not counted. If usage is correlated across platforms, this may scale the absolute level of usage without distorting the cross-occupation distribution, but we cannot be certain.</li>
    <li><strong>Coverage gap.</strong> AEI maps interactions to 608 of approximately 800 detailed SOC occupations. The remaining occupations may genuinely have low usage, or their usage may be too sparse to assign reliably. The zero imputation for missing occupations is conservative.</li>
    <li><strong>Share-of-pie versus per-occupation rate.</strong> The AEI usage index is a relative concentration measure (it sums to 1), not an absolute per-occupation rate (which would be comparable to the exposure index on its own terms). Exposure asks "what fraction of this occupation's tasks could AI do?"; usage asks "what fraction of all AI usage goes to this occupation?" These are different questions embedded in the same aggregation formula.</li>
    <li><strong>Temporal snapshot.</strong> Both indices represent a specific point in time. Exposure reflects AI capabilities as assessed in 2023. Usage reflects AEI data through late 2025. Neither captures how fast adoption is changing, which may be the most economically important variable.</li>
  </ul>

  <h3>E. Full Results Table</h3>
  <div class="table-wrap">
    <p class="table-caption">Table A1 &mdash; All computed quantities by index, with fixed parameters &phi; = 0.23 and &pi;&#772; = 0.27</p>
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
        <tr><td>Labor share of exposed industries (s<sub>L</sub>)</td><td>53.51%</td><td>57.63%</td><td>58.72%</td></tr>
        <tr><td>Productivity component (s<sub>L</sub> &times; &pi;&#772;)</td><td>14.45%</td><td>15.56%</td><td>15.85%</td></tr>
        <tr><td>TFP gain over 10 years</td><td>0.62%</td><td>0.01%</td><td>0.05%</td></tr>
        <tr><td>Implied annual TFP growth</td><td>0.062%/yr</td><td>0.001%/yr</td><td>0.005%/yr</td></tr>
      </tbody>
    </table>
  </div>
  <p>Note: Productivity and TFP figures use fixed parameters &phi; = 0.23 (feasibility of automation, from Svanberg et al. 2024) and &pi;&#772; = 0.27 (average labor cost savings, averaged from Noy &amp; Zhang 2023 and Brynjolfsson et al. 2023) across all three index variants. The only quantity that changes across columns is the index s&#772;<sub>A</sub> and its industry composition (which determines s<sub>L</sub>).</p>

  <h3>F. References</h3>
  <ul>
    <li>Acemoglu, D. (2024). <em>The Simple Macroeconomics of AI.</em> Economic Policy. MIT Department of Economics.</li>
    <li>Acemoglu, D., and P. Restrepo (2022). "Tasks, automation, and the rise in U.S. wage inequality." <em>Econometrica</em>, 90(5), 1973–2016.</li>
    <li>Anthropic (2025). <em>Anthropic Economic Index.</em> September 2025 release. Occupation-level Claude usage, mapped to O*NET/SOC occupations.</li>
    <li>Brynjolfsson, E., D. Li, and L. R. Raymond (2023). "Generative AI at work." <em>NBER Working Paper</em> No. 31161.</li>
    <li>Eloundou, T., S. Manning, P. Mishkin, and D. Rock (2023). "GPTs are GPTs: An early look at the labor market impact potential of large language models." <em>NBER Working Paper</em> No. 31255.</li>
    <li>Hulten, C. R. (1978). "Growth accounting with intermediate inputs." <em>Review of Economic Studies</em>, 45(3), 511–518.</li>
    <li>Noy, S., and W. Zhang (2023). "Experimental evidence on the productivity effects of generative artificial intelligence." <em>Science</em>, 381(6654), 187–192.</li>
    <li>Svanberg, M., et al. (2024). Computer vision automation feasibility study. Referenced in Acemoglu (2024) for the 23% automation feasibility parameter.</li>
    <li>U.S. Bureau of Labor Statistics. Occupational Employment and Wage Statistics (OEWS), national estimates, 2019–2024.</li>
    <li>U.S. Bureau of Economic Analysis. National Income and Product Accounts (NIPA); Industry accounts, 2015–2024.</li>
  </ul>

</div>
</section>

<footer>
  Shisham Adhikari <span class="dot">&middot;</span> March 2026 <span class="dot">&middot;</span> AI &amp; Labor Markets
</footer>

</body>
</html>
