---
title: "API Tokens"
description: "Generating developer access tokens for the FinalDoc API."
slug: "api-tokens"
status: "PUBLISHED"
createdAt: "2026-02-23T18:16:38.067Z"
updatedAt: "2026-03-20T20:14:12.815Z"
---

<h1>API Tokens</h1>
<p>API tokens let you access FinalDoc's REST API programmatically — to create, read, update, and delete articles; manage readers; pull analytics data; and more. Use API tokens to build integrations, automate content workflows, or connect FinalDoc to your own tools.</p>

<h2>Opening API Tokens</h2>
<ol>
<li>Go to <strong>Settings → Data &amp; Compliance → API Tokens</strong></li>
</ol>

<h2>Creating an API Token</h2>
<ol>
<li>Click <strong>+ Create Token</strong></li>
<li>Give the token a <strong>name</strong> (describes its purpose, e.g., "Content Sync Script" or "Zapier Integration")</li>
<li>Select the <strong>token type</strong>:
  <ul>
    <li><strong>Standard token</strong> — Uses your account session for all operations (inherits your permissions)</li>
    <li><strong>API token (scoped)</strong> — For the Bulk API with specific read/write/delete permission scopes</li>
  </ul>
</li>
<li>If using a scoped API token, select the allowed scopes:
  <ul>
    <li><code>read:articles</code> — Read article content and metadata</li>
    <li><code>write:articles</code> — Create and update articles</li>
    <li><code>delete:articles</code> — Delete articles</li>
  </ul>
</li>
<li>Click <strong>Create Token</strong></li>
<li>The token value is shown <strong>once</strong> — copy it immediately. After closing the dialog, the full token value is never shown again (only the first few characters as a preview)</li>
</ol>

<div style="border-left: 4px solid #ef4444; border-radius: 8px; padding: 16px; margin: 16px 0; background: rgba(239,68,68,0.08);">
<strong>Security:</strong> Treat API tokens like passwords. Never share them, commit them to source code repositories, or embed them in client-side JavaScript. Store them in environment variables or a secrets manager.
</div>

<h2>Using an API Token</h2>
<p>Include the token in the <code>Authorization</code> header of API requests:</p>
<pre><code>Authorization: Bearer YOUR_TOKEN_HERE</code></pre>
<p>For Bulk API tokens (scoped), the token format is <code>api_xxxxxxxx</code>.</p>

<h2>Token List</h2>
<p>The token list shows all your created tokens with:</p>
<ul>
<li>Token name</li>
<li>Token preview (first 8 characters only)</li>
<li>Date created</li>
<li>Last used date</li>
<li>Scopes (for scoped tokens)</li>
</ul>

<h2>Revoking a Token</h2>
<ol>
<li>Find the token in the list</li>
<li>Click the <strong>Revoke</strong> button (trash icon)</li>
<li>Confirm the revocation</li>
</ol>
<p>Revoked tokens immediately stop working. Any scripts or integrations using that token will start getting 401 Unauthorized errors. Update them with a new token before revoking.</p>

<h2>API Rate Limits</h2>
<p>The Bulk API has a rate limit of <strong>60 requests per minute</strong> per token. Standard session-based API calls do not have explicit rate limits but are subject to fair use policies. If you need higher limits, contact support.</p>

<h2>API Documentation</h2>
<p>Full API documentation is available in the <strong>API Docs</strong> section of FinalDoc. You can also view it on your public knowledge base under the API Reference section if you have published your API spec.</p>