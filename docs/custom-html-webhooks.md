---
title: "Custom HTML & Webhooks"
description: "Inject custom HTML/CSS/JavaScript into your knowledge base and set up webhook integrations."
slug: "custom-html-webhooks"
status: "PUBLISHED"
createdAt: "2026-02-23T18:26:56.442Z"
updatedAt: "2026-03-26T19:01:38.965Z"
---

<h1>Custom HTML &amp; Webhooks</h1>
<p>The Custom HTML &amp; Webhooks section lets you add custom HTML blocks to specific areas of your public knowledge base, and configure webhook endpoints that receive event notifications from FinalDoc when things happen in your KB.</p>

<h2>Custom HTML Blocks</h2>
<p>Custom HTML blocks let you inject custom content into specific zones of your KB layout:</p>
<ul>
<li><strong>Above KB header</strong> — Site-wide announcement banner above the navigation bar</li>
<li><strong>Below KB header</strong> — Content between the header and the main KB content</li>
<li><strong>Before article content</strong> — Block shown at the top of every article, before the article body</li>
<li><strong>After article content</strong> — Block shown at the bottom of every article, after the content and before feedback</li>
<li><strong>KB footer</strong> — Content at the very bottom of every KB page</li>
</ul>

<h3>Adding a Custom HTML Block</h3>
<ol>
<li>Go to <strong>Settings → Integrations → Custom Code</strong></li>
<li>Find the zone where you want to add content</li>
<li>Click <strong>Add HTML Block</strong></li>
<li>Enter your HTML (and optionally inline CSS/JS)</li>
<li>Click <strong>Save</strong></li>
</ol>

<h3>Use Cases</h3>
<ul>
<li>Add a promotional banner ("Try our new feature — learn more in the docs")</li>
<li>Add a disclaimer or legal notice before all article content</li>
<li>Embed a calendar widget in the KB footer for booking support calls</li>
<li>Add a custom cookie notice that matches your brand</li>
</ul>

<h2>Webhooks</h2>
<div style="background:#eff6ff;border-left:4px solid #3b82f6;padding:12px 16px;border-radius:4px;margin:16px 0">
  <strong>Webhooks have moved.</strong> Webhook Subscriptions are now configured under <strong>Settings → Integrations → Automation</strong>. See <a href="/article/webhook-events-subscriptions">Webhook Events &amp; Subscriptions</a> for details.
</div>
<p>Webhooks are HTTP POST requests that FinalDoc sends to your server when events occur — article published, feedback received, reader registered, etc. Use webhooks to build custom automation: send feedback to Slack, sync articles to another system, trigger CI/CD when docs are published, etc.</p>

<h3>Setting Up a Webhook</h3>
<ol>
<li>In the Webhooks section, click <strong>+ Add Webhook</strong></li>
<li>Enter the <strong>Endpoint URL</strong> — the URL of your server that will receive the events</li>
<li>Select which <strong>events</strong> to subscribe to</li>
<li>Enter a <strong>Secret</strong> — a random string used to sign webhook payloads so you can verify they came from FinalDoc</li>
<li>Click <strong>Save</strong></li>
</ol>

<p>Your server receives POST requests with a JSON body containing the event data and an <code>X-FinalDoc-Signature</code> header for verification. See the Webhook Events &amp; Subscriptions article for the full event list and payload format.</p>

<h3>Testing a Webhook</h3>
<p>After saving, click <strong>Send Test Event</strong>. FinalDoc sends a test payload to your endpoint. Check your server logs to confirm it was received.</p>