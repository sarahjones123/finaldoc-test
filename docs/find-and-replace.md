---
title: "Find and Replace"
description: "How to search and replace text across all your documentation."
slug: "find-and-replace"
status: "PUBLISHED"
createdAt: "2026-02-23T18:13:43.110Z"
updatedAt: "2026-03-21T03:30:55.831Z"
---

<h1>Find and Replace</h1>
<p>Find and Replace lets you search for any word, phrase, or text across all articles in your knowledge base and replace it — in bulk, across hundreds of articles at once. This is essential for renaming products, fixing recurring errors, updating URLs, or changing terminology across your entire documentation.</p>

<h2>Opening Find and Replace</h2>
<ol>
<li>Click <strong>Toolbox</strong> in the left sidebar</li>
<li>Under the <strong>Content</strong> section, click <strong>Find &amp; Replace</strong></li>
</ol>

<h2>How to Use It</h2>
<ol>
<li>In the <strong>Find</strong> field, type the word or phrase you are looking for</li>
<li>In the <strong>Replace with</strong> field, type what you want to replace it with (leave blank to just delete the found text)</li>
<li>Configure options:
  <ul>
    <li><strong>Case sensitive</strong> — Check this if you want to match exact capitalization (e.g., only match "API" not "api")</li>
    <li><strong>Whole word only</strong> — Only match complete words (e.g., "run" will not match "running")</li>
    <li><strong>Search in titles</strong> — Also search article titles, not just body content</li>
    <li><strong>Search in descriptions</strong> — Also search the article description/summary field</li>
  </ul>
</li>
<li>Click <strong>Search</strong> to find all matches across all articles</li>
<li>Review the results — each match shows the article title and the context around the match</li>
<li>Select which articles to apply the replacement to (all by default, or uncheck specific articles to skip them)</li>
<li>Click <strong>Replace All</strong> to apply the replacement</li>
</ol>

<h2>Results View</h2>
<p>After searching, you see a list of matching articles with:</p>
<ul>
<li>Article title (click to open the article in a new tab)</li>
<li>Category it belongs to</li>
<li>Number of matches in that article</li>
<li>A preview of the text with the matched phrase highlighted</li>
</ul>

<h2>Safety Features</h2>
<ul>
<li>You can preview changes before applying them</li>
<li>Replacements only happen on the articles you confirm</li>
<li>Version history captures the state before and after the replacement — you can restore any article if the replacement was a mistake</li>
</ul>

<h2>Common Use Cases</h2>
<ul>
<li>Renaming a product feature ("Widget" → "Component")</li>
<li>Updating a URL that changed (old domain → new domain)</li>
<li>Fixing a spelling error that appeared consistently ("recieve" → "receive")</li>
<li>Updating version numbers in code examples ("v1.0" → "v2.0")</li>
<li>Replacing placeholder text left from templates ("[Company Name]" → "Acme Corp")</li>
</ul>

<div style="border-left: 4px solid #f59e0b; border-radius: 8px; padding: 16px; margin: 16px 0; background: rgba(245,158,11,0.08);">
<strong>Important:</strong> Find and Replace modifies article content directly and saves immediately. Always review the search results carefully before clicking Replace All. If something goes wrong, use Version History to restore any affected article.
</div>