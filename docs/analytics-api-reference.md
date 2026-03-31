---
title: "Analytics API Reference"
description: ""
slug: "analytics-api-reference"
status: "PUBLISHED"
createdAt: "2026-02-24T08:32:54.589Z"
updatedAt: "2026-03-27T10:29:46.727Z"
---

<h1>Analytics API Reference</h1>
<p>The Analytics API lets you retrieve article view statistics, reader engagement data, and search analytics programmatically — useful for building custom dashboards or exporting data to external BI tools.</p>

<h2>Get Article Analytics</h2>
<pre><code>GET /projects/{projectId}/analytics/articles</code></pre>

<p><strong>Query parameters:</strong></p>
<ul>
<li><code>startDate</code> — ISO 8601 start date (e.g., <code>2026-01-01</code>)</li>
<li><code>endDate</code> — ISO 8601 end date</li>
<li><code>workspaceId</code> — Restrict to a specific workspace</li>
<li><code>limit</code> — Max articles returned (default 50)</li>
<li><code>sortBy</code> — <code>views</code>, <code>unique_readers</code>, <code>avg_time</code>, <code>feedback_score</code></li>
<li><code>sortOrder</code> — <code>desc</code> (default) or <code>asc</code></li>
</ul>

<p><strong>Example response:</strong></p>
<pre><code>{
  "articles": [
    {
      "articleId": "art123",
      "title": "Getting Started",
      "views": 4521,
      "uniqueReaders": 2103,
      "avgTimeOnPage": 187,
      "feedbackPositive": 234,
      "feedbackNegative": 12,
      "feedbackScore": 0.95
    }
  ],
  "period": { "start": "2026-01-01", "end": "2026-03-12" },
  "total": 184
}</code></pre>

<h2>Get Daily Traffic</h2>
<pre><code>GET /projects/{projectId}/analytics/traffic</code></pre>
<p>Returns daily page view totals for the project's KB over a date range.</p>

<p><strong>Query parameters:</strong></p>
<ul>
<li><code>startDate</code>, <code>endDate</code> — Date range</li>
<li><code>granularity</code> — <code>day</code>, <code>week</code>, or <code>month</code></li>
</ul>

<h2>Get Search Analytics</h2>
<pre><code>GET /projects/{projectId}/analytics/searches</code></pre>
<p>Returns search query data — top queries, zero-result queries, and search volume trends.</p>

<p><strong>Query parameters:</strong></p>
<ul>
<li><code>startDate</code>, <code>endDate</code></li>
<li><code>zeroResults</code> — If <code>true</code>, only returns queries that returned no results</li>
<li><code>limit</code></li>
</ul>

<h2>Get Reader Analytics</h2>
<pre><code>GET /projects/{projectId}/analytics/readers</code></pre>
<p>Returns reader engagement data — top readers by activity, geographic distribution, and session data.</p>

<h2>Authentication</h2>
<p>Analytics API endpoints require a session token (<code>fd_</code>). API tokens (<code>api_</code>) do not have access to analytics data.</p>