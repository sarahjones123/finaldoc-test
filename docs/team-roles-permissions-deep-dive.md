---
title: "Team Roles & Permissions Deep Dive"
description: ""
slug: "team-roles-permissions-deep-dive"
status: "PUBLISHED"
createdAt: "2026-02-24T08:37:07.788Z"
updatedAt: "2026-03-19T09:29:33.584Z"
---

<h1>Team Roles &amp; Permissions Deep Dive</h1>
<p>FinalDoc has a 5-level role hierarchy for team members. Each role has a specific set of permissions. This article explains exactly what each role can and cannot do — useful when deciding which role to assign to new team members.</p>

<h2>The Five Roles</h2>
<table>
<thead><tr><th>Role</th><th>Best For</th></tr></thead>
<tbody>
<tr><td><strong>OWNER</strong></td><td>The account creator and primary decision-maker. Full control over everything including billing</td></tr>
<tr><td><strong>ADMIN</strong></td><td>Senior team members who need to configure settings, manage the team, and have full editorial control</td></tr>
<tr><td><strong>EDITOR</strong></td><td>Documentation writers who create, edit, and publish articles without needing admin access</td></tr>
<tr><td><strong>AUTHOR</strong></td><td>Occasional contributors who create drafts but need editorial review before publishing</td></tr>
<tr><td><strong>VIEWER</strong></td><td>Stakeholders who need to see admin-side drafts and analytics but should not edit anything</td></tr>
</tbody>
</table>

<h2>Permissions Matrix</h2>
<table>
<thead><tr><th>Permission</th><th>VIEWER</th><th>AUTHOR</th><th>EDITOR</th><th>ADMIN</th><th>OWNER</th></tr></thead>
<tbody>
<tr><td>View published articles (admin)</td><td>Yes</td><td>Yes</td><td>Yes</td><td>Yes</td><td>Yes</td></tr>
<tr><td>View draft articles</td><td>Yes</td><td>Yes</td><td>Yes</td><td>Yes</td><td>Yes</td></tr>
<tr><td>Create articles</td><td>No</td><td>Yes</td><td>Yes</td><td>Yes</td><td>Yes</td></tr>
<tr><td>Edit own articles</td><td>No</td><td>Yes</td><td>Yes</td><td>Yes</td><td>Yes</td></tr>
<tr><td>Edit any article</td><td>No</td><td>No</td><td>Yes</td><td>Yes</td><td>Yes</td></tr>
<tr><td>Publish articles</td><td>No</td><td>No</td><td>Yes</td><td>Yes</td><td>Yes</td></tr>
<tr><td>Delete articles</td><td>No</td><td>No</td><td>Yes</td><td>Yes</td><td>Yes</td></tr>
<tr><td>Manage categories</td><td>No</td><td>No</td><td>Yes</td><td>Yes</td><td>Yes</td></tr>
<tr><td>View analytics</td><td>Yes</td><td>Yes</td><td>Yes</td><td>Yes</td><td>Yes</td></tr>
<tr><td>Manage readers</td><td>No</td><td>No</td><td>No</td><td>Yes</td><td>Yes</td></tr>
<tr><td>Configure settings</td><td>No</td><td>No</td><td>No</td><td>Yes</td><td>Yes</td></tr>
<tr><td>Invite team members</td><td>No</td><td>No</td><td>No</td><td>Yes</td><td>Yes</td></tr>
<tr><td>Remove team members</td><td>No</td><td>No</td><td>No</td><td>Yes</td><td>Yes</td></tr>
<tr><td>View audit logs</td><td>No</td><td>No</td><td>No</td><td>Yes</td><td>Yes</td></tr>
<tr><td>Manage billing</td><td>No</td><td>No</td><td>No</td><td>No</td><td>Yes</td></tr>
<tr><td>Delete the project</td><td>No</td><td>No</td><td>No</td><td>No</td><td>Yes</td></tr>
<tr><td>Transfer project ownership</td><td>No</td><td>No</td><td>No</td><td>No</td><td>Yes</td></tr>
</tbody>
</table>

<h2>Assigning Roles</h2>
<ol>
<li>Go to <strong>Settings → Security &amp; Access → Team Management</strong></li>
<li>Click the role badge next to any team member's name</li>
<li>Select the new role from the dropdown</li>
<li>Changes take effect immediately</li>
</ol>
<p>Note: Only the OWNER can assign or change ADMIN roles. EDITORs cannot be promoted above EDITOR by an ADMIN.</p>

<h2>Custom Roles</h2>
<p>Custom roles (with fully customizable permission sets) are available on <strong>Enterprise plans</strong>. Contact support to set up custom roles tailored to your organization's specific access requirements.</p>