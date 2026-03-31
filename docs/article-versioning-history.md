---
title: "Article Versioning & History"
description: "Track changes to articles with automatic version history and restore previous versions."
slug: "article-versioning-history"
status: "PUBLISHED"
createdAt: "2026-02-23T18:27:07.177Z"
updatedAt: "2026-03-21T03:04:33.945Z"
---

<h1>Article Versioning and History</h1>
<p>FinalDoc automatically keeps a version history of every article. Every time you save, a snapshot is created. You can browse past versions, compare them, and restore any version at any time — without losing your current work.</p>

<h2>How Versioning Works</h2>
<p>Every save creates a new version record in the database. Version records store:</p>
<ul>
<li>The full article content at the time of save</li>
<li>The title and description at the time of save</li>
<li>The author who made the save (their name)</li>
<li>The date and time of save</li>
<li>A change note (optional — you provide this)</li>
</ul>
<p>Versions are stored indefinitely. There is no automatic cleanup. You can manually delete individual versions if you want to tidy up the history.</p>

<h2>Adding Change Notes</h2>
<p>When saving an article, you can add a brief description of what you changed. This makes the version history much easier to read.</p>
<ol>
<li>Open the article</li>
<li>Make your edits</li>
<li>Before pressing Save (or instead of autosave), look for the <strong>Change Note</strong> field in the right Inspector panel</li>
<li>Type a short note like "Updated installation steps for v2" or "Fixed typo in Step 3"</li>
<li>Save the article — the note is stored with this version</li>
</ol>

<h2>Viewing Version History</h2>
<ol>
<li>Open the article in the editor</li>
<li>In the right Inspector panel, click <strong>Version History</strong></li>
<li>A list of all saved versions appears, ordered newest to oldest</li>
<li>Each entry shows: date, time, author name, and change note (if provided)</li>
</ol>

<h2>Previewing a Past Version</h2>
<ol>
<li>Click any version in the history list</li>
<li>A preview pane shows the article as it was at that point in time</li>
<li>You can scroll through the content to review it</li>
</ol>

<h2>Restoring a Version</h2>
<p>To roll back to a previous version:</p>
<ol>
<li>Open the version you want in the preview pane</li>
<li>Click the <strong>Restore</strong> button</li>
<li>FinalDoc first saves the current content as a new version (so you can undo the restore if needed)</li>
<li>The article editor then loads the restored version</li>
<li>The status remains as it was — if it was Published, it stays published. If it was Draft, it stays draft</li>
<li>To make the restored version live, click <strong>Save</strong> and then <strong>Publish</strong></li>
</ol>

<div style="border-left: 4px solid #f59e0b; border-radius: 8px; padding: 16px; margin: 16px 0; background: rgba(245,158,11,0.08);">
<strong>Important:</strong> Restoring a version does not automatically publish the change. It loads the old content into the editor as a draft. You still need to save and publish as normal.
</div>

<h2>Version History in PDF Exports</h2>
<p>When exporting articles to PDF, you can optionally include a <strong>Changelog</strong> section at the end of each article. This shows the version history (dates, authors, change notes) so readers can see when and how the article was updated. Enable this option in <strong>Toolbox → PDF Export → Include Change Notes</strong>.</p>