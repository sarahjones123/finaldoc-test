---
title: "Webhook Events & Subscriptions"
description: "Subscribe to event types and receive real-time HTTP notifications when things happen in your project."
slug: "webhook-events-subscriptions"
status: "PUBLISHED"
createdAt: "2026-02-27T10:22:41.004Z"
updatedAt: "2026-03-27T10:59:45.789Z"
---

<h1>Webhook Events and Subscriptions</h1>
<p>Webhooks let FinalDoc send real-time HTTP POST notifications to any URL when specific events happen in your knowledge base. Use webhooks to integrate FinalDoc with your own backend systems, trigger automation pipelines (Zapier, Make), post updates to custom dashboards, or sync content changes to external tools.</p>

<h2>Opening Webhook Settings</h2>
<ol>
<li>Go to <strong>Settings → Integrations → Automation &amp; Subscriptions</strong></li>
</ol>

<h2>Creating a Webhook</h2>
<ol>
<li>Click <strong>+ Add Webhook</strong></li>
<li>Enter the <strong>Endpoint URL</strong> — the HTTPS URL where FinalDoc will send POST requests</li>
<li>Enter a <strong>Secret</strong> (optional but recommended) — used to sign payloads with HMAC-SHA256 so your server can verify the request came from FinalDoc</li>
<li>Select which <strong>events</strong> should trigger this webhook (see event list below)</li>
<li>Click <strong>Save</strong></li>
<li>Click <strong>Send Test Event</strong> to verify your endpoint is receiving events correctly</li>
</ol>

<h2>Available Events</h2>
<table>
<thead><tr><th>Event</th><th>Triggered When</th></tr></thead>
<tbody>
<tr><td><code>article.created</code></td><td>A new article is created (in any status)</td></tr>
<tr><td><code>article.updated</code></td><td>A published article's content is saved</td></tr>
<tr><td><code>article.published</code></td><td>An article is moved to Published status</td></tr>
<tr><td><code>article.unpublished</code></td><td>A published article is moved back to Draft</td></tr>
<tr><td><code>article.deleted</code></td><td>An article is moved to the Recycle Bin</td></tr>
<tr><td><code>feedback.received</code></td><td>A reader submits feedback (thumbs up or down) on any article</td></tr>
<tr><td><code>search.performed</code></td><td>A reader performs a search query on your KB (high volume — use with care)</td></tr>
<tr><td><code>category.created</code></td><td>A new category is created</td></tr>
<tr><td><code>category.updated</code></td><td>A category is renamed or moved</td></tr>
<tr><td><code>version.published</code></td><td>A KB version (workspace) is published</td></tr>
<tr><td><code>reader.registered</code></td><td>A new reader creates an account on your KB</td></tr>
</tbody>
</table>

<h2>Webhook Payload Format</h2>
<p>All webhook payloads are JSON with the same wrapper structure:</p>
<pre><code>{
  "event": "article.published",
  "projectId": "proj_abc123",
  "timestamp": "2026-03-12T10:30:00Z",
  "data": {
    "articleId": "art_xyz789",
    "title": "Getting Started with the API",
    "slug": "getting-started-with-the-api",
    "status": "published",
    "categoryId": "cat_abc",
    "authorId": "user_123",
    "updatedAt": "2026-03-12T10:30:00Z"
  }
}</code></pre>

<h2>Verifying Webhook Signatures</h2>
<p>If you set a secret when creating the webhook, FinalDoc includes an <code>X-FinalDoc-Signature</code> header with each request. Verify it on your server to confirm the request came from FinalDoc:</p>
<pre><code>// Node.js example
const crypto = require('crypto');
const signature = req.headers['x-finaldoc-signature'];
const expected = crypto
  .createHmac('sha256', YOUR_WEBHOOK_SECRET)
  .update(JSON.stringify(req.body))
  .digest('hex');
const isValid = signature === expected;</code></pre>

<h2>Delivery and Retries</h2>
<ul>
<li>FinalDoc expects a <strong>2xx HTTP response</strong> within 10 seconds. Anything else is treated as a delivery failure</li>
<li>Failed deliveries are <strong>retried up to 3 times</strong> with exponential backoff (5s, 15s, 45s)</li>
<li>If all retries fail, the delivery is logged as failed</li>
</ul>

<h2>Delivery Logs</h2>
<p>Click any webhook in the list to see its recent delivery history:</p>
<ul>
<li>Timestamp of each delivery attempt</li>
<li>HTTP status code returned</li>
<li>Response body (first 500 characters)</li>
<li>Whether the delivery succeeded or failed</li>
</ul>
<p>Delivery logs help you debug why your endpoint may not be receiving events.</p>

<h2>Disabling and Deleting Webhooks</h2>
<ul>
<li><strong>Disable</strong>: Toggle the webhook off to stop receiving events without deleting the configuration</li>
<li><strong>Delete</strong>: Permanently remove the webhook and all its delivery history</li>
</ul>