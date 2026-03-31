---
title: "Comments API Reference"
description: ""
slug: "comments-api-reference"
status: "PUBLISHED"
createdAt: "2026-02-24T08:32:54.565Z"
updatedAt: "2026-03-27T10:29:46.727Z"
---

<h1>Comments API Reference</h1>
<p>The Comments API lets you retrieve and manage article comments programmatically — both threaded discussion comments and inline text-selection comments.</p>

<h2>List Comments for an Article</h2>
<pre><code>GET /articles/{articleId}/comments</code></pre>

<p><strong>Query parameters:</strong></p>
<ul>
<li><code>type</code> — <code>discussion</code> (article-level threaded comments) or <code>inline</code> (text-selection comments)</li>
<li><code>resolved</code> — <code>true</code> or <code>false</code> to filter by resolution status</li>
</ul>

<p><strong>Example response:</strong></p>
<pre><code>{
  "comments": [
    {
      "id": "comment_abc",
      "type": "discussion",
      "authorName": "Alice Johnson",
      "authorId": "user_abc",
      "content": "Should we add a note about IE11 support here?",
      "createdAt": "2026-03-08T10:15:00Z",
      "resolved": false,
      "replies": [
        {
          "id": "comment_def",
          "authorName": "Bob Smith",
          "content": "Good point, adding a note now.",
          "createdAt": "2026-03-08T10:22:00Z"
        }
      ]
    }
  ]
}</code></pre>

<h2>Get Comment</h2>
<pre><code>GET /comments/{commentId}</code></pre>

<h2>Create Comment</h2>
<pre><code>POST /articles/{articleId}/comments</code></pre>

<p><strong>Request body:</strong></p>
<pre><code>{
  "content": "This section needs updating for v2",
  "type": "discussion",
  "parentId": null
}</code></pre>
<p>To reply to an existing comment, set <code>parentId</code> to the parent comment's ID. To create an inline comment, set <code>type: "inline"</code> and include <code>selectedText</code> and <code>position</code> fields.</p>

<h2>Update Comment</h2>
<pre><code>PUT /comments/{commentId}</code></pre>

<p><strong>Request body:</strong></p>
<pre><code>{ "content": "Updated comment text" }</code></pre>
<p>Only the comment author or an ADMIN can update a comment.</p>

<h2>Resolve Comment</h2>
<pre><code>POST /comments/{commentId}/resolve</code></pre>
<p>Marks the comment as resolved. Returns the updated comment object.</p>

<h2>Delete Comment</h2>
<pre><code>DELETE /comments/{commentId}</code></pre>
<p>Permanently deletes the comment and all its replies. Returns 204 No Content.</p>

<h2>Authentication</h2>
<p>Comments API requires a session token (<code>fd_</code>). Comment creation requires at least AUTHOR role.</p>