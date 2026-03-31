---
title: "Readers API Reference"
description: "Reference for the Readers API — invite, manage, and remove readers programmatically."
slug: "readers-api-reference"
status: "PUBLISHED"
createdAt: "2026-02-24T05:06:07.521Z"
updatedAt: "2026-03-27T10:29:46.727Z"
---

<h1>Readers API Reference</h1>
<p>The Readers API lets you programmatically manage reader accounts — list readers, invite new ones, update their details, and remove them.</p>

<h2>List Readers</h2>
<pre><code>GET /projects/{projectId}/readers</code></pre>
<p>Returns all readers for this project.</p>

<p><strong>Query parameters:</strong></p>
<ul>
<li><code>groupId</code> — Filter by reader group</li>
<li><code>email</code> — Search by email address (partial match)</li>
<li><code>limit</code> — Max results (default 50)</li>
<li><code>offset</code> — Pagination offset</li>
</ul>

<p><strong>Example response:</strong></p>
<pre><code>{
  "readers": [
    {
      "id": "reader_abc",
      "email": "jane@example.com",
      "name": "Jane Smith",
      "groups": ["group_enterprise"],
      "createdAt": "2026-02-01T09:00:00Z",
      "lastActiveAt": "2026-03-10T16:45:00Z"
    }
  ],
  "total": 142
}</code></pre>

<h2>Get Reader</h2>
<pre><code>GET /projects/{projectId}/readers/{readerId}</code></pre>
<p>Returns a single reader's details including group memberships and activity summary.</p>

<h2>Invite Reader</h2>
<pre><code>POST /projects/{projectId}/readers/invite</code></pre>

<p><strong>Request body:</strong></p>
<pre><code>{
  "email": "newreader@example.com",
  "name": "New Reader",
  "groupIds": ["group_abc"],
  "sendInviteEmail": true
}</code></pre>
<p>Creates the reader account and optionally sends an invitation email with a login link. If <code>sendInviteEmail</code> is false, the reader is created but receives no email — useful for bulk imports where you'll handle communication separately.</p>

<h2>Bulk Invite Readers</h2>
<pre><code>POST /projects/{projectId}/readers/bulk-invite</code></pre>

<p><strong>Request body:</strong></p>
<pre><code>{
  "readers": [
    { "email": "user1@example.com", "name": "User One" },
    { "email": "user2@example.com", "name": "User Two" }
  ],
  "groupIds": ["group_enterprise"],
  "sendInviteEmail": false
}</code></pre>
<p>Maximum 100 readers per bulk invite request. Returns a summary of how many succeeded and which emails failed (e.g., duplicate emails).</p>

<h2>Update Reader</h2>
<pre><code>PUT /projects/{projectId}/readers/{readerId}</code></pre>
<p>Update reader name, group memberships, or other metadata.</p>

<h2>Remove Reader</h2>
<pre><code>DELETE /projects/{projectId}/readers/{readerId}</code></pre>
<p>Removes the reader from the project. They lose access immediately. Returns 204 No Content.</p>

<h2>Reader Groups</h2>
<pre><code>GET /projects/{projectId}/reader-groups
POST /projects/{projectId}/reader-groups
DELETE /projects/{projectId}/reader-groups/{groupId}</code></pre>
<p>Manage reader groups (for segmented content access). See the Reader Groups article for details on how groups control content visibility.</p>