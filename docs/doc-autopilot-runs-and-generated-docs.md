---
title: "Runs and Generated Documents"
description: ""
slug: "doc-autopilot-runs-and-generated-docs"
status: "PUBLISHED"
createdAt: "2026-02-24T18:29:42.084Z"
updatedAt: "2026-03-27T10:59:45.835Z"
---

<h1>Runs and Generated Documents</h1>


<p>Doc Autopilot runs are triggered events — each time Autopilot detects a source change, processes it, and generates documentation, that's a Run. This article describes how Runs work and how to manage generated documents.</p>

<h2>What Triggers a Run</h2>
<ul>
<li>A commit is merged to a monitored branch</li>
<li>A new version is added to a changelog</li>
<li>A Jira issue transitions to Done with a docs label</li>
<li>An OpenAPI spec diff is detected at the monitored URL</li>
<li>Manual trigger: clicking "Run Now" in the Autopilot dashboard</li>
</ul>

<h2>Run Stages</h2>
<p>Each Run goes through these stages:</p>
<ol>
<li><strong>Detection</strong> — Source change is detected and queued</li>
<li><strong>Analysis</strong> — AI analyzes the change to understand its documentation impact</li>
<li><strong>Generation</strong> — AI drafts new or updated article content</li>
<li><strong>Review Queue</strong> — Draft appears in the review queue for human approval</li>
<li><strong>Published</strong> (after human approval) — Article is published to the KB</li>
</ol>

<h2>Generated Document Types</h2>

<h3>New Article Draft</h3>
<p>For new features detected in source changes, Autopilot creates a new draft article in your Documentation workspace. The draft includes AI-generated content describing the feature based on the commit/issue description.</p>

<h3>Article Update</h3>
<p>For changes to existing features, Autopilot identifies the existing article and suggests specific changes. The changes appear as tracked edits — you review what the AI wants to add, modify, or remove before accepting.</p>

<h3>Release Notes</h3>
<p>From changelog files, Autopilot generates a structured "Release Notes" article with sections for new features, improvements, and bug fixes — automatically formatted and categorized.</p>

<h2>Managing Generated Documents</h2>
<p>In the planned Review Queue:</p>
<ul>
<li><strong>Approve</strong> — Publishes the generated draft as-is</li>
<li><strong>Edit then Approve</strong> — Opens the draft in the editor for manual edits before publishing</li>
<li><strong>Reject</strong> — Discards the generated draft (with optional feedback to improve future generation)</li>
<li><strong>Merge with existing</strong> — If Autopilot generated a new article about a topic you've already covered, merge the generated content into the existing article</li>
</ul>

<h2>Generation History</h2>
<p>A planned log shows all Autopilot runs — what was detected, what was generated, what was approved or rejected, and by whom. Useful for auditing AI-generated content and ensuring documentation quality standards are maintained.</p>