---
title: "Redirects"
description: "Setting up URL redirect rules for moved or renamed content."
slug: "redirects"
status: "PUBLISHED"
createdAt: "2026-02-23T18:16:24.339Z"
updatedAt: "2026-03-12T09:12:47.045Z"
---

<h1>URL Redirects</h1>
<p>Redirects let you route old or changed URLs to new ones. When you rename an article (changing its slug/URL), readers with bookmarks or external links to the old URL get a broken page. Set up a redirect from the old URL to the new one so those links keep working.</p>

<h2>Opening Redirects</h2>
<ol>
<li>Go to <strong>Settings → Domain &amp; SEO → Redirects</strong></li>
</ol>

<h2>Creating a Redirect</h2>
<ol>
<li>Click <strong>+ Add Redirect</strong></li>
<li>Enter the <strong>source URL</strong> — the old URL path you want to redirect FROM (e.g., <code>/kb/old-article-slug</code>)</li>
<li>Enter the <strong>destination URL</strong> — where the redirect goes TO (e.g., <code>/kb/new-article-slug</code>)</li>
<li>Choose the <strong>redirect type</strong>:
  <ul>
    <li><strong>301 (Permanent)</strong> — Tells search engines to update their index to the new URL. Use this when the content has permanently moved. This is the most common choice</li>
    <li><strong>302 (Temporary)</strong> — Tells search engines the old URL is still the "real" one, just temporarily redirecting. Use this for temporary redirects</li>
  </ul>
</li>
<li>Click <strong>Save</strong></li>
</ol>

<h2>When to Use Redirects</h2>
<ul>
<li>You renamed an article and its slug changed</li>
<li>You merged two articles into one</li>
<li>You reorganized your KB structure and moved articles to new URL paths</li>
<li>You migrated from another documentation platform and need to preserve old URLs</li>
</ul>

<h2>Bulk Redirects</h2>
<p>For large migrations with many URL changes, you can import redirects in bulk:</p>
<ol>
<li>Prepare a CSV file with columns: <code>source,destination,type</code></li>
<li>Click <strong>Import CSV</strong> in the Redirects page</li>
<li>Upload the file — all redirects are created at once</li>
</ol>

<h2>Testing Redirects</h2>
<p>After creating a redirect, test it:</p>
<ol>
<li>Open a private/incognito browser window</li>
<li>Navigate to the old URL</li>
<li>Verify you are redirected to the new URL correctly</li>
</ol>
<p>Note: Redirects may be cached by browsers. If testing does not work immediately, try clearing browser cache or using a different browser.</p>