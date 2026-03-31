---
title: "AI Usage Dashboard & Cost Tracking"
description: ""
slug: "ai-usage-dashboard-cost-tracking"
status: "PUBLISHED"
createdAt: "2026-02-24T08:32:54.607Z"
updatedAt: "2026-03-12T09:15:11.972Z"
---

<h1>AI Usage Dashboard &amp; Cost Tracking</h1>
<p>The AI Usage Dashboard shows you exactly how much of your AI quota has been used — how many AI requests have been made, how many tokens were consumed, and how that usage breaks down by feature. Use this to monitor consumption and avoid unexpected overages.</p>

<h2>Opening the AI Usage Dashboard</h2>
<ol>
<li>Go to <strong>Settings</strong> in the left sidebar</li>
<li>Click <strong>AI (Ved AI)</strong></li>
<li>Click <strong>AI Usage &amp; Cost Tracking</strong></li>
</ol>

<h2>What You Can See</h2>

<h3>Monthly Usage Summary</h3>
<p>At the top of the page, a progress bar and number show your current month's AI usage versus your plan's monthly limit:</p>
<ul>
<li><strong>Tokens used this month</strong> — Total tokens consumed across all AI features</li>
<li><strong>Requests made</strong> — Number of individual AI calls</li>
<li><strong>Remaining quota</strong> — How much you have left for this billing period</li>
</ul>

<h3>Usage by Feature</h3>
<p>A breakdown table shows how AI usage is distributed across features:</p>
<table>
<thead><tr><th>Feature</th><th>What It Tracks</th></tr></thead>
<tbody>
<tr><td><strong>AI Writer Assistant</strong></td><td>Tokens used by Improve, Summarize, Expand, Translate commands in the editor</td></tr>
<tr><td><strong>Ved AI Chatbot</strong></td><td>Tokens used answering reader questions on the public KB</td></tr>
<tr><td><strong>AI Optimizer</strong></td><td>Tokens used for article optimization suggestions</td></tr>
<tr><td><strong>Embeddings</strong></td><td>Tokens used to generate vector embeddings for semantic search</td></tr>
<tr><td><strong>Translation</strong></td><td>Tokens used for one-click article translation</td></tr>
<tr><td><strong>Video Scripts</strong></td><td>Tokens used generating scripts for Video Studio</td></tr>
</tbody>
</table>

<h3>Usage History Chart</h3>
<p>A line chart shows daily AI usage over the past 30 days. Spot days with spikes to understand what drove usage (e.g., a bulk embed operation or heavy chatbot activity from a traffic spike).</p>

<h2>Usage Limits and Overage</h2>
<p>When you approach your plan's limit:</p>
<ul>
<li>At <strong>80%</strong> — A warning banner appears on the AI Usage Dashboard</li>
<li>At <strong>100%</strong> — AI features are rate-limited. Writer AI responses may be slower or unavailable. Chatbot continues at reduced capacity</li>
<li>After the billing period resets — Quota refreshes to the full monthly allowance</li>
</ul>
<p>To increase your AI quota, upgrade your plan in <strong>Settings → Billing</strong>.</p>

<h2>Bringing Your Own API Key</h2>
<p>If you want unlimited AI usage without quota restrictions, configure your own OpenAI API key. See the <strong>AI API Keys (Bring Your Own Key)</strong> article for setup instructions. Using your own key bypasses FinalDoc's quota system — you pay OpenAI directly.</p>