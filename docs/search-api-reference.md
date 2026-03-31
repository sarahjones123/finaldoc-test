---
title: "Search API Reference"
description: "Reference for the Search API — full-text search, filters, and public search endpoints."
slug: "search-api-reference"
status: "PUBLISHED"
createdAt: "2026-02-24T05:06:05.938Z"
updatedAt: "2026-03-27T10:29:46.727Z"
---

<h1>Search API Reference</h1>
<p>The Search API lets you programmatically search your knowledge base articles. Use it to build custom search interfaces, power your own site search, or integrate FinalDoc article search into another tool.</p>

<h2>Search Articles</h2>
<pre><code>GET /public/kb/{projectSlug}/search</code></pre>
<p>Public endpoint — no authentication required for public knowledge bases.</p>

<p><strong>Query parameters:</strong></p>
<ul>
<li><code>q</code> — The search query (required)</li>
<li><code>limit</code> — Max results (default 10, max 50)</li>
<li><code>categoryId</code> — Restrict search to a specific category</li>
<li><code>language</code> — Language code to filter results (e.g., <code>en</code>, <code>fr</code>)</li>
</ul>

<p><strong>Example:</strong></p>
<pre><code>GET /public/kb/my-project/search?q=password+reset&amp;limit=5</code></pre>

<p><strong>Example response:</strong></p>
<pre><code>{
  "results": [
    {
      "id": "art123",
      "title": "How to Reset Your Password",
      "slug": "how-to-reset-password",
      "description": "Step-by-step guide to reset your account password",
      "categoryName": "Account Management",
      "url": "/article/how-to-reset-password",
      "excerpt": "...click Forgot Password on the login page...",
      "score": 0.95
    }
  ],
  "total": 3,
  "query": "password reset",
  "searchType": "keyword"
}</code></pre>

<h2>Authenticated Search (Private KB)</h2>
<pre><code>GET /kb/{projectSlug}/search</code></pre>
<p>For private knowledge bases, include the reader's authentication token:</p>
<pre><code>Authorization: Bearer reader_token_here</code></pre>

<h2>Semantic (AI) Search</h2>
<p>When the standard search returns 0 results, FinalDoc automatically falls back to semantic search. The <code>searchType</code> field in the response indicates which search type was used:</p>
<ul>
<li><code>"keyword"</code> — Standard full-text search matched</li>
<li><code>"semantic"</code> — AI semantic search was used (no keyword matches found)</li>
<li><code>"fuzzy"</code> — Fuzzy matching was used</li>
</ul>

<h2>Search Suggestions (Autocomplete)</h2>
<pre><code>GET /public/kb/{projectSlug}/search/suggest?q={partial_query}</code></pre>
<p>Returns up to 5 article title suggestions as the user types. Use this to build a typeahead search box.</p>

<p><strong>Example response:</strong></p>
<pre><code>{
  "suggestions": [
    { "title": "Password Reset Guide", "slug": "password-reset-guide" },
    { "title": "Password Requirements", "slug": "password-requirements" }
  ]
}</code></pre>

<h2>Rate Limits</h2>
<p>The public search endpoint is rate-limited to 60 requests per minute per IP address. For higher limits, use authenticated requests with an API token.</p>