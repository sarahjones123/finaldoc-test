---
title: "Collecting & Managing Feedback"
description: "Set up article feedback, manage submissions, and configure notifications."
slug: "collecting-managing-feedback"
status: "PUBLISHED"
createdAt: "2026-02-24T03:50:57.787Z"
updatedAt: "2026-03-28T18:19:07.395Z"
---

<h1>Collecting &amp; Managing Feedback</h1>
<p>FinalDoc lets your readers leave feedback on articles and report issues. All feedback is collected in the <strong>Feedback</strong> section of the admin panel.</p>

<h2>Enabling Feedback</h2>
<ol>
<li>Go to <strong>Settings &rarr; Appearance &rarr; Article Display</strong></li>
<li>Expand the <strong>Article bottom</strong> section</li>
<li>Toggle <strong>Show feedback form</strong> ON</li>
</ol>
<p>Once enabled, readers see two widgets at the bottom of every published article:</p>
<ul>
<li><strong>"Helpful?"</strong> &mdash; Yes/No buttons. Clicking "Yes" immediately submits positive feedback. Clicking "No" reveals a text field for the reader to explain what was missing</li>
<li><strong>"Report Issue" / "Flag"</strong> &mdash; Opens a panel where readers select an issue type (Wrong Info, Missing Step, Broken Link, Other), optionally add details and a screenshot, then submit</li>
</ul>

<h2>Where Feedback Appears</h2>
<table>
<thead><tr><th>Reader Action</th><th>Admin Tab</th></tr></thead>
<tbody>
<tr><td>Clicks "Yes" (helpful)</td><td>Article Feedback &mdash; shows as positive rating</td></tr>
<tr><td>Clicks "No" (not helpful) + comment</td><td>Article Feedback &mdash; shows as negative rating with comment</td></tr>
<tr><td>Submits a "Report Issue" flag</td><td>Portal Issues &mdash; shows with issue type and details</td></tr>
<tr><td>Rates an AI chatbot response</td><td>Ved AI &rarr; Feedback tab</td></tr>
<tr><td>Asks a question the AI can&rsquo;t answer</td><td>Ved AI &rarr; Unanswered tab</td></tr>
</tbody>
</table>

<h2>Actions on Article Feedback</h2>
<p>Each feedback card has action buttons that appear on hover:</p>
<table>
<thead><tr><th>Button</th><th>What It Does</th></tr></thead>
<tbody>
<tr><td><strong>Edit Article</strong> (pencil icon)</td><td>Opens the specific article in the Documentation editor so you can fix the issue</td></tr>
<tr><td><strong>View Article</strong> (external link icon)</td><td>Opens the article on the public knowledge base in a new tab</td></tr>
<tr><td><strong>Mark Resolved</strong> (checkmark icon)</td><td>Opens a dialog to add an optional resolution note, then marks the feedback as resolved</td></tr>
<tr><td><strong>Create Task</strong> (checklist icon)</td><td>Creates a task on the Home page Tasks card. Negative feedback is automatically marked HIGH priority. Once created, the card shows "Task created &mdash; manage on Home page"</td></tr>
<tr><td><strong>Reply</strong> (message icon)</td><td>Opens a reply dialog to email the reader. Only appears when the reader&rsquo;s email is available (logged-in readers only)</td></tr>
<tr><td><strong>Delete</strong> (trash icon)</td><td>Soft-deletes the feedback with a 5-second undo option</td></tr>
</tbody>
</table>

<h2>Actions on Portal Issues</h2>
<p>Each issue report card has the same set of action buttons:</p>
<table>
<thead><tr><th>Button</th><th>What It Does</th></tr></thead>
<tbody>
<tr><td><strong>Edit Article</strong></td><td>Opens the reported article in the Documentation editor</td></tr>
<tr><td><strong>View Article</strong></td><td>Opens the article on the public KB in a new tab</td></tr>
<tr><td><strong>Create Task</strong></td><td>Creates a HIGH priority task with the issue type and details pre-filled</td></tr>
<tr><td><strong>Mark Resolved / Reopen</strong></td><td>Toggles the issue between resolved and open status</td></tr>
<tr><td><strong>Delete</strong></td><td>Permanently removes the issue report</td></tr>
</tbody>
</table>
<p>Portal issues also have a <strong>status dropdown</strong> (badge in the top-right corner) with four states: New &rarr; In Progress &rarr; Resolved &rarr; Dismissed.</p>

<h2>Creating Tasks from Feedback</h2>
<p>The recommended workflow for handling feedback:</p>
<ol>
<li>Review the feedback in the Feedback inbox</li>
<li>Click <strong>Create Task</strong> on any feedback item that needs attention</li>
<li>Go to <strong>Home</strong> &rarr; <strong>Tasks</strong> card &mdash; feedback tasks show as <strong>F-001</strong>, <strong>F-002</strong>, etc.</li>
<li>Open the task and assign it to the appropriate writer</li>
<li>The writer fixes the article and marks the task as done</li>
<li>Come back to Feedback and mark the item as resolved</li>
</ol>

<h2>Reply to Feedback</h2>
<p>The Reply button only appears on feedback from <strong>logged-in readers</strong> (readers who have an email address). Anonymous feedback cannot be replied to.</p>
<p>When you reply:</p>
<ol>
<li>Click the message icon on a feedback card</li>
<li>Type your response in the reply dialog</li>
<li>Click <strong>Send Reply</strong></li>
<li>The reader receives an email with your response</li>
</ol>

<h2>Ved AI Feedback</h2>
<p>The Ved AI tab has two sub-tabs:</p>
<ul>
<li><strong>Feedback</strong> &mdash; Shows reader ratings on AI chatbot responses (helpful/not helpful)</li>
<li><strong>Unanswered</strong> &mdash; Shows questions the AI could not answer. Use these to identify content gaps and create new articles</li>
</ul>
<p>To enable AI chatbot feedback, go to <strong>Settings &rarr; AI (Ved AI) &rarr; Enable &amp; Configure</strong> and toggle the <strong>Reader Assistant</strong> ON.</p>