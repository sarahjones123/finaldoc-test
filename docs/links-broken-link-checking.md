---
title: "Links & Broken Link Checking"
description: "How to use the links analytics dashboard to detect and fix broken links in your documentation."
slug: "links-broken-link-checking"
status: "PUBLISHED"
createdAt: "2026-02-24T05:03:38.917Z"
updatedAt: "2026-03-14T14:51:22.703Z"
---

<h1>Links &amp; Broken Link Checking</h1>
<p>FinalDoc's content health tools include a broken link checker that scans all your published articles for hyperlinks that no longer work — returning 404, 500, or other error responses. Dead links frustrate readers and damage your KB's credibility. The broken link checker helps you find and fix them systematically.</p>

<h2>How Links Work in FinalDoc</h2>
<p>Two types of links appear in articles:</p>
<ul>
<li><strong>Internal links</strong> — Links to other articles within your FinalDoc KB (created using Smart Linking or manual hyperlinks). These are relative links (<code>/article/slug</code>)</li>
<li><strong>External links</strong> — Links to external websites (docs.your-tool.com, GitHub, etc.). Full URLs starting with https://</li>
</ul>

<h2>Running the Broken Link Check</h2>
<ol>
<li>Click <strong>Analytics</strong> in the left sidebar</li>
<li>Click <strong>Content Health Dashboard</strong></li>
<li>Find the <strong>Broken Links</strong> check</li>
<li>Click <strong>Run Link Check</strong></li>
</ol>
<p>FinalDoc scans every hyperlink in every published article. This can take a few minutes for large knowledge bases. You can navigate away — the check runs in the background.</p>

<h2>Viewing Broken Links</h2>
<p>When the scan completes:</p>
<ol>
<li>Click <strong>Broken Links</strong> in the Content Health Dashboard</li>
<li>A table shows all broken links found: article name, broken URL, error type (404, 500, timeout, SSL error)</li>
</ol>

<h2>Fixing Broken Links</h2>
<p>For each broken link:</p>
<ol>
<li>Click the article name in the broken links list — the article opens in the editor</li>
<li>Find the broken link (use Ctrl+F to search for the broken URL)</li>
<li>Right-click the link → <strong>Edit Link</strong></li>
<li>Update the URL to the new/correct URL, or remove the link if the page no longer exists</li>
<li>Save the article</li>
</ol>

<h2>Smart Link Checking (Internal Links)</h2>
<p>When you delete an article in FinalDoc, the system automatically checks if any other articles have links pointing to the deleted article. A warning appears: "This article is linked from X other articles. Deleting it will create broken links in those articles." You can choose to update those links before deleting, or proceed anyway.</p>

<h2>Scheduled Link Checks</h2>
<p>Enable automatic weekly link checks from <strong>Settings → Notifications</strong> → <strong>Broken Link Check</strong>. When broken links are found, you receive an email or Slack notification listing the articles with broken links.</p>