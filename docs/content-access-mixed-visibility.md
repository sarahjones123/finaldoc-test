---
title: "Content Access & Mixed Visibility"
description: ""
slug: "content-access-mixed-visibility"
status: "PUBLISHED"
createdAt: "2026-02-24T08:32:54.671Z"
updatedAt: "2026-03-12T09:12:46.998Z"
---

<h1>Content Access and Mixed Visibility</h1>
<p>Mixed Visibility lets you have a single knowledge base where some content is publicly accessible and other content requires reader login. This is useful when you want to publish general documentation publicly while keeping premium, sensitive, or customer-specific content gated.</p>

<h2>Enabling Mixed Visibility</h2>
<ol>
<li>Go to <strong>Settings → Security &amp; Access → Site Visibility</strong></li>
<li>Select <strong>Mixed</strong></li>
<li>Click <strong>Save</strong></li>
</ol>

<h2>Configuring Which Content Is Private</h2>
<ol>
<li>Go to <strong>Settings → Security &amp; Access → Content Access &amp; Mixed Visibility</strong></li>
<li>You see a list of all your categories and articles</li>
<li>Toggle any category or article to <strong>Private</strong> to require login for that content</li>
<li>Marking a category as Private makes ALL articles in that category private</li>
<li>You can also mark individual articles as private within a public category</li>
</ol>

<h2>How It Works for Readers</h2>
<ul>
<li>Public articles: Anyone can access, no login required</li>
<li>Private articles: Clicking the article title redirects to the login page. After logging in, the reader is taken directly to the article they tried to access</li>
<li>In the KB sidebar, private articles may show a lock icon to indicate they require login (optional — configurable in Portal Builder)</li>
</ul>

<h2>Reader Groups and Mixed Visibility</h2>
<p>For more granular control, combine Mixed Visibility with <strong>Reader Groups</strong>. Instead of "logged in = all private content", you can restrict specific categories to specific groups:</p>
<ul>
<li>Category "Partner Resources" — only visible to readers in the "Partners" group</li>
<li>Category "Beta Features" — only visible to readers in the "Beta Testers" group</li>
</ul>
<p>Configure this in <strong>Settings → Security &amp; Access → Reader Groups &amp; Segmented Access</strong>.</p>

<h2>Public vs. Private vs. Mixed — When to Use Each</h2>
<table>
<thead><tr><th>Use Case</th><th>Recommended Setting</th></tr></thead>
<tbody>
<tr><td>Public product documentation for all visitors</td><td>Public</td></tr>
<tr><td>Internal company wiki</td><td>Private</td></tr>
<tr><td>Mix of public marketing docs + private enterprise features</td><td>Mixed</td></tr>
<tr><td>Customer support KB (general FAQ public, account guides private)</td><td>Mixed</td></tr>
</tbody>
</table>