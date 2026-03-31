---
title: "Bulk API Reference"
description: "Programmatically create, update, and delete articles in bulk using API tokens."
slug: "bulk-api-reference"
status: "PUBLISHED"
createdAt: "2026-02-27T10:22:40.999Z"
updatedAt: "2026-03-27T10:29:46.727Z"
---

<h1>Bulk API Reference</h1>
<p>The Bulk API provides high-throughput endpoints for batch operations on articles — useful for content migrations, automated syncing, and large-scale content updates.</p>

<h2>Authentication</h2>
<p>All Bulk API endpoints require an API token (<code>api_</code>) with the appropriate scopes. Session tokens are not accepted. Create API tokens in <strong>Settings → Data &amp; Compliance → API Tokens</strong>.</p>

<h2>Rate Limits</h2>
<p><strong>60 requests per minute</strong> per API token. Exceeding this returns HTTP 429 with a <code>Retry-After: 60</code> header.</p>

<h2>Bulk Create Articles</h2>
<pre><code>POST /bulk/workspaces/{workspaceId}/articles</code></pre>
<p>Requires scope: <code>write:articles</code></p>

<p><strong>Request body:</strong></p>
<pre><code>{
  "articles": [
    {
      "title": "Article One",
      "content": "&lt;h1&gt;...&lt;/h1&gt;",
      "categoryId": "cat_abc",
      "status": "published"
    },
    {
      "title": "Article Two",
      "content": "&lt;h1&gt;...&lt;/h1&gt;"
    }
  ]
}</code></pre>
<p>Maximum 50 articles per request. Returns a results array with success/failure status for each article.</p>

<h2>Bulk Update Articles</h2>
<pre><code>PUT /bulk/articles</code></pre>
<p>Requires scope: <code>write:articles</code></p>

<p><strong>Request body:</strong></p>
<pre><code>{
  "updates": [
    { "id": "art_abc", "status": "published" },
    { "id": "art_def", "title": "New Title", "content": "..." }
  ]
}</code></pre>
<p>Maximum 50 updates per request.</p>

<h2>Bulk Delete Articles</h2>
<pre><code>DELETE /bulk/articles</code></pre>
<p>Requires scope: <code>delete:articles</code></p>

<p><strong>Request body:</strong></p>
<pre><code>{
  "ids": ["art_abc", "art_def", "art_ghi"]
}</code></pre>
<p>Maximum 100 IDs per request. Moves articles to Recycle Bin (not permanent). Returns count of deleted articles.</p>

<h2>Bulk List Articles</h2>
<pre><code>GET /bulk/workspaces/{workspaceId}/articles</code></pre>
<p>Requires scope: <code>read:articles</code></p>
<p>Returns all articles in a workspace with full content. Use <code>cursor</code> parameter for pagination through large datasets.</p>

<h2>Response Format</h2>
<p>Bulk operations return a results object:</p>
<pre><code>{
  "succeeded": 48,
  "failed": 2,
  "results": [
    { "index": 0, "id": "art_abc", "status": "success" },
    { "index": 1, "status": "error", "error": "Category not found" }
  ]
}</code></pre>
<p>Failed items do not stop the batch — all items are processed and the summary shows what succeeded and what failed.</p>

<h2>Webhooks API Reference</h2>
<p>See the <strong>Webhooks API Reference</strong> article for managing webhook subscriptions via API.</p>