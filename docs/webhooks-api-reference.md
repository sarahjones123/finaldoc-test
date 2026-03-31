---
title: "Webhooks API Reference"
description: "Reference for configuring and using webhooks to receive real-time event notifications."
slug: "webhooks-api-reference"
status: "PUBLISHED"
createdAt: "2026-02-24T05:06:09.095Z"
updatedAt: "2026-03-27T10:29:46.727Z"
---

<h1>Webhooks API Reference</h1>
<p>The Webhooks API lets you programmatically manage webhook subscriptions — create, list, test, update, and delete webhook endpoints.</p>

<h2>List Webhooks</h2>
<pre><code>GET /projects/{projectId}/webhooks</code></pre>

<p><strong>Example response:</strong></p>
<pre><code>{
  "webhooks": [
    {
      "id": "wh_abc",
      "url": "https://your-server.com/finaldoc-hook",
      "events": ["article.published", "feedback.received"],
      "active": true,
      "secret": "whs_hidden",
      "createdAt": "2026-02-01T10:00:00Z",
      "lastTriggeredAt": "2026-03-11T09:15:00Z",
      "successRate": 0.98
    }
  ]
}</code></pre>

<h2>Create Webhook</h2>
<pre><code>POST /projects/{projectId}/webhooks</code></pre>

<p><strong>Request body:</strong></p>
<pre><code>{
  "url": "https://your-server.com/finaldoc-hook",
  "events": ["article.published", "article.updated", "feedback.received"],
  "secret": "your-signing-secret"
}</code></pre>

<p><strong>Available events:</strong></p>
<ul>
<li><code>article.created</code> — New article created</li>
<li><code>article.updated</code> — Article content changed</li>
<li><code>article.published</code> — Article status changed to published</li>
<li><code>article.unpublished</code> — Article moved back to draft</li>
<li><code>article.deleted</code> — Article moved to recycle bin</li>
<li><code>feedback.received</code> — New reader feedback received (thumbs up or down)</li>
<li><code>search.performed</code> — Search query performed on your KB (high volume)</li>
<li><code>category.created</code> — New category created</li>
<li><code>category.updated</code> — Category renamed or moved</li>
<li><code>version.published</code> — KB version (workspace) published</li>
<li><code>reader.registered</code> — New reader account created</li>
</ul>

<h2>Test Webhook</h2>
<pre><code>POST /projects/{projectId}/webhooks/{webhookId}/test</code></pre>
<p>Sends a test payload to the webhook URL with event type <code>webhook.test</code>. Returns the HTTP response your server returned, so you can verify your endpoint is receiving correctly.</p>

<h2>Update Webhook</h2>
<pre><code>PUT /projects/{projectId}/webhooks/{webhookId}</code></pre>
<p>Update URL, events list, secret, or active status.</p>

<p><strong>Pausing a webhook:</strong></p>
<pre><code>{ "active": false }</code></pre>

<h2>Delete Webhook</h2>
<pre><code>DELETE /projects/{projectId}/webhooks/{webhookId}</code></pre>
<p>Permanently removes the webhook. Returns 204 No Content.</p>

<h2>Webhook Payload Verification</h2>
<p>Every webhook request includes an <code>X-FinalDoc-Signature</code> header containing an HMAC-SHA256 signature of the request body using your webhook secret. Verify it server-side:</p>
<pre><code>const crypto = require('crypto');
const signature = req.headers['x-finaldoc-signature'];
const expectedSig = 'sha256=' + crypto
  .createHmac('sha256', YOUR_WEBHOOK_SECRET)
  .update(JSON.stringify(req.body))
  .digest('hex');
if (signature !== expectedSig) {
  return res.status(401).send('Invalid signature');
}</code></pre>

<h2>Delivery &amp; Retries</h2>
<p>FinalDoc delivers webhook events with at most 3 retry attempts (at 5min, 30min, and 2hr intervals) if your server returns a non-2xx response or times out. After 3 failures, the event is marked as permanently failed and no further retries occur.</p>