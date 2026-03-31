---
title: "Performance & Loading Issues"
description: ""
slug: "performance-loading-issues"
status: "PUBLISHED"
createdAt: "2026-02-24T08:37:07.806Z"
updatedAt: "2026-03-12T09:37:06.373Z"
---

<h1>Performance &amp; Loading Issues</h1>
<p>FinalDoc is generally fast, but if you're experiencing slow page loads or the app feels sluggish, this guide covers the common causes and how to fix them.</p>

<h2>Admin Panel Is Slow to Load</h2>

<h3>Check Your Internet Connection</h3>
<p>FinalDoc requires a stable connection. Run a speed test at fast.com or speedtest.net. If your download speed is below 5 Mbps, that may be the issue — try switching to a different network or closer to your router.</p>

<h3>Clear Browser Cache</h3>
<ol>
<li>Press <strong>Ctrl+Shift+Delete</strong> (Cmd+Shift+Delete on Mac)</li>
<li>Select "Cached images and files" and "Cookies and site data"</li>
<li>Set the time range to "Last 7 days" or "All time"</li>
<li>Click <strong>Clear data</strong></li>
<li>Reload FinalDoc</li>
</ol>

<h3>Try a Different Browser</h3>
<p>If the admin panel is slow in one browser but faster in another, the issue is browser-specific. Try Chrome, Firefox, or Edge. Extensions can slow down web apps — try opening FinalDoc in an incognito/private window (which disables extensions) to test.</p>

<h3>Disable Browser Extensions</h3>
<p>Ad blockers, password managers, and productivity extensions can interfere with FinalDoc. Temporarily disable them and see if performance improves.</p>

<h2>Public Knowledge Base Is Slow for Readers</h2>

<h3>Large Images</h3>
<p>The most common cause of slow KB pages is large, uncompressed images. Check your article images:</p>
<ul>
<li>Images should be under 500KB for standard screenshots</li>
<li>Use JPEG for photos, PNG for screenshots and diagrams, WebP for everything if possible</li>
<li>Use a tool like TinyPNG (tinypng.com) to compress images before uploading</li>
</ul>

<h3>Too Many Embedded Videos</h3>
<p>Embedding multiple YouTube/Vimeo videos on one page significantly increases load time. Consider linking to videos instead of embedding, or moving to a dedicated video page.</p>

<h3>Custom JavaScript Conflicts</h3>
<p>Custom JavaScript in Settings → Appearance → Custom JavaScript runs on every page. Poorly written scripts can block page rendering. Temporarily disable your custom JavaScript to see if it improves performance.</p>

<h2>Editor Feels Laggy While Typing</h2>
<p>If the article editor feels slow while typing:</p>
<ul>
<li><strong>Very long articles</strong> — Articles over 10,000 words may feel slightly laggy in the editor. Consider splitting very long articles into multiple articles</li>
<li><strong>Many embedded images</strong> — Lots of full-size images in the editor consume memory. Use Drive-hosted images via URL rather than pasting directly</li>
<li><strong>Browser tab memory</strong> — If you have 50+ browser tabs open, the tab with FinalDoc may have reduced memory allocation. Close unused tabs</li>
</ul>

<h2>Reporting Performance Issues</h2>
<p>If none of the above resolves your issue, contact support at support@finaldoc.io with:</p>
<ul>
<li>Your browser and version</li>
<li>Operating system</li>
<li>Which specific page or action is slow</li>
<li>Approximate time when you noticed the issue</li>
</ul>