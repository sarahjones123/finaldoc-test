---
title: "AI Optimizer"
description: "Using the AI-powered documentation health check to improve your content."
slug: "ai-optimizer"
status: "PUBLISHED"
createdAt: "2026-02-23T18:13:43.337Z"
updatedAt: "2026-03-12T08:53:58.316Z"
---

<h1>AI Optimizer</h1>
<p>The AI Optimizer runs a comprehensive health check on all your articles using AI. It analyzes each article for readability, completeness, SEO best practices, and content quality — then gives each article a score and actionable recommendations for improvement. Think of it as an automatic content auditor that works across your entire knowledge base at once.</p>

<h2>Opening the AI Optimizer</h2>
<ol>
<li>Go to <strong>Toolbox</strong> in the left sidebar</li>
<li>Under <strong>AI Tools</strong>, click <strong>AI Optimizer</strong></li>
</ol>

<h2>Running an Analysis</h2>
<ol>
<li>Click <strong>Analyze All Articles</strong></li>
<li>The AI processes each article in your knowledge base (this may take a minute or two for large KBs)</li>
<li>Results appear in a table showing each article with its overall score and individual category scores</li>
</ol>

<h2>What Gets Analyzed</h2>
<table>
<thead><tr><th>Category</th><th>What the AI Checks</th></tr></thead>
<tbody>
<tr><td><strong>Readability</strong></td><td>Sentence length, paragraph density, use of passive voice, reading level (Flesch-Kincaid score)</td></tr>
<tr><td><strong>Completeness</strong></td><td>Does the article have a description? Does it cover the topic fully? Are there any obvious gaps (e.g., a "How to" with no steps)?</td></tr>
<tr><td><strong>SEO</strong></td><td>Description quality, heading structure (H1/H2/H3 hierarchy), presence of a clear topic keyword, image alt text</td></tr>
<tr><td><strong>Consistency</strong></td><td>Does the article use consistent terminology? Does it align with your style guide (if defined in AI Settings)?</td></tr>
<tr><td><strong>Freshness</strong></td><td>When was the article last updated? Stale articles (not updated in 6+ months) may need a review</td></tr>
</tbody>
</table>

<h2>Interpreting Scores</h2>
<ul>
<li><strong>80–100 (Green)</strong> — Article is in great shape. No urgent action needed</li>
<li><strong>50–79 (Yellow)</strong> — Some improvements recommended. Click the article to see specific suggestions</li>
<li><strong>0–49 (Red)</strong> — Article needs significant work. Likely missing key elements</li>
</ul>

<h2>Viewing Recommendations</h2>
<ol>
<li>Click any article row in the results to expand its detailed recommendations</li>
<li>Each recommendation explains:
  <ul>
    <li>What the issue is</li>
    <li>Why it matters (impact on readers or search)</li>
    <li>How to fix it</li>
  </ul>
</li>
<li>Click <strong>Open Article</strong> to jump to the article editor and make the changes</li>
</ol>

<h2>Re-running the Analysis</h2>
<p>After making improvements, you can re-run the analysis on specific articles or all articles to see how scores have changed. Click <strong>Re-analyze</strong> next to any article, or click <strong>Analyze All Articles</strong> again to refresh all scores.</p>

<h2>Requirements</h2>
<p>The AI Optimizer requires an AI model to be enabled — either FinalDoc's built-in AI or your own OpenAI key configured in <strong>Settings → AI (Ved AI) → AI Configuration</strong>.</p>