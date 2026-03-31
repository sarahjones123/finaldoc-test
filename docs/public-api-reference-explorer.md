---
title: "Public API Reference Explorer"
description: ""
slug: "public-api-reference-explorer"
status: "PUBLISHED"
createdAt: "2026-02-24T08:32:54.742Z"
updatedAt: "2026-03-12T09:21:35.632Z"
---

<h1>Public API Reference Explorer</h1>
<p>When you publish API documentation in FinalDoc, your readers get access to a fully interactive API explorer on your public knowledge base. This is not just static documentation — readers can browse your endpoints, fill in parameters, and make real live API calls directly from the documentation page.</p>

<h2>How It Looks to Readers</h2>
<p>Your public API reference has:</p>
<ul>
<li><strong>Left panel</strong> — Endpoint list, organized by tag/group (e.g., "Authentication", "Articles", "Users"). Click any endpoint to jump to it</li>
<li><strong>Main area</strong> — Endpoint detail: HTTP method, path, description, parameters, request body schema, and response schemas</li>
<li><strong>Try It Out</strong> — An interactive panel where readers enter their API key and parameters, then send a real request</li>
<li><strong>Code Examples</strong> — Auto-generated snippets in curl, JavaScript (fetch), Python, PHP, Ruby, and Go</li>
</ul>

<h2>Making the API Reference Public</h2>
<ol>
<li>Go to <strong>API Docs</strong> in the left sidebar</li>
<li>Click on your API specification</li>
<li>Find the <strong>Visibility</strong> setting</li>
<li>Set it to <strong>Published</strong></li>
<li>The API reference is now visible on your public KB under <strong>/api-reference</strong></li>
</ol>

<h2>Authentication in Try It Out</h2>
<p>When readers use "Try It Out," they can enter their own API key in the Authorization section. FinalDoc does not expose or store this key — it's only used in the browser for the live request.</p>
<p>The authentication scheme comes from your OpenAPI spec. If your spec defines <code>Bearer</code> auth, readers see a field to enter their Bearer token. If it defines API key auth, they see the appropriate field.</p>

<h2>Base URL Configuration</h2>
<p>The base URL used for "Try It Out" requests comes from the <code>servers</code> section of your OpenAPI spec. If your API is at <code>https://api.yourcompany.com/v1</code>, include that in your spec's server list. Readers' live requests go directly to your API — they do not go through FinalDoc.</p>

<h2>CORS Requirements for Try It Out</h2>
<p>For Try It Out to work, your API must allow CORS requests from your KB's domain. Add <code>yourproject.finaldoc.io</code> (or your custom domain) to your API's CORS allowed origins. Without this, readers will see CORS errors when trying to make live requests.</p>

<h2>Search Within API Docs</h2>
<p>Readers can search within the API reference — both the standard KB search and the API reference's own search bar (searches endpoint names, descriptions, and parameters). This helps readers with many endpoints find what they need quickly.</p>