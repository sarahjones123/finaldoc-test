---
title: "Drive Overview"
description: "How to use FinalDoc Drive for file management."
slug: "drive-overview"
status: "PUBLISHED"
createdAt: "2026-02-23T18:13:43.427Z"
updatedAt: "2026-03-14T14:51:21.485Z"
---

<h1>Drive Overview</h1>
<p>Drive is FinalDoc's built-in file storage. Upload images, PDFs, videos, and other files to Drive, then use them in your articles, share them publicly, or let readers download them. All files in Drive are stored securely on DigitalOcean Spaces object storage.</p>

<h2>Opening Drive</h2>
<p>Click <strong>Drive</strong> (the folder icon) in the left sidebar.</p>

<h2>The Drive Interface</h2>
<p>Drive shows your files in a grid or list view:</p>
<ul>
<li>Files are organized in folders (create folders to keep things tidy)</li>
<li>Each file shows its name, size, type, and upload date</li>
<li>Click any file to preview it (images, PDFs, videos, and audio files have built-in previews)</li>
</ul>

<h2>Uploading Files</h2>
<p>Three ways to upload:</p>
<ol>
<li>Click <strong>Upload</strong> and select files from your computer (supports batch upload — select multiple files at once)</li>
<li>Drag and drop files directly from your desktop into the Drive window</li>
<li>When inserting an image in the article editor, the upload option automatically saves to Drive</li>
</ol>
<p>Supported file types: images (JPG, PNG, GIF, WebP, SVG), documents (PDF, DOCX, XLSX, PPTX), videos (MP4, WebM, MOV), audio (MP3, WAV), archives (ZIP), and more.</p>
<p>Maximum file size: <strong>50MB per file</strong>.</p>

<h2>Organizing with Folders</h2>
<ol>
<li>Click <strong>New Folder</strong></li>
<li>Enter a folder name</li>
<li>Click <strong>Create</strong></li>
<li>Drag files into folders to organize them</li>
</ol>
<p>Suggested organization: create folders by content type (Images, PDFs, Screenshots) or by topic (Product A, Onboarding, Marketing).</p>

<h2>Making Files Public</h2>
<p>Files in Drive are private by default — only team members can access them. To share a file with readers or embed it in a public article:</p>
<ol>
<li>Click the file to select it</li>
<li>Click <strong>Share</strong> → <strong>Make Public</strong></li>
<li>A public URL is generated (looks like: <code>https://cdn.finaldoc.io/accounts/.../filename.jpg</code>)</li>
<li>Copy the URL to use in articles or share externally</li>
</ol>
<p>Public files are accessible by anyone with the URL — they are not indexed or listed anywhere, but they are not password-protected.</p>

<h2>Downloading Files</h2>
<p>Click any file → <strong>Download</strong> to save it to your computer.</p>

<h2>Renaming and Deleting Files</h2>
<ul>
<li>Right-click a file or click the three-dot menu → <strong>Rename</strong></li>
<li>Right-click → <strong>Delete</strong> — permanently removes the file from storage</li>
</ul>

<div style="border-left: 4px solid #f59e0b; border-radius: 8px; padding: 16px; margin: 16px 0; background: rgba(245,158,11,0.08);">
<strong>Important:</strong> If you delete a file from Drive that is used in an article (e.g., an article image), the image will break in that article. Always check where a file is used before deleting it.
</div>

<h2>Storage Usage</h2>
<p>Your Drive storage usage is shown at the bottom of the Drive page. Storage limits depend on your FinalDoc plan. Upgrade in <strong>Settings → General → Billing</strong> if you need more storage.</p>