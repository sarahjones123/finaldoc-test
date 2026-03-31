---
title: "Workflow Designer"
description: "Design multi-step approval workflows for content review before publishing."
slug: "workflow-designer"
status: "PUBLISHED"
createdAt: "2026-02-23T18:26:45.685Z"
updatedAt: "2026-03-12T11:15:01.467Z"
---

<h1>Workflow Designer (Approval Flow)</h1>
<p>The Approval Flow (also called Workflow Designer) lets you build multi-step review and approval workflows for your articles. When a writer finishes an article, instead of publishing it immediately, it enters the workflow — moving through review stages (Technical Review, Legal Review, Editorial Review, etc.) before it can be published. Each stage has an assigned reviewer who must approve before the article advances.</p>

<h2>Opening Approval Flow</h2>
<ol>
<li>Click <strong>Toolbox</strong> in the left sidebar</li>
<li>Under <strong>Content</strong>, click <strong>Approval Flow</strong></li>
</ol>

<h2>Creating a Workflow</h2>
<ol>
<li>Click <strong>+ New Workflow</strong></li>
<li>Give the workflow a name (e.g., "Standard Review", "Compliance Review")</li>
<li>Add stages by clicking <strong>+ Add Stage</strong>:
  <ul>
    <li><strong>Stage name</strong> — e.g., "Technical Review", "Manager Approval", "Legal Check"</li>
    <li><strong>Reviewer(s)</strong> — Assign one or more team members who must review at this stage</li>
    <li><strong>Approval type</strong> — <em>Any one</em> (any assigned reviewer can approve) or <em>All</em> (all reviewers must approve)</li>
    <li><strong>SLA</strong> — Optional time limit before auto-escalation (e.g., 48 hours)</li>
  </ul>
</li>
<li>Drag stages to reorder them</li>
<li>Click <strong>Save Workflow</strong></li>
</ol>

<h2>Assigning a Workflow to Articles</h2>
<p>There are two ways to put an article through a workflow:</p>

<h3>Per-Article Assignment</h3>
<ol>
<li>Open the article in the editor</li>
<li>In the Inspector panel, find <strong>Workflow</strong></li>
<li>Select the workflow to assign</li>
<li>Click <strong>Submit for Review</strong></li>
</ol>

<h3>Automatic Assignment by Category</h3>
<ol>
<li>In Approval Flow, click on a workflow → <strong>Auto-Apply Rules</strong></li>
<li>Set up rules: "Apply this workflow to all articles in [category]"</li>
<li>All new articles in that category automatically enter the workflow on creation</li>
</ol>

<h2>The Review Process</h2>
<p>When an article enters a workflow:</p>
<ol>
<li>The assigned reviewer at Stage 1 receives an email notification</li>
<li>They open the article in the editor (read-only mode while in review)</li>
<li>They add comments if needed</li>
<li>They click <strong>Approve</strong> to advance to Stage 2, or <strong>Request Changes</strong> to return to the author</li>
<li>This repeats for each stage</li>
<li>After all stages are approved, the article can be published</li>
</ol>

<h2>Viewing Workflow Status</h2>
<p>In the Documentation sidebar, articles in active workflows show a colored status badge (e.g., "In Review", "Pending Approval"). Click <strong>Toolbox → Approval Flow</strong> to see all articles currently in workflows and their current stage.</p>