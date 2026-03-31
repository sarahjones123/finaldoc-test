---
title: "Articles API Reference"
description: "Complete reference for the Articles API — create, read, update, and delete articles."
slug: "articles-api-reference"
status: "PUBLISHED"
createdAt: "2026-02-24T05:06:02.600Z"
updatedAt: "2026-03-27T10:29:46.727Z"
---

<h1>Articles API Reference</h1>
<p>The Articles API lets you programmatically create, read, update, and delete articles in your FinalDoc knowledge base.</p>

<h2>Base URL</h2>
<pre><code>https://app.finaldoc.io/api</code></pre>

<h2>List Articles</h2>
<pre><code>GET /workspaces/{workspaceId}/articles</code></pre>
<p>Returns all articles in a workspace.</p>

<p><strong>Query parameters:</strong></p>
<ul>
<li><code>status</code> — Filter by status: <code>published</code>, <code>draft</code>, <code>archived</code></li>
<li><code>categoryId</code> — Filter by category</li>
<li><code>limit</code> — Max results (default: 50, max: 200)</li>
<li><code>offset</code> — Pagination offset</li>
</ul>

<p><strong>Example response:</strong></p>
<pre><code>{
  "articles": [
    {
      "id": "abc123",
      "title": "Getting Started",
      "slug": "getting-started",
      "status": "published",
      "categoryId": "cat456",
      "createdAt": "2026-01-15T10:00:00Z",
      "updatedAt": "2026-03-01T14:30:00Z",
      "wordCount": 842,
      "views": 1250
    }
  ],
  "total": 184,
  "limit": 50,
  "offset": 0
}</code></pre>

<h2>Get Article</h2>
<pre><code>GET /articles/{articleId}</code></pre>
<p>Returns a single article including full HTML content.</p>

<h2>Create Article</h2>
<pre><code>POST /workspaces/{workspaceId}/articles</code></pre>

<p><strong>Request body:</strong></p>
<pre><code>{
  "title": "My New Article",
  "content": "&lt;h1&gt;Introduction&lt;/h1&gt;&lt;p&gt;Content here...&lt;/p&gt;",
  "categoryId": "cat456",
  "status": "draft",
  "slug": "my-new-article",
  "description": "A brief summary for search results"
}</code></pre>

<p><strong>Required fields:</strong> <code>title</code></p>
<p><strong>Returns:</strong> The created article object with its new <code>id</code>.</p>

<h2>Update Article</h2>
<pre><code>PUT /articles/{articleId}</code></pre>
<p>Replaces article fields. Only include fields you want to change — omitted fields remain unchanged.</p>

<p><strong>Common update operations:</strong></p>
<pre><code>// Publish a draft article
{ "status": "published" }

// Update content
{ "content": "&lt;h1&gt;Updated Content&lt;/h1&gt;..." }

// Change title and slug together
{ "title": "New Title", "slug": "new-title" }</code></pre>

<h2>Delete Article</h2>
<pre><code>DELETE /articles/{articleId}</code></pre>
<p>Moves the article to the Recycle Bin (not permanently deleted). Returns 204 No Content on success.</p>

<h2>Required Scopes</h2>
<ul>
<li>List/Get: <code>read:articles</code></li>
<li>Create/Update: <code>write:articles</code></li>
<li>Delete: <code>delete:articles</code></li>
</ul>