---
title: "File Sharing & Public URLs"
description: "Share files publicly, generate permanent short URLs, and use files in articles."
slug: "file-sharing-public-urls"
status: "PUBLISHED"
createdAt: "2026-02-24T03:50:54.708Z"
updatedAt: "2026-03-14T14:51:22.621Z"
---

<h1>File Sharing &amp; Public URLs</h1>
<p>Files in FinalDoc Drive can be made publicly accessible via a CDN URL — useful for embedding images in articles, linking to downloadable PDFs, or using a file as an Open Graph image for social media sharing. You control whether each file is public or private.</p>

<h2>Public vs. Private Files</h2>
<table>
<thead><tr><th>Visibility</th><th>Who Can Access</th><th>Use Case</th></tr></thead>
<tbody>
<tr><td><strong>Public</strong></td><td>Anyone with the URL</td><td>Images in articles, downloadable PDFs, logos, media you want to share</td></tr>
<tr><td><strong>Private</strong></td><td>Only authenticated team members via the admin panel</td><td>Internal reference files, confidential documents, raw source files</td></tr>
</tbody>
</table>

<h2>Making a File Public</h2>
<ol>
<li>Click the file in Drive to select it</li>
<li>In the right info panel, find <strong>Visibility</strong></li>
<li>Click <strong>Make Public</strong></li>
<li>The <strong>Public URL</strong> appears — copy it</li>
</ol>

<h2>The Public URL Format</h2>
<p>Public files are served from FinalDoc's CDN. The URL looks like:</p>
<pre><code>https://app.finaldoc.io/api/public/media/{fileId}</code></pre>
<p>This URL redirects to the actual CDN location (DigitalOcean Spaces). The URL is permanent — it won't break if you rename the file in Drive.</p>

<h2>Using File URLs in Articles</h2>
<p>When you insert an image or file link in the article editor:</p>
<ul>
<li>Images inserted from Drive are automatically linked using the public URL</li>
<li>For download links, use the public URL as the href in a hyperlink</li>
</ul>

<h2>Making a File Private</h2>
<ol>
<li>Click the file in Drive</li>
<li>In the info panel, click <strong>Make Private</strong></li>
<li>The public URL stops working — anyone trying to access it gets a 403 error</li>
</ol>
<p>Note: If articles are embedding this image using its public URL, those articles will show broken images after you make the file private. Check where the file is used before revoking public access.</p>

<h2>Short URLs</h2>
<p>For files you share frequently, FinalDoc generates a short URL alias. Click <strong>Copy Short URL</strong> in the file info panel to get a shorter, cleaner URL for use in emails, documentation links, or presentations.</p>

<h2>Access Logging</h2>
<p>FinalDoc does not currently log individual public file accesses (no analytics on how many times a file URL was accessed). If you need download tracking, host the file externally (e.g., on your own CDN) and link to it from Drive as an external URL.</p>