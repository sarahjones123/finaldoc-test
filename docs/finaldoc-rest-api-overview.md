---
title: "FinalDoc REST API Overview"
description: "Introduction to the FinalDoc REST API, base URLs, authentication, and conventions."
slug: "finaldoc-rest-api-overview"
status: "PUBLISHED"
createdAt: "2026-02-24T05:05:59.136Z"
updatedAt: "2026-03-27T10:29:46.727Z"
---

<h1>FinalDoc REST API Overview</h1>
<p>FinalDoc has a REST API that lets you programmatically manage your knowledge base — create and update articles, manage readers, retrieve analytics data, and more. Use it to integrate FinalDoc with your own tools, build custom automation workflows, or sync documentation with your codebase.</p>

<h2>API Base URL</h2>
<pre><code>https://app.finaldoc.io/api</code></pre>

<h2>Authentication</h2>
<p>All API requests require authentication. FinalDoc supports two token types:</p>
<table>
<thead><tr><th>Token Type</th><th>Format</th><th>Use Case</th></tr></thead>
<tbody>
<tr><td><strong>Session token</strong></td><td><code>fd_xxxxxxxx</code></td><td>Full admin access; for internal automation trusted scripts</td></tr>
<tr><td><strong>API token (scoped)</strong></td><td><code>api_xxxxxxxx</code></td><td>Read/write/delete articles; for Bulk API, third-party integrations</td></tr>
</tbody>
</table>
<p>Include the token in the <code>Authorization</code> header:</p>
<pre><code>Authorization: Bearer YOUR_TOKEN_HERE</code></pre>
<p>Create tokens in <strong>Settings → Data &amp; Compliance → API Tokens</strong>.</p>

<h2>Request Format</h2>
<ul>
<li>All requests and responses use <strong>JSON</strong></li>
<li>Set <code>Content-Type: application/json</code> on POST/PUT/PATCH requests</li>
<li>Date/time values use <strong>ISO 8601</strong> format (e.g., <code>2026-03-12T10:30:00Z</code>)</li>
</ul>

<h2>Response Format</h2>
<p>Most endpoints return JSON. Success responses include the requested data. Error responses follow this format:</p>
<pre><code>{
  "error": "Not found",
  "message": "Article with ID xxx not found",
  "statusCode": 404
}</code></pre>

<h2>Rate Limits</h2>
<ul>
<li><strong>Bulk API (api_ tokens)</strong> — 60 requests per minute per token</li>
<li><strong>Session API (fd_ tokens)</strong> — Subject to fair use; no hard limit but excessive use is throttled</li>
</ul>
<p>When rate limited, the API returns HTTP 429 with a <code>Retry-After</code> header.</p>

<h2>Available APIs</h2>
<table>
<thead><tr><th>API</th><th>What It Covers</th></tr></thead>
<tbody>
<tr><td><strong>Articles API</strong></td><td>List, get, create, update, delete articles</td></tr>
<tr><td><strong>Categories API</strong></td><td>List and manage categories</td></tr>
<tr><td><strong>Readers API</strong></td><td>List, invite, and remove readers</td></tr>
<tr><td><strong>Search API</strong></td><td>Search articles programmatically</td></tr>
<tr><td><strong>Analytics API</strong></td><td>Retrieve article views, reader stats</td></tr>
<tr><td><strong>Feedback API</strong></td><td>List and manage article feedback</td></tr>
<tr><td><strong>Bulk API</strong></td><td>Batch create/update/delete articles</td></tr>
<tr><td><strong>Webhooks API</strong></td><td>Manage webhook subscriptions</td></tr>
</tbody>
</table>
<p>Full reference documentation for each API is in the following articles in this section.</p>

<h2>Versioning</h2>
<p>The current API version is <strong>v1</strong>. Version is implicit in the base URL — there is no <code>/v1/</code> path prefix. When breaking changes are introduced, a new version will be announced with a migration period.</p>