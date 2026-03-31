---
title: "Feedback API Reference"
description: ""
slug: "feedback-api-reference"
status: "PUBLISHED"
createdAt: "2026-02-24T08:32:54.573Z"
updatedAt: "2026-03-27T10:29:46.727Z"
---

<h1>Feedback API Reference</h1>
<p>The Feedback API lets you retrieve and manage reader feedback submissions programmatically.</p>

<h2>List Feedback</h2>
<pre><code>GET /projects/{projectId}/feedback</code></pre>

<p><strong>Query parameters:</strong></p>
<ul>
<li><code>rating</code> — Filter by <code>positive</code> or <code>negative</code></li>
<li><code>status</code> — Filter by <code>open</code>, <code>in_progress</code>, <code>resolved</code>, <code>dismissed</code></li>
<li><code>articleId</code> — Filter by specific article</li>
<li><code>startDate</code>, <code>endDate</code> — Date range filter</li>
<li><code>limit</code>, <code>offset</code> — Pagination</li>
</ul>

<p><strong>Example response:</strong></p>
<pre><code>{
  "feedback": [
    {
      "id": "fb_abc",
      "articleId": "art123",
      "articleTitle": "Getting Started",
      "rating": "negative",
      "comment": "The screenshots are outdated",
      "readerEmail": "user@example.com",
      "status": "open",
      "createdAt": "2026-03-10T14:22:00Z"
    }
  ],
  "total": 47
}</code></pre>

<h2>Get Feedback Entry</h2>
<pre><code>GET /projects/{projectId}/feedback/{feedbackId}</code></pre>
<p>Returns a single feedback entry with full details.</p>

<h2>Update Feedback Status</h2>
<pre><code>PATCH /projects/{projectId}/feedback/{feedbackId}</code></pre>

<p><strong>Request body:</strong></p>
<pre><code>{
  "status": "resolved",
  "assigneeId": "user_team_member",
  "note": "Updated screenshots in the article"
}</code></pre>

<h2>Delete Feedback</h2>
<pre><code>DELETE /projects/{projectId}/feedback/{feedbackId}</code></pre>
<p>Permanently deletes the feedback entry. Returns 204 No Content.</p>

<h2>Bulk Update Feedback</h2>
<pre><code>POST /projects/{projectId}/feedback/bulk-update</code></pre>

<p><strong>Request body:</strong></p>
<pre><code>{
  "ids": ["fb_abc", "fb_def", "fb_ghi"],
  "status": "resolved"
}</code></pre>
<p>Updates status for multiple feedback entries at once. Maximum 100 IDs per request.</p>

<h2>Feedback Summary</h2>
<pre><code>GET /projects/{projectId}/feedback/summary</code></pre>
<p>Returns aggregate feedback statistics: total count, positive count, negative count, satisfaction rate, and counts by status.</p>

<h2>Authentication</h2>
<p>Feedback API endpoints require a session token (<code>fd_</code>) with admin access to the project.</p>