---
title: "KB Table of Contents & Navigation"
description: ""
slug: "kb-table-of-contents-navigation"
status: "PUBLISHED"
createdAt: "2026-02-24T08:37:07.760Z"
updatedAt: "2026-03-12T09:32:33.740Z"
---

<h1>KB Table of Contents &amp; Navigation</h1>
<p>FinalDoc automatically generates a Table of Contents (TOC) for each article based on its headings (H2 and H3 tags). The TOC appears in a panel on the right side of the article page, helping readers navigate long articles. This article explains how the TOC works and how to configure it.</p>

<h2>How the TOC Is Generated</h2>
<p>FinalDoc reads your article's heading structure automatically:</p>
<ul>
<li><strong>H2 headings</strong> → Top-level TOC entries</li>
<li><strong>H3 headings</strong> → Indented sub-entries under the H2 above them</li>
<li><strong>H4 headings and below</strong> → Not included in the TOC (too granular)</li>
</ul>
<p>No setup required — just use proper heading hierarchy in your article and the TOC builds itself.</p>

<h2>TOC Behavior</h2>
<ul>
<li>The TOC panel is sticky — it stays visible as you scroll, always showing which section you're currently reading (the active heading is highlighted)</li>
<li>Click any TOC entry to jump directly to that section (smooth scroll)</li>
<li>On mobile, the TOC collapses and is accessible via a "Contents" button at the top of the article</li>
</ul>

<h2>Enabling/Disabling the TOC</h2>
<h3>Globally (all articles)</h3>
<ol>
<li>Go to <strong>Settings → Appearance → Article Display</strong></li>
<li>Find <strong>Show Table of Contents</strong> and toggle it ON or OFF</li>
</ol>

<h3>Per Article</h3>
<ol>
<li>Open the article in the editor</li>
<li>In the Inspector panel, find <strong>Table of Contents</strong></li>
<li>Set it to <strong>Show</strong>, <strong>Hide</strong>, or <strong>Use Global Setting</strong></li>
</ol>
<p>Articles shorter than 500 words automatically hide the TOC even when it's enabled globally — a TOC with only 1–2 entries isn't useful.</p>

<h2>TOC Anchor Links</h2>
<p>Each heading in your article gets an anchor link (a <code>#section-name</code> URL fragment). Readers can copy these anchor links to link directly to a specific section of your article from anywhere. The anchor link appears when you hover over a heading — a chain link icon appears that you can click to copy.</p>

<h2>KB Sidebar Navigation</h2>
<p>Beyond per-article TOC, the KB sidebar on the left shows the full category/article tree. Readers can:</p>
<ul>
<li>Browse categories (click to expand/collapse)</li>
<li>Click any article to navigate to it</li>
<li>Use the search bar above the sidebar to find articles</li>
</ul>
<p>Configure the sidebar behavior (open/collapsed state, show/hide article counts) in <strong>Settings → Appearance → Portal Builder → Navigation Options</strong>.</p>