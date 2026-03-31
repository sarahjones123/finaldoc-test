---
title: "Workflow Designer & Approval Flow"
description: ""
slug: "workflow-designer-approval-flow"
status: "PUBLISHED"
createdAt: "2026-02-24T08:37:07.741Z"
updatedAt: "2026-03-19T09:29:33.594Z"
---

<h1>Workflow Designer and Approval Flow</h1>
<p>The Approval Flow tool lets you create structured content review workflows. Instead of authors publishing directly, articles pass through one or more review stages — each requiring a designated reviewer to approve before the article can proceed. This ensures content quality, accuracy, and consistency.</p>

<h2>When to Use Approval Flows</h2>
<ul>
<li>Your documentation affects compliance, safety, or legal obligations</li>
<li>You have junior authors whose work needs review before going live</li>
<li>Technical content must be verified by subject matter experts</li>
<li>Your organization requires an audit trail of who approved what</li>
</ul>

<h2>Opening the Workflow Designer</h2>
<ol>
<li>Go to <strong>Toolbox</strong> in the left sidebar</li>
<li>Under <strong>Content</strong>, click <strong>Approval Flow</strong></li>
</ol>

<h2>Creating a Workflow</h2>
<ol>
<li>Click <strong>New Workflow</strong></li>
<li>Give the workflow a name (e.g., "Standard Article Review" or "Technical Documentation")</li>
<li>Add review <strong>stages</strong> — each stage is a checkpoint that requires approval before moving on:
  <ul>
    <li>Click <strong>Add Stage</strong></li>
    <li>Name the stage (e.g., "Technical Review", "Editorial Review", "Legal Approval")</li>
    <li>Assign one or more <strong>reviewers</strong> from your team members</li>
    <li>Choose if any one reviewer is enough to approve, or if all must approve</li>
  </ul>
</li>
<li>Add more stages if needed. The stages run in the order listed, from top to bottom</li>
<li>Click <strong>Save Workflow</strong></li>
</ol>

<h2>How the Approval Flow Works</h2>
<p>Once a workflow is set up and assigned to your project, the publishing process changes:</p>
<ol>
<li><strong>Draft Writer</strong> finishes writing and clicks <strong>Submit for Review</strong></li>
<li>The article moves to "In Review" status and the first stage's reviewers are notified</li>
<li>Each reviewer opens the article, reads it, and clicks <strong>Approve</strong> or <strong>Request Changes</strong></li>
<li>If changes are requested, the author is notified, makes edits, and resubmits</li>
<li>Once the first stage is approved, the article moves to the second stage (if any)</li>
<li>After all stages are approved, an Editor or Admin can click <strong>Publish</strong></li>
</ol>

<h2>Reviewer Notifications</h2>
<p>Reviewers receive notifications when:</p>
<ul>
<li>An article enters their review stage</li>
<li>An article is resubmitted after changes were requested</li>
</ul>
<p>Notifications appear in the bell icon in the top navigation and can also be sent by email (configure in Settings → General → Notifications).</p>

<h2>Bypassing the Workflow</h2>
<p>Admins and Owners can always publish directly, bypassing the workflow. This is useful for urgent updates or corrections that cannot wait for the full review cycle.</p>

<h2>Multiple Workflows</h2>
<p>You can create multiple workflows for different purposes — for example, a fast single-stage workflow for blog posts and a rigorous three-stage workflow for compliance-sensitive documentation. You can assign different workflows to different categories.</p>