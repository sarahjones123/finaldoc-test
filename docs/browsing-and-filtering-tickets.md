---
title: "Browsing and Filtering Tickets"
description: ""
slug: "browsing-and-filtering-tickets"
status: "PUBLISHED"
createdAt: "2026-02-24T18:29:42.054Z"
updatedAt: "2026-03-21T03:07:11.685Z"
---

<h1>Browsing and Filtering Tickets</h1>
<p>Beyond the AI analysis overview, you can browse your individual imported tickets in the Ticket Analysis section. This lets you read the actual support conversations to understand specific issues in detail — useful when the AI flags a topic but you want to understand the context.</p>

<h2>The Ticket Browser</h2>
<ol>
<li>Click <strong>Ticket Analysis</strong> in the left sidebar</li>
<li>Click the <strong>Tickets</strong> tab (or click a topic in the analysis results to jump to filtered tickets for that topic)</li>
</ol>
<p>You'll see a list of all imported tickets with:</p>
<ul>
<li>Ticket subject/title</li>
<li>Source (Zendesk, Intercom, etc.)</li>
<li>Date submitted</li>
<li>AI-assigned topic label</li>
<li>Has documentation gap badge (if this ticket represents a gap)</li>
</ul>

<h2>Filtering Tickets</h2>
<p>Use the filter bar to narrow the ticket list:</p>
<ul>
<li><strong>Topic</strong> — Show only tickets tagged with a specific AI topic label</li>
<li><strong>Source</strong> — Filter by ticket source if you have multiple connected</li>
<li><strong>Date range</strong> — Focus on a specific time period</li>
<li><strong>Documentation gap</strong> — Show only tickets that are documentation gaps vs. all tickets</li>
<li><strong>Search</strong> — Full-text search within ticket subjects and bodies</li>
</ul>

<h2>Reading a Ticket</h2>
<p>Click any ticket to open the full conversation view:</p>
<ul>
<li>The full ticket subject and body text</li>
<li>The AI-assigned topic label and confidence score</li>
<li>Whether this ticket indicates a documentation gap</li>
<li>Related KB articles that the AI found relevant to this ticket's topic</li>
<li>A <strong>Create Article Draft</strong> button to generate a draft article addressing this ticket's issue</li>
</ul>

<h2>Exporting Tickets</h2>
<p>Click <strong>Export CSV</strong> in the Tickets view to download all currently visible (filtered) tickets as a CSV file. Useful for sharing with a team member or analyzing in Excel/Sheets.</p>

<h2>Privacy and Data Handling</h2>
<p>Imported ticket data is stored in your FinalDoc database and treated with the same data security as your other content. Ticket content is sent to OpenAI's API during analysis — the same AI processing that happens when you use Writer AI. If tickets contain sensitive customer data (PII), consider anonymizing them before import. See the AI Compliance article for more details.</p>