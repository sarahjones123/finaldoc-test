---
title: "Drive & Storage API Reference"
description: ""
slug: "drive-storage-api-reference"
status: "PUBLISHED"
createdAt: "2026-02-24T08:32:54.580Z"
updatedAt: "2026-03-27T10:29:46.727Z"
---

<h1>Drive &amp; Storage API Reference</h1>
<p>The Drive &amp; Storage API lets you programmatically upload, list, and manage files in your FinalDoc Drive — the media library for your knowledge base.</p>

<h2>List Files</h2>
<pre><code>GET /projects/{projectId}/drive/files</code></pre>

<p><strong>Query parameters:</strong></p>
<ul>
<li><code>folderId</code> — List files in a specific folder (omit for root)</li>
<li><code>type</code> — Filter by file type: <code>image</code>, <code>pdf</code>, <code>video</code>, <code>document</code>, <code>other</code></li>
<li><code>search</code> — Search files by name</li>
<li><code>limit</code> — Max results (default 50)</li>
<li><code>offset</code> — Pagination offset</li>
</ul>

<p><strong>Example response:</strong></p>
<pre><code>{
  "files": [
    {
      "id": "file_abc",
      "name": "getting-started-screenshot.png",
      "type": "image",
      "size": 184320,
      "mimeType": "image/png",
      "folderId": null,
      "publicUrl": "https://app.finaldoc.io/api/public/media/file_abc",
      "isPublic": true,
      "uploadedBy": "user_xyz",
      "uploadedAt": "2026-02-15T10:30:00Z"
    }
  ],
  "total": 247
}</code></pre>

<h2>Get File</h2>
<pre><code>GET /projects/{projectId}/drive/files/{fileId}</code></pre>
<p>Returns a single file's metadata. Does not return the file content itself — use the <code>publicUrl</code> to access the file directly.</p>

<h2>Upload File</h2>
<pre><code>POST /projects/{projectId}/drive/upload</code></pre>
<p>Uploads a file to Drive. Use <code>multipart/form-data</code> encoding.</p>

<p><strong>Form fields:</strong></p>
<ul>
<li><code>file</code> — The file to upload (required)</li>
<li><code>folderId</code> — Target folder ID (optional; uploads to root if omitted)</li>
<li><code>makePublic</code> — <code>true</code> to immediately make the file publicly accessible (default: <code>false</code>)</li>
</ul>

<p><strong>Example (curl):</strong></p>
<pre><code>curl -X POST https://app.finaldoc.io/api/projects/{projectId}/drive/upload   -H "Authorization: Bearer fd_your_token"   -F "file=@/path/to/screenshot.png"   -F "makePublic=true"</code></pre>

<p>Returns the created file object including its <code>id</code> and <code>publicUrl</code>.</p>

<h2>Update File</h2>
<pre><code>PUT /projects/{projectId}/drive/files/{fileId}</code></pre>
<p>Update file metadata — rename the file, move to a different folder, or update visibility.</p>

<p><strong>Request body:</strong></p>
<pre><code>{
  "name": "new-filename.png",
  "folderId": "folder_abc",
  "isPublic": true
}</code></pre>

<h2>Delete File</h2>
<pre><code>DELETE /projects/{projectId}/drive/files/{fileId}</code></pre>
<p>Permanently deletes the file from Drive and the CDN. Returns 204 No Content. This cannot be undone — files embedded in articles will show as broken images after deletion.</p>

<h2>List Folders</h2>
<pre><code>GET /projects/{projectId}/drive/folders</code></pre>
<p>Returns the folder tree for Drive.</p>

<h2>Create Folder</h2>
<pre><code>POST /projects/{projectId}/drive/folders</code></pre>

<p><strong>Request body:</strong></p>
<pre><code>{
  "name": "Screenshots",
  "parentId": null
}</code></pre>
<p>Set <code>parentId</code> to create a sub-folder inside an existing folder. Returns the created folder object.</p>

<h2>Get Public File URL</h2>
<p>Public files are accessible at:</p>
<pre><code>https://app.finaldoc.io/api/public/media/{fileId}</code></pre>
<p>This URL redirects (302) to the CDN URL on DigitalOcean Spaces. The CDN URL may change — always use the <code>/api/public/media/{fileId}</code> URL for stable, permanent links to Drive files.</p>

<h2>Authentication</h2>
<p>Drive API endpoints require a session token (<code>fd_</code>) with at least EDITOR role on the project. File upload and deletion require EDITOR or above.</p>