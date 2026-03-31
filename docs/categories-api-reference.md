---
title: "Categories API Reference"
description: "Complete reference for the Categories API — manage your documentation structure."
slug: "categories-api-reference"
status: "PUBLISHED"
createdAt: "2026-02-24T05:06:04.312Z"
updatedAt: "2026-03-27T10:29:46.727Z"
---

<h1>Categories API Reference</h1>
<p>The Categories API lets you list, create, and manage categories (folders) in your FinalDoc workspace.</p>

<h2>List Categories</h2>
<pre><code>GET /workspaces/{workspaceId}/categories</code></pre>
<p>Returns all categories in the workspace, including nested sub-categories.</p>

<p><strong>Example response:</strong></p>
<pre><code>{
  "categories": [
    {
      "id": "cat123",
      "name": "Getting Started",
      "slug": "getting-started",
      "parentId": null,
      "order": 0,
      "articleCount": 5,
      "color": "green",
      "icon": "rocket"
    },
    {
      "id": "cat456",
      "name": "Installation",
      "slug": "installation",
      "parentId": "cat123",
      "order": 0,
      "articleCount": 3
    }
  ]
}</code></pre>

<h2>Get Category</h2>
<pre><code>GET /categories/{categoryId}</code></pre>
<p>Returns a single category with its articles list.</p>

<h2>Create Category</h2>
<pre><code>POST /workspaces/{workspaceId}/categories</code></pre>

<p><strong>Request body:</strong></p>
<pre><code>{
  "name": "Advanced Topics",
  "parentId": null,
  "description": "In-depth guides for power users",
  "color": "purple",
  "icon": "lightning"
}</code></pre>

<p><strong>Required fields:</strong> <code>name</code></p>
<p>Set <code>parentId</code> to the ID of an existing category to create a sub-category. Leave null for a top-level category.</p>

<h2>Update Category</h2>
<pre><code>PUT /categories/{categoryId}</code></pre>
<p>Update category name, description, parent, color, or icon. Only include fields to change.</p>

<h2>Delete Category</h2>
<pre><code>DELETE /categories/{categoryId}</code></pre>
<p>Deletes the category. Articles in the category are <strong>not</strong> deleted — they become uncategorized. Sub-categories are also deleted. Returns 204 No Content.</p>

<h2>Reorder Categories</h2>
<pre><code>POST /workspaces/{workspaceId}/categories/reorder</code></pre>

<p><strong>Request body:</strong></p>
<pre><code>{
  "order": ["cat123", "cat456", "cat789"]
}</code></pre>
<p>Sets the display order of categories. Provide a complete ordered array of category IDs at the same level.</p>

<h2>Required Scopes</h2>
<p>Category API operations require a session token (fd_) or an API token with at minimum <code>read:articles</code> for read operations. Create/update/delete require <code>write:articles</code>.</p>