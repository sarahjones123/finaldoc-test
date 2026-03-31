---
title: "Microsoft Teams Integration"
description: ""
slug: "microsoft-teams-integration"
status: "PUBLISHED"
createdAt: "2026-02-24T08:32:54.657Z"
updatedAt: "2026-03-12T09:02:15.508Z"
---

<h1>Microsoft Teams Integration</h1>
<p>FinalDoc integrates with Microsoft Teams via an Outgoing Webhook. Your team members can ask documentation questions directly in a Teams channel by mentioning the FinalDoc bot — the AI searches your knowledge base and replies with an answer, right inside Teams.</p>

<h2>How It Works</h2>
<ol>
<li>A team member types a question in a Teams channel and @mentions the FinalDoc bot (e.g., "@FinalDoc How do I reset a user's password?")</li>
<li>Teams sends the message to FinalDoc via a webhook</li>
<li>FinalDoc's AI searches your knowledge base and formulates an answer</li>
<li>The answer is posted back in the Teams channel as a reply from the bot</li>
</ol>

<h2>Setting Up the Integration</h2>
<h3>Step 1: Configure in FinalDoc</h3>
<ol>
<li>Go to <strong>Settings → Integrations → Extensions</strong></li>
<li>Find <strong>Microsoft Teams</strong> and click <strong>Configure</strong></li>
<li>Note the <strong>Webhook Endpoint URL</strong> that FinalDoc provides — you will need this in Teams</li>
</ol>

<h3>Step 2: Create the Outgoing Webhook in Teams</h3>
<ol>
<li>Open Microsoft Teams and go to the team where you want the bot to work</li>
<li>Click the <strong>three-dot menu</strong> next to the team name</li>
<li>Go to <strong>Manage team</strong></li>
<li>Click the <strong>Apps</strong> tab</li>
<li>At the bottom of the Apps page, click <strong>Create an outgoing webhook</strong></li>
<li>Fill in the form:
  <ul>
    <li><strong>Name</strong>: "FinalDoc" (this is the @mention name)</li>
    <li><strong>Callback URL</strong>: Paste the Webhook Endpoint URL from FinalDoc</li>
    <li><strong>Description</strong>: "FinalDoc knowledge base AI"</li>
  </ul>
</li>
<li>Click <strong>Create</strong></li>
<li>Teams shows you an <strong>HMAC security token</strong> — copy it</li>
</ol>

<h3>Step 3: Add the HMAC Token to FinalDoc</h3>
<ol>
<li>Back in FinalDoc, paste the HMAC security token into the <strong>Teams HMAC Secret</strong> field</li>
<li>Click <strong>Save</strong></li>
<li>The integration is now active</li>
</ol>

<h2>Using the Bot in Teams</h2>
<ul>
<li>In any channel where the outgoing webhook is enabled, type your question with @FinalDoc at the start: <strong>@FinalDoc How do I export to PDF?</strong></li>
<li>The bot replies with an answer pulled from your knowledge base</li>
<li>The reply includes a link to the full article for more detail</li>
</ul>

<h2>Security</h2>
<p>All incoming webhooks from Teams are verified using HMAC-SHA256 signatures before being processed. This prevents unauthorized requests from reaching your knowledge base.</p>