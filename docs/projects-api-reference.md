---
title: "Projects API Reference"
description: ""
slug: "projects-api-reference"
status: "PUBLISHED"
createdAt: "2026-02-24T08:32:54.551Z"
updatedAt: "2026-03-27T10:29:46.727Z"
---

<h1>Projects API Reference</h1>
<p>The Projects API lets you retrieve information about your FinalDoc projects and workspaces programmatically.</p>

<h2>List Projects</h2>
<pre><code>GET /projects</code></pre>
<p>Returns all projects accessible to the authenticated user/token.</p>

<p><strong>Example response:</strong></p>
<pre><code>{
  "projects": [
    {
      "id": "proj_abc123",
      "name": "Acme Corp Help Center",
      "slug": "acme-corp-help",
      "plan": "business",
      "createdAt": "2026-01-01T00:00:00Z",
      "workspaces": [
        {
          "id": "ws_def456",
          "name": "Main Documentation",
          "articleCount": 84
        }
      ]
    }
  ]
}</code></pre>

<h2>Get Project</h2>
<pre><code>GET /projects/{projectId}</code></pre>
<p>Returns a single project's full details including workspaces, settings summary, and usage stats.</p>

<h2>Get Project Settings</h2>
<pre><code>GET /projects/{projectId}/settings</code></pre>
<p>Returns the project's public settings (KB name, description, plan info, custom domain if configured). Does not include sensitive settings like API keys.</p>

<h2>Update Project Settings</h2>
<pre><code>PUT /projects/{projectId}/settings</code></pre>
<p>Update project settings. Accepts a partial settings object — only specified fields are updated.</p>

<p><strong>Request body (partial example):</strong></p>
<pre><code>{
  "name": "New Help Center Name",
  "description": "Updated description",
  "settings": {
    "docShowTableOfContents": true,
    "docShowReadingTime": true
  }
}</code></pre>

<div style="border-left: 4px solid #ef4444; border-radius: 8px; padding: 16px; margin: 16px 0; background: rgba(239,68,68,0.08);">
<strong>Warning:</strong> The settings field in the database is a JSON object. The PUT endpoint does a merge of the settings you provide with existing settings. However, if you accidentally send the wrong structure, it can break features. Always read current settings before updating them.
</div>

<h2>List Workspaces</h2>
<pre><code>GET /projects/{projectId}/workspaces</code></pre>
<p>Returns all workspaces within a project. A workspace is a distinct knowledge base (most projects have one, enterprise projects may have multiple for different product lines or audiences).</p>

<h2>Get Workspace</h2>
<pre><code>GET /workspaces/{workspaceId}</code></pre>
<p>Returns a single workspace with article count, category count, and configuration details.</p>

<h2>Authentication</h2>
<p>All Projects API endpoints require a session token (<code>fd_</code>) with admin access to the project. API tokens (<code>api_</code>) do not have access to project-level settings.</p>