---
title: "Knowledge Bases (Versions)"
description: "Managing KB versions, workspaces, and languages."
slug: "knowledge-bases-versions"
status: "PUBLISHED"
createdAt: "2026-02-23T18:13:43.783Z"
updatedAt: "2026-03-21T02:32:31.283Z"
---

<h1>Knowledge Bases (Workspaces)</h1>
<p>FinalDoc supports running multiple separate knowledge base workspaces within one project. This lets you maintain completely different sets of content under the same project — for example, documentation for v1 and v2 of your product, separate documentation for different product lines, or one KB for customers and one for internal teams.</p>

<h2>What Is a Workspace?</h2>
<p>Within your FinalDoc project, a <strong>workspace</strong> is a distinct knowledge base. Each workspace has its own:</p>
<ul>
<li>Articles and categories (completely separate from other workspaces)</li>
<li>URL segment (e.g., <code>/v1</code> or <code>/v2</code> on your KB domain)</li>
<li>Visibility settings (a workspace can be public while another is private)</li>
<li>Category structure and article tree</li>
</ul>
<p>All workspaces share the same project settings: design, branding, team members, readers, and billing plan.</p>

<h2>Managing Workspaces</h2>
<ol>
<li>Go to <strong>Settings → General → Knowledge Bases</strong></li>
</ol>
<p>You'll see a list of all workspaces in your project. Click any workspace to see its settings or switch to writing in it.</p>

<h2>Creating a New Workspace</h2>
<ol>
<li>In the Knowledge Bases settings, click <strong>+ Add Workspace</strong></li>
<li>Enter a <strong>Name</strong> for the workspace (e.g., "v2.0 Documentation", "Internal Wiki", "API Reference")</li>
<li>Enter a <strong>Slug</strong> — this becomes the URL path segment (e.g., slug <code>v2</code> → accessible at <code>yourproject.finaldoc.io/v2</code>)</li>
<li>Choose <strong>Visibility</strong> (Public or Private)</li>
<li>Click <strong>Create</strong></li>
</ol>

<h2>Switching Between Workspaces</h2>
<p>When you have multiple workspaces, a workspace selector appears in the Documentation sidebar (usually a dropdown near the top). Click it to switch which workspace you're writing in. All article and category lists update to show the selected workspace's content.</p>

<h2>Workspace URLs</h2>
<p>Each workspace is accessible at a different URL path:</p>
<ul>
<li><strong>Default workspace</strong>: <code>yourproject.finaldoc.io/</code> (root)</li>
<li><strong>Additional workspaces</strong>: <code>yourproject.finaldoc.io/{slug}</code></li>
</ul>
<p>For example, if you create a workspace with slug <code>v2</code>, it's at <code>yourproject.finaldoc.io/v2</code>. The homepage for that workspace shows its own articles and categories.</p>

<h2>Workspace Visibility</h2>
<p>Each workspace has independent visibility settings:</p>
<ul>
<li><strong>Public</strong>: Anyone can browse this workspace without logging in</li>
<li><strong>Private</strong>: Readers must log in to access this workspace</li>
</ul>
<p>For example, you might make your main customer docs public but keep an internal wiki workspace private (employees only).</p>

<h2>Workspace Navigation on the Public KB</h2>
<p>Readers can navigate between workspaces via direct URLs. You can also add links between workspaces in the KB header navigation (Settings → Appearance → Portal Builder → Header) to help readers switch between doc sets.</p>

<h2>Deleting a Workspace</h2>
<p>To delete a workspace, open its settings in <strong>Settings → General → Knowledge Bases</strong> and click <strong>Delete Workspace</strong>. This permanently deletes all articles and categories in that workspace. This action cannot be undone — make sure to export the content first if needed.</p>

<h2>Common Use Cases</h2>
<ul>
<li><strong>API versioning</strong>: Workspace "v1" for v1 API docs, workspace "v2" for v2 API docs</li>
<li><strong>Internal + external docs</strong>: Public workspace for customers, private workspace for internal team SOPs</li>
<li><strong>Multi-product</strong>: Separate workspace per product when your documentation sets are large and distinct</li>
<li><strong>Beta documentation</strong>: Private workspace for beta feature docs, separate from the public-facing KB</li>
</ul>