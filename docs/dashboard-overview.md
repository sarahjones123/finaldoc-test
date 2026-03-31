---
title: "Dashboard Overview"
description: "Snapshot of your knowledge base's health, recent activity, and key metrics at a glance."
slug: "dashboard-overview"
status: "PUBLISHED"
createdAt: "2026-02-23T18:13:42.804Z"
updatedAt: "2026-03-28T18:19:07.377Z"
---

<h1>Dashboard Overview</h1>
<p>The Dashboard is the first page you see when you log in. It gives you a snapshot of your knowledge base's health, recent activity, and key metrics at a glance.</p>

<h2>Accessing the Dashboard</h2>
<p>Click the <strong>FinalDoc logo</strong> or <strong>Home</strong> icon in the left sidebar at any time to return to the Dashboard.</p>

<h2>Stats Cards (Top Row)</h2>
<table>
<thead><tr><th>Card</th><th>Metric</th><th>What It Means</th></tr></thead>
<tbody>
<tr><td><strong>Total Articles</strong></td><td>Published article count</td><td>Articles in PUBLISHED status across all categories</td></tr>
<tr><td><strong>Total Views (30d)</strong></td><td>Page views</td><td>Unique page views on your public/private KB in the last 30 days</td></tr>
<tr><td><strong>Reader Feedback</strong></td><td>Open items</td><td>Unresolved feedback submissions from readers</td></tr>
<tr><td><strong>Team Members</strong></td><td>Active users</td><td>Team members with access to this project</td></tr>
</tbody>
</table>

<h2>Documents</h2>
<p>The Documents card shows your articles with two tabs:</p>
<ul>
<li><strong>Recent</strong> — Articles sorted by their last real save date (not inflated by view counts). Shows the article title, status, and who last saved it.</li>
<li><strong>Starred</strong> — Articles you have starred/favourited. Star an article in the Documentation editor sidebar to pin it here for quick access.</li>
</ul>
<p>The card displays up to 8 articles with scroll. Click <strong>View all documents</strong> at the bottom to open a slide-over panel showing up to 30 articles. Click any article to open it directly in the editor.</p>

<h2>Activity Heatmap</h2>
<p>A 52-week calendar grid (inspired by GitHub's contribution graph). Each cell is one day:</p>
<ul>
<li><strong>Dark green</strong> — High editing activity</li>
<li><strong>Light green</strong> — Some editing activity</li>
<li><strong>Grey</strong> — No editing activity</li>
</ul>
<p>Hover over any cell to see the date and exact number of article edits. The heatmap helps you identify documentation sprints, gaps, and long-term consistency.</p>

<h2>Contribution Timeline</h2>
<p>A stacked bar chart showing per-author contributions over the past 12 weeks:</p>
<ul>
<li>Each colour represents one team member</li>
<li>Bar height = total edits that week across all authors</li>
<li>Hover a bar segment to see one author's contribution for that week</li>
<li>The legend below shows each author's name and total contributions in the period</li>
</ul>
<p>This is ideal for understanding workload distribution across your writing team.</p>

<h2>Tasks</h2>
<p>A comprehensive task management system designed for documentation teams. The Tasks card supports list and Kanban board views, inline creation, a slide-over detail panel, AI-powered suggestions, bulk actions, and email notifications.</p>

<h3>Task IDs</h3>
<p>Every task has a human-readable ID displayed as a teal badge:</p>
<table>
<thead><tr><th>Prefix</th><th>Task Type</th></tr></thead>
<tbody>
<tr><td><strong>F-001</strong></td><td>Feedback / Issue report tasks</td></tr>
<tr><td><strong>D-001</strong></td><td>Content Review / Content Update</td></tr>
<tr><td><strong>N-001</strong></td><td>New Article</td></tr>
<tr><td><strong>T-001</strong></td><td>Translation</td></tr>
<tr><td><strong>S-001</strong></td><td>SEO Optimization</td></tr>
<tr><td><strong>U-001</strong></td><td>Screenshot Update</td></tr>
<tr><td><strong>L-001</strong></td><td>Link Fix</td></tr>
</tbody>
</table>
<p>IDs are sequential per type and stable &mdash; they do not change when you filter or sort.</p>

<h3>Views</h3>
<table>
<thead><tr><th>View</th><th>Description</th></tr></thead>
<tbody>
<tr><td><strong>List View</strong></td><td>Table with title, type, priority, status, and due date columns. Includes checkboxes for bulk selection.</td></tr>
<tr><td><strong>Board View</strong></td><td>Kanban board with four columns (To Do, In Progress, In Review, Done). Drag-and-drop cards to change status.</td></tr>
</tbody>
</table>
<p>Toggle between views using the list/board icons in the card header. Both views support scrolling when there are more tasks than fit in the card.</p>

<h3>Type Filter</h3>
<p>Use the <strong>type dropdown</strong> (between My/All and List/Board toggles) to filter tasks by type: Content Review, Content Update, New Article, Translation, Screenshot Update, Link Fix, or SEO Optimization.</p>

<h3>Sorting</h3>
<p>In list view, click any <strong>column header</strong> (Title, Type, Priority, Status, Due) to sort. Click once for ascending, click again for descending. The active sort column shows an arrow indicator.</p>

<h3>Filter Tabs</h3>
<table>
<thead><tr><th>Tab</th><th>Shows</th></tr></thead>
<tbody>
<tr><td><strong>All</strong></td><td>Every task assigned to you or created by you</td></tr>
<tr><td><strong>Today</strong></td><td>Tasks with today's due date</td></tr>
<tr><td><strong>Overdue</strong></td><td>Past-due tasks (badge pulses red when overdue tasks exist)</td></tr>
<tr><td><strong>AI</strong></td><td>AI-generated task suggestions. Click <strong>Accept</strong> to convert a suggestion into a real task.</td></tr>
</tbody>
</table>

<h3>My Tasks vs All Tasks</h3>
<p>Use the <strong>My / All</strong> toggle in the card header to switch between tasks assigned to you and all tasks across the team.</p>

<h3>Creating Tasks</h3>
<p>Tasks can be created from multiple places:</p>
<ul>
<li><strong>Dashboard</strong> — Click the green <strong>+</strong> button. Pick title, type, priority, and due date. The form stays open for creating multiple tasks.</li>
<li><strong>Editor</strong> — Click the <strong>Task</strong> button in the editor toolbar. A modal opens with the title pre-filled and the article pre-linked. Choose type (Content Review, Content Update, Translation, Screenshot Update, etc.) and priority.</li>
<li><strong>Feedback</strong> — Click the task icon on any feedback item to create a task from reader feedback, pre-filled with the feedback message and linked article.</li>
<li><strong>AI Suggestions</strong> — Click <strong>Accept</strong> on any AI suggestion to convert it into a real task.</li>
</ul>

<h3>Task Detail Panel</h3>
<p>Click any task to open the slide-over panel. Edit title, status, priority, type, assignee, due date, description, and linked article. The panel shows an article preview card and an activity timeline. Assignee changes require confirmation before sending an email notification.</p>

<h3>Bulk Select &amp; Delete</h3>
<p>Select multiple tasks using checkboxes, then click <strong>Delete</strong> in the action bar. A confirmation dialog appears before deletion.</p>

<h3>Email Notifications</h3>
<p>When a task is assigned to a team member (not yourself), they receive a branded email with the task title, priority, type, due date, and a link to open FinalDoc.</p>

<h3>Burndown Sparkline</h3>
<p>A small teal line chart next to the streak counter shows task completions over the last 7 days.</p>

<h3>Completion Streak</h3>
<p>A flame icon with the streak count appears when you complete tasks on consecutive days.</p>

<h3>Documentation-Specific Task Types</h3>
<ul>
<li><strong>Content Review</strong> — Review an article for accuracy</li>
<li><strong>Content Update</strong> — Update outdated content</li>
<li><strong>New Article</strong> — Write a new article</li>
<li><strong>Translation</strong> — Translate content to another language</li>
<li><strong>Screenshot Update</strong> — Replace stale screenshots</li>
<li><strong>Link Fix</strong> — Fix broken links</li>
<li><strong>SEO Optimization</strong> — Improve search ranking</li>
</ul>

<h3>AI Task Suggestions</h3>
<p>The AI tab surfaces suggestions based on your knowledge base data:</p>
<ul>
<li><strong>Stale articles</strong> — Published articles not updated in 90+ days</li>
<li><strong>Negative feedback</strong> — Articles with more dislikes than likes</li>
<li><strong>Content gaps</strong> — Reader searches that returned zero results</li>
</ul>

<h2>Comments</h2>
<p>The Comments card shows recent discussion activity across your articles. Filter by:</p>
<ul>
<li><strong>All</strong> — All comments on your articles</li>
<li><strong>@Me</strong> — Comments where you are mentioned</li>
<li><strong>Articles</strong> — Article-level comments only</li>
</ul>

<h2>Ved AI</h2>
<p>The Ved AI card provides quick access to your AI writing assistant. Click <strong>Learn More</strong> to explore AI features including smart search suggestions, content generation, and translation.</p>

<h2>Refreshing the Dashboard</h2>
<p>Dashboard data refreshes automatically every 60 seconds. You can also reload the page to fetch the latest data immediately.</p>

<div style="background:#eff6ff;border-left:4px solid #3b82f6;padding:12px 16px;border-radius:4px;margin:16px 0">
  <strong>Tip:</strong> Bookmark <code>https://app.finaldoc.io</code> to jump straight to your Dashboard each time you open FinalDoc.
</div>