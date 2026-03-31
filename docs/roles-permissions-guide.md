---
title: "Roles & Permissions Guide"
description: "Understand the role hierarchy and configure access permissions for your team."
slug: "roles-permissions-guide"
status: "PUBLISHED"
createdAt: "2026-02-24T03:51:22.535Z"
updatedAt: "2026-03-19T09:28:32.185Z"
---

<h1>Roles and Permissions Guide</h1>
<p>This guide explains what each team role can and cannot do in FinalDoc, so you can assign the right role to each team member.</p>

<h2>Role Overview</h2>
<table>
<thead><tr><th>Permission</th><th>Owner</th><th>Admin</th><th>Editor</th><th>Draft Writer</th><th>Viewer</th></tr></thead>
<tbody>
<tr><td>Read published articles (admin)</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td></tr>
<tr><td>Read draft articles (admin)</td><td>✅</td><td>✅</td><td>✅</td><td>Own only</td><td>✅</td></tr>
<tr><td>Create articles</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>❌</td></tr>
<tr><td>Edit any article</td><td>✅</td><td>✅</td><td>✅</td><td>Own only</td><td>❌</td></tr>
<tr><td>Publish articles</td><td>✅</td><td>✅</td><td>✅</td><td>❌</td><td>❌</td></tr>
<tr><td>Delete any article</td><td>✅</td><td>✅</td><td>✅</td><td>Own only</td><td>❌</td></tr>
<tr><td>Manage categories</td><td>✅</td><td>✅</td><td>✅</td><td>❌</td><td>❌</td></tr>
<tr><td>Access Analytics</td><td>✅</td><td>✅</td><td>✅</td><td>❌</td><td>❌</td></tr>
<tr><td>Access Feedback</td><td>✅</td><td>✅</td><td>✅</td><td>❌</td><td>❌</td></tr>
<tr><td>Access Toolbox</td><td>✅</td><td>✅</td><td>✅</td><td>❌</td><td>❌</td></tr>
<tr><td>Manage Drive</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>❌</td></tr>
<tr><td>Access Settings</td><td>✅</td><td>✅</td><td>❌</td><td>❌</td><td>❌</td></tr>
<tr><td>Manage Team Members</td><td>✅</td><td>✅</td><td>❌</td><td>❌</td><td>❌</td></tr>
<tr><td>Manage Readers</td><td>✅</td><td>✅</td><td>❌</td><td>❌</td><td>❌</td></tr>
<tr><td>Manage Billing</td><td>✅</td><td>❌</td><td>❌</td><td>❌</td><td>❌</td></tr>
<tr><td>Delete Account</td><td>✅</td><td>❌</td><td>❌</td><td>❌</td><td>❌</td></tr>
<tr><td>Invite new team members</td><td>✅</td><td>✅</td><td>❌</td><td>❌</td><td>❌</td></tr>
</tbody>
</table>

<h2>Choosing the Right Role</h2>
<ul>
<li><strong>Owner</strong> — The account creator. Assign to the person who owns the account and manages the subscription</li>
<li><strong>Admin</strong> — For your documentation leads, content managers, and senior team members who need full access to settings</li>
<li><strong>Editor</strong> — For your primary writers who create and publish content regularly. This is the most common role</li>
<li><strong>Draft Writer</strong> — For contributors who write drafts but should not publish directly. Use with the Approval Flow for review before publishing</li>
<li><strong>Viewer</strong> — For stakeholders, executives, or support team members who need to read docs (including drafts) but should not make changes</li>
</ul>

<h2>Draft Writers and the Approval Flow</h2>
<p>Draft Writers submit articles for review instead of publishing directly. To set this up:</p>
<ol>
<li>Assign team members the Draft Writer role</li>
<li>Set up an Approval Flow in <strong>Toolbox → Approval Flow</strong></li>
<li>Draft Writers see a "Submit for Review" button instead of "Publish"</li>
<li>Editors and Admins review and approve before the article goes live</li>
</ol>

<h2>Audit Trail</h2>
<p>All significant actions (article publish, article delete, settings changes, team member invite/remove) are logged in the Audit Log. Access it in <strong>Settings → Data &amp; Compliance → Audit Logs</strong>. The log shows who did what and when.</p>