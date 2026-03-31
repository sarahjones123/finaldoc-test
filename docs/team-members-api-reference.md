---
title: "Team Members API Reference"
description: ""
slug: "team-members-api-reference"
status: "PUBLISHED"
createdAt: "2026-02-24T08:32:54.595Z"
updatedAt: "2026-03-27T10:29:46.727Z"
---

<h1>Team Members API Reference</h1>
<p>The Team Members API lets you programmatically manage your team — invite new members, update roles, and remove members.</p>

<h2>List Team Members</h2>
<pre><code>GET /projects/{projectId}/team</code></pre>
<p>Returns all team members with their roles and last activity.</p>

<p><strong>Example response:</strong></p>
<pre><code>{
  "members": [
    {
      "id": "user_abc",
      "email": "alice@company.com",
      "name": "Alice Johnson",
      "role": "EDITOR",
      "joinedAt": "2026-01-15T09:00:00Z",
      "lastActiveAt": "2026-03-11T16:30:00Z"
    }
  ]
}</code></pre>

<h2>Invite Team Member</h2>
<pre><code>POST /projects/{projectId}/team/invite</code></pre>

<p><strong>Request body:</strong></p>
<pre><code>{
  "email": "newmember@company.com",
  "name": "New Member",
  "role": "EDITOR"
}</code></pre>

<p><strong>Available roles:</strong></p>
<ul>
<li><code>VIEWER</code> — Read-only access to admin panel; cannot edit</li>
<li><code>AUTHOR</code> — Can create/edit own articles; cannot publish</li>
<li><code>EDITOR</code> — Can create, edit, and publish any article</li>
<li><code>ADMIN</code> — Full access except billing and account deletion</li>
<li><code>OWNER</code> — Full access including billing (only via UI; cannot assign via API)</li>
</ul>
<p>FinalDoc sends an invitation email to the new member. If they don't have an account, they're prompted to create one.</p>

<h2>Update Team Member Role</h2>
<pre><code>PUT /projects/{projectId}/team/{userId}/role</code></pre>

<p><strong>Request body:</strong></p>
<pre><code>{ "role": "ADMIN" }</code></pre>
<p>Only the project OWNER can promote members to ADMIN or demote ADMINs. EDITORs cannot be promoted above ADMIN via API.</p>

<h2>Remove Team Member</h2>
<pre><code>DELETE /projects/{projectId}/team/{userId}</code></pre>
<p>Removes the team member from the project. They lose access immediately. Returns 204 No Content. The OWNER cannot be removed via API.</p>

<h2>Authentication</h2>
<p>Team API endpoints require a session token (<code>fd_</code>) with ADMIN or OWNER role on the project.</p>