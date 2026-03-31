---
title: "Running AI Analysis"
description: ""
slug: "running-ai-analysis"
status: "PUBLISHED"
createdAt: "2026-02-24T18:29:42.058Z"
updatedAt: "2026-03-12T09:27:38.979Z"
---

<h1>Running AI Analysis</h1>
<p>After connecting a ticket source and importing tickets, you run the AI analysis — which reads through all your support tickets and identifies patterns: the most common issues, topics readers ask about, potential documentation gaps, and article suggestions. This is the core of Ticket Analysis.</p>

<h2>Prerequisites</h2>
<ul>
<li>At least one ticket source connected (see Connecting Ticket Sources)</li>
<li>At least 20 tickets imported (analysis is less useful with very few tickets)</li>
</ul>

<h2>Running an Analysis</h2>
<ol>
<li>Click <strong>Ticket Analysis</strong> in the left sidebar</li>
<li>Click <strong>Run New Analysis</strong></li>
<li>Choose the ticket scope:
  <ul>
    <li>All imported tickets</li>
    <li>A specific date range</li>
    <li>Tickets from a specific source (if you have multiple connected)</li>
  </ul>
</li>
<li>Choose the analysis depth:
  <ul>
    <li><strong>Standard</strong> — Analyzes topics and common issues. Faster (5–10 minutes)</li>
    <li><strong>Deep</strong> — Also generates specific documentation recommendations and article drafts. Slower (10–30 minutes)</li>
  </ul>
</li>
<li>Click <strong>Start Analysis</strong></li>
<li>A progress bar shows the analysis status. You can navigate away — you'll be notified when it's complete</li>
</ol>

<h2>Analysis Results</h2>
<p>When analysis completes, the results appear in the Ticket Analysis dashboard:</p>

<h3>Top Issue Topics</h3>
<p>A ranked list of the most common topics across all analyzed tickets:</p>
<ul>
<li>Topic name (AI-generated label like "Login issues", "Billing questions", "Feature requests")</li>
<li>Ticket count — How many tickets were about this topic</li>
<li>% of all tickets</li>
<li>Trend — Is this topic growing, shrinking, or stable?</li>
</ul>

<h3>Documentation Gaps</h3>
<p>Topics where tickets are common but your KB has little or no coverage. These are your highest-value documentation opportunities. For each gap:</p>
<ul>
<li>The identified topic</li>
<li>Sample ticket excerpts that illustrate the issue</li>
<li>Suggested article title(s)</li>
<li><strong>Create Draft</strong> button — generates an AI article draft for this topic</li>
</ul>

<h3>Article Improvement Suggestions</h3>
<p>Existing KB articles that are related to high-volume ticket topics but may be incomplete or unclear — based on readers' tickets suggesting they didn't find the answer in existing docs.</p>

<h2>Scheduling Regular Analyses</h2>
<p>Set up automatic periodic analyses in <strong>Settings → Integrations → Ticket Analysis</strong>. Choose weekly or monthly. Results appear automatically in the dashboard when the scheduled analysis completes.</p>