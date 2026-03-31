---
title: "Connecting Ticket Sources"
description: ""
slug: "connecting-ticket-sources"
status: "PUBLISHED"
createdAt: "2026-02-24T18:29:42.044Z"
updatedAt: "2026-03-18T18:57:36.955Z"
---

<h1>Connecting Ticket Sources</h1>
<p>Ticket Analysis works by importing support tickets from your helpdesk into FinalDoc, where the AI analyzes them to find common issues, documentation gaps, and deflection opportunities. The first step is connecting your helpdesk as a ticket source.</p>

<h2>Opening Ticket Analysis</h2>
<ol>
<li>Click <strong>Ticket Analysis</strong> in the left sidebar (the headset/support icon)</li>
</ol>

<h2>Supported Ticket Sources</h2>
<table>
<thead><tr><th>Source</th><th>Integration Type</th></tr></thead>
<tbody>
<tr><td><strong>Zendesk</strong></td><td>Native API integration — connect with your Zendesk subdomain and API token</td></tr>
<tr><td><strong>Intercom</strong></td><td>Native API integration — connect with your Intercom access token</td></tr>
<tr><td><strong>Freshdesk</strong></td><td>Native API integration — connect with your Freshdesk domain and API key</td></tr>
<tr><td><strong>CSV Upload</strong></td><td>Upload a CSV export of your tickets (works with any helpdesk)</td></tr>
<tr><td><strong>Manual Entry</strong></td><td>Type or paste ticket content directly</td></tr>
</tbody>
</table>

<h2>Connecting Zendesk</h2>
<ol>
<li>In Ticket Analysis, click <strong>Connect Source</strong></li>
<li>Select <strong>Zendesk</strong></li>
<li>Enter your <strong>Zendesk subdomain</strong> (the part before .zendesk.com)</li>
<li>Enter your <strong>Zendesk email</strong> and <strong>API token</strong>
  <ul>
    <li>To get your API token: Zendesk Admin → Apps &amp; Integrations → APIs → Zendesk API → API token</li>
  </ul>
</li>
<li>Click <strong>Connect</strong></li>
<li>FinalDoc tests the connection and confirms it can access your tickets</li>
</ol>

<h2>Connecting Intercom</h2>
<ol>
<li>Click <strong>Connect Source → Intercom</strong></li>
<li>You'll be redirected to Intercom's OAuth authorization page</li>
<li>Click <strong>Authorize</strong> to grant FinalDoc read access to your conversations</li>
<li>You're redirected back to FinalDoc with the connection active</li>
</ol>

<h2>Connecting via CSV Upload</h2>
<p>If your helpdesk isn't natively supported, export your tickets as a CSV and upload it:</p>
<ol>
<li>Click <strong>Connect Source → CSV Upload</strong></li>
<li>Click <strong>Upload CSV file</strong></li>
<li>Map columns: Tell FinalDoc which column contains the ticket subject, which has the ticket body, and optionally which has the status/date</li>
<li>Click <strong>Import</strong></li>
</ol>
<p>Your CSV should have at minimum a column with the ticket subject or question and a column with the conversation body.</p>

<h2>Ticket Import Scope</h2>
<p>When connecting a live helpdesk (Zendesk, Intercom, etc.), you can configure the import scope:</p>
<ul>
<li><strong>Date range</strong> — Import tickets from the last 30, 90, 180, or 365 days</li>
<li><strong>Status</strong> — Import only Closed tickets (resolved issues, most useful for analysis) or all statuses</li>
<li><strong>Tags/Groups</strong> — Filter to specific ticket groups or tags if your helpdesk uses them</li>
</ul>
<p>Start with the last 90 days of closed tickets. This gives a good sample without overwhelming the analysis.</p>