---
title: "Audit Logs"
description: "Viewing team activity history and change tracking."
slug: "audit-logs"
status: "PUBLISHED"
createdAt: "2026-02-23T18:16:36.545Z"
updatedAt: "2026-03-12T13:27:35.028Z"
---

<h1>Audit Logs</h1>
<p>The Audit Log records every significant action taken in your FinalDoc project — who did what and when. Use it for security monitoring, compliance requirements, team accountability, and understanding the history of changes to your knowledge base.</p>

<h2>Opening Audit Logs</h2>
<ol>
<li>Go to <strong>Settings</strong> in the left sidebar</li>
<li>Click <strong>Data &amp; Compliance → Audit Logs</strong></li>
</ol>

<h2>What Gets Logged</h2>
<p>Every entry in the audit log shows the action, the user who performed it, the affected resource, and a timestamp. Actions that are recorded include:</p>

<h3>Article Actions</h3>
<ul>
<li>Article created</li>
<li>Article published / unpublished</li>
<li>Article updated (content saved)</li>
<li>Article deleted / moved to recycle bin</li>
<li>Article restored from recycle bin</li>
<li>Article moved to different category</li>
<li>Article scheduled for publication</li>
</ul>

<h3>Category Actions</h3>
<ul>
<li>Category created</li>
<li>Category renamed</li>
<li>Category deleted</li>
<li>Category reordered</li>
</ul>

<h3>Team Actions</h3>
<ul>
<li>Team member invited</li>
<li>Team member role changed</li>
<li>Team member removed</li>
</ul>

<h3>Reader Actions</h3>
<ul>
<li>Reader account created</li>
<li>Reader login (successful and failed)</li>
<li>Reader group membership changes</li>
</ul>

<h3>Settings Actions</h3>
<ul>
<li>Project settings updated</li>
<li>Domain configuration changes</li>
<li>API token created or deleted</li>
<li>Security settings changed (IP restrictions, visibility)</li>
<li>Extension connected or disconnected</li>
</ul>

<h3>Content Actions</h3>
<ul>
<li>Files uploaded to Drive</li>
<li>Files deleted from Drive</li>
<li>Import job started or completed</li>
<li>Backup created or restored</li>
</ul>

<h2>Reading the Audit Log</h2>
<p>Each log entry shows:</p>
<ul>
<li><strong>Timestamp</strong> — Exact date and time of the action</li>
<li><strong>User</strong> — The team member who performed the action (name + email)</li>
<li><strong>Action</strong> — What happened (e.g., "Article Published", "Team Member Invited")</li>
<li><strong>Resource</strong> — What was affected (article title, email address, file name, etc.)</li>
<li><strong>IP Address</strong> — The IP address from which the action was performed (useful for security audits)</li>
</ul>

<h2>Filtering and Searching</h2>
<ul>
<li><strong>Date range</strong> — Filter to a specific time period (today, last 7 days, last 30 days, or custom)</li>
<li><strong>Action type</strong> — Filter to only see certain types of events (e.g., only article publishes)</li>
<li><strong>User</strong> — Filter to see only actions from a specific team member</li>
<li><strong>Search</strong> — Search within the log by keyword</li>
</ul>

<h2>Exporting Audit Logs</h2>
<p>Click <strong>Export CSV</strong> to download the audit log data as a CSV file. This is useful for compliance reporting, security incident reviews, or archiving logs in your own systems.</p>

<h2>Log Retention</h2>
<p>Audit logs are retained for 90 days on paid plans and 30 days on the free plan. Older entries are automatically purged. If you need longer retention for compliance purposes, export logs regularly before they are purged.</p>

<h2>Use Cases</h2>
<ul>
<li><strong>Security incident investigation</strong>: See exactly who accessed or changed what, and from which IP</li>
<li><strong>Compliance</strong>: Many compliance frameworks (SOC 2, ISO 27001, GDPR) require audit trails of who accessed data</li>
<li><strong>Team accountability</strong>: Know who published an article, who deleted content, or who made a settings change</li>
<li><strong>Debugging</strong>: Trace the history of changes to an article if something looks wrong</li>
</ul>