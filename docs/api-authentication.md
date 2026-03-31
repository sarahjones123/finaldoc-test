---
title: "API Authentication"
description: "How to authenticate with the FinalDoc API using tokens and manage API security."
slug: "api-authentication"
status: "PUBLISHED"
createdAt: "2026-02-24T05:06:00.749Z"
updatedAt: "2026-03-27T10:29:46.727Z"
---

<h1>API Authentication</h1>
<p>All FinalDoc API endpoints require authentication. This article explains how authentication works, how to obtain tokens, and how to include them in your API requests.</p>

<h2>Token Types</h2>

<h3>Session Tokens (fd_)</h3>
<p>Session tokens start with <code>fd_</code> and represent a logged-in user session. They have full admin permissions for the accounts and projects that user can access.</p>
<p>To get a session token: Log in to FinalDoc, then go to <strong>Settings → Data &amp; Compliance → API Tokens → Create Token → Standard token</strong>.</p>

<h3>API Tokens (api_)</h3>
<p>API tokens start with <code>api_</code> and are scoped to specific permissions. Use these for integrations and automation where you want least-privilege access.</p>
<p>Scopes available:</p>
<ul>
<li><code>read:articles</code> — Read article content and metadata</li>
<li><code>write:articles</code> — Create and update articles</li>
<li><code>delete:articles</code> — Delete articles</li>
</ul>
<p>To create an API token: <strong>Settings → Data &amp; Compliance → API Tokens → Create Token → API token (scoped)</strong>.</p>

<h2>Using Tokens in Requests</h2>
<p>Include your token in the <code>Authorization</code> header as a Bearer token:</p>
<pre><code>curl -H "Authorization: Bearer fd_your_token_here"   https://app.finaldoc.io/api/projects</code></pre>

<p>In JavaScript (fetch):</p>
<pre><code>const response = await fetch('https://app.finaldoc.io/api/projects', {
  headers: {
    'Authorization': 'Bearer fd_your_token_here',
    'Content-Type': 'application/json'
  }
});</code></pre>

<h2>Token Expiry</h2>
<ul>
<li><strong>Session tokens</strong> — Expire after 24 hours of inactivity</li>
<li><strong>API tokens</strong> — Do not expire (valid until manually revoked)</li>
</ul>

<h2>Revoking Tokens</h2>
<p>Go to <strong>Settings → Data &amp; Compliance → API Tokens</strong>, find the token, and click <strong>Revoke</strong>. Revoked tokens immediately return 401 Unauthorized on any request.</p>

<h2>401 Unauthorized Errors</h2>
<p>If you receive a 401 error:</p>
<ul>
<li>Check that the token is included in the Authorization header</li>
<li>Check that the token starts with <code>fd_</code> or <code>api_</code></li>
<li>Check that the token has not been revoked</li>
<li>For session tokens: they may have expired — generate a new one</li>
</ul>

<h2>403 Forbidden Errors</h2>
<p>If you receive 403:</p>
<ul>
<li>Your token is valid but lacks permission for this operation</li>
<li>For API tokens: check that the required scope is enabled (e.g., write:articles for creating articles)</li>
<li>For session tokens: you may not have admin access to this project</li>
</ul>

<h2>Security Best Practices</h2>
<ul>
<li>Never put tokens in client-side JavaScript — they can be extracted by anyone</li>
<li>Store tokens in environment variables, not in source code</li>
<li>Use API tokens (scoped) instead of session tokens whenever possible — limit the blast radius if a token is leaked</li>
<li>Rotate tokens periodically, especially if you suspect a leak</li>
</ul>