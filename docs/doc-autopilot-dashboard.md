---
title: "Doc Autopilot Dashboard"
description: ""
slug: "doc-autopilot-dashboard"
status: "PUBLISHED"
createdAt: "2026-02-24T18:29:42.088Z"
updatedAt: "2026-03-27T10:59:45.828Z"
---

<h1>Doc Autopilot Dashboard</h1>


<p>The Doc Autopilot Dashboard will be the central hub for monitoring automated documentation activity — what changes were detected, what documents were generated or updated, and what still needs human review before publishing.</p>

<h2>Planned Dashboard Sections</h2>

<h3>Activity Feed</h3>
<p>A real-time log of all Autopilot activity:</p>
<ul>
<li>Source event detected (e.g., "GitHub commit abc123 merged to main")</li>
<li>Analysis running (AI reading the commit to identify documentation impact)</li>
<li>Documentation action taken (e.g., "Draft created: 'New Reporting Dashboard feature'")</li>
<li>Review needed (flags that require human approval before publishing)</li>
</ul>

<h3>Pending Review Queue</h3>
<p>Auto-generated documents don't publish automatically — they require review first. The Pending Review Queue shows all AI-generated drafts awaiting human review:</p>
<ul>
<li>Draft title and generated content preview</li>
<li>Source event that triggered the draft</li>
<li>Confidence score (how confident the AI is that this draft is complete and accurate)</li>
<li>Actions: Approve &amp; Publish, Edit First, or Dismiss</li>
</ul>

<h3>Documentation Coverage Map</h3>
<p>A visual map showing which parts of your product are documented vs. undocumented. Features with code changes but no corresponding documentation updates are highlighted as coverage gaps.</p>

<h3>Sources Status</h3>
<p>Status of all connected sources — GitHub repositories, Jira projects, feature flag tools. Shows last sync time, connection health, and any configuration errors.</p>

<h2>Human-in-the-Loop Design</h2>
<p>Doc Autopilot is designed as an AI assistant, not full automation. Every generated document requires a human to review and approve before it appears on your public knowledge base. This ensures accuracy and brand voice consistency — the AI drafts, humans decide.</p>