---
title: "Article Publishing Workflow"
description: "Learn about article status lifecycle, publishing, unpublishing, and draft management in FinalDoc."
slug: "article-publishing-workflow"
status: "PUBLISHED"
createdAt: "2026-02-24T05:48:14.283Z"
updatedAt: "2026-03-27T10:59:45.779Z"
---

<h1>Article Publishing Workflow</h1>
<p>FinalDoc uses a straightforward draft-to-publish workflow. You write in private (draft mode), then publish when ready. You can also use an optional multi-step approval flow if your team requires content review before articles go live.</p>

<h2>Article Statuses</h2>
<table>
<thead><tr><th>Status</th><th>Visible to Readers?</th><th>What It Means</th></tr></thead>
<tbody>
<tr><td><strong>Draft</strong></td><td>No</td><td>Work in progress. Only team members with access can see it in the admin panel</td></tr>
<tr><td><strong>In Review</strong></td><td>No</td><td>Submitted for approval via the Approval Flow workflow. Awaiting reviewer sign-off</td></tr>
<tr><td><strong>Published</strong></td><td>Yes</td><td>Live on the public knowledge base. Readers can find and read it</td></tr>
<tr><td><strong>Archived</strong></td><td>No</td><td>Removed from public view but kept in the database. Useful for outdated content you may need again</td></tr>
</tbody>
</table>

<h2>Simple Publish (No Approval Required)</h2>
<p>By default, any Editor or above can publish directly without approval:</p>
<ol>
<li>Open the article in the Documentation editor</li>
<li>Write and format your content</li>
<li>Optionally add a description, tags, and featured image in the right Inspector panel</li>
<li>Click the <strong>Publish</strong> button in the top-right of the editor</li>
<li>The status changes from <strong>Draft</strong> to <strong>Published</strong></li>
<li>The article immediately appears on your public knowledge base</li>
</ol>

<h2>Unpublishing an Article</h2>
<p>To remove an article from public view without deleting it:</p>
<ol>
<li>Open the article</li>
<li>Click the green <strong>Published</strong> status badge near the top</li>
<li>Select <strong>Set to Draft</strong> from the dropdown</li>
<li>The article returns to draft state and disappears from the public KB immediately</li>
</ol>

<h2>Approval Flow (Multi-Step Review)</h2>
<p>If your organization requires content review before publishing, enable the <strong>Approval Flow</strong> in the Toolbox:</p>
<ol>
<li>Go to <strong>Toolbox → Approval Flow</strong> in the left sidebar</li>
<li>Create a workflow with one or more review stages (e.g., "Technical Review" → "Editorial Review")</li>
<li>Assign reviewers (team members) to each stage</li>
</ol>
<p>Once an Approval Flow is active for your project:</p>
<ul>
<li><strong>Authors</strong> click "Submit for Review" instead of "Publish"</li>
<li>Assigned reviewers receive a notification to review the article</li>
<li>Reviewers approve or reject each stage</li>
<li>Once all stages are approved, the article can be published by an Editor or Admin</li>
</ul>

<h2>Scheduled Publishing</h2>
<p>You can schedule an article to publish automatically at a future date and time:</p>
<ol>
<li>Open the article</li>
<li>In the Inspector panel, find <strong>Publish Date</strong></li>
<li>Set the date and time you want it to go live</li>
<li>Click <strong>Schedule</strong> — the status changes to "Scheduled"</li>
<li>At the specified time, the system automatically publishes the article</li>
</ol>

<h2>Review Reminders</h2>
<p>Articles can fall out of date over time. Use <strong>Review Reminders</strong> (in Toolbox → Content Review) to set periodic review dates for your articles. When a review date arrives, assigned team members get notified to check and update the article content.</p>

<h2>Bulk Publishing</h2>
<p>To publish multiple articles at once:</p>
<ol>
<li>In Documentation view, click the <strong>Bulk Select</strong> checkbox</li>
<li>Check each article you want to publish</li>
<li>Click <strong>Publish All</strong> in the bulk action bar that appears</li>
<li>All selected draft articles are published simultaneously</li>
</ol>

<h2>Notifications on Publish</h2>
<p>When an article is published, FinalDoc can automatically trigger webhook events or Slack/email notifications. Configure these in <strong>Settings → Integrations → Automation → Webhook Subscriptions &amp; Subscriptions</strong>.</p>