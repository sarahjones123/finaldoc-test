---
title: "Recycle Bin & Article Recovery"
description: "Recover deleted articles and categories from the trash within 30 days."
slug: "recycle-bin-article-recovery"
status: "PUBLISHED"
createdAt: "2026-02-24T03:51:19.463Z"
updatedAt: "2026-03-21T03:04:34.017Z"
---

<h1>Recycle Bin and Article Recovery</h1>
<p>When you delete an article in FinalDoc, it does not disappear immediately. It goes to the <strong>Recycle Bin</strong> first — a safety net that holds deleted articles for 30 days, giving you time to recover anything deleted by mistake.</p>

<h2>How Deletion Works</h2>
<ul>
<li>When you delete an article (individually or via bulk delete), it is marked as deleted in the database and removed from the public knowledge base</li>
<li>The article is no longer visible to readers or in normal admin views</li>
<li>It sits in the Recycle Bin for <strong>30 days</strong></li>
<li>After 30 days, it is permanently erased automatically</li>
</ul>

<h2>Accessing the Recycle Bin</h2>
<ol>
<li>Go to <strong>Documentation</strong> in the left sidebar</li>
<li>At the bottom of the article tree panel, look for a <strong>trash icon</strong> or a link that says <strong>Recycle Bin</strong></li>
<li>Click it to open the Recycle Bin view</li>
<li>You will see a list of deleted articles with:
  <ul>
    <li>Article title</li>
    <li>Original category</li>
    <li>Date deleted</li>
    <li>Days remaining before permanent deletion</li>
  </ul>
</li>
</ol>

<h2>Restoring a Deleted Article</h2>
<ol>
<li>Find the article in the Recycle Bin</li>
<li>Click the <strong>Restore</strong> button next to it</li>
<li>The article is restored to its original category as a <strong>Draft</strong> (it will not automatically re-publish — you need to review and publish it manually)</li>
<li>If the original category no longer exists, the article is restored to the default workspace root</li>
</ol>

<h2>Permanently Deleting an Article</h2>
<p>If you are sure you do not need an article and want to free up space or clean up the Recycle Bin:</p>
<ol>
<li>Find the article in the Recycle Bin</li>
<li>Click <strong>Delete Permanently</strong></li>
<li>Confirm the action in the dialog that appears</li>
<li>The article is erased from the database immediately and cannot be recovered</li>
</ol>

<div style="border-left: 4px solid #ef4444; border-radius: 8px; padding: 16px; margin: 16px 0; background: rgba(239,68,68,0.08);">
<strong>Warning:</strong> Permanent deletion is irreversible. Once you confirm, there is no way to get the article back. Make sure you have exported a copy if you might need the content later.
</div>

<h2>Bulk Actions in the Recycle Bin</h2>
<p>To restore or permanently delete multiple articles at once:</p>
<ol>
<li>In the Recycle Bin view, check the checkboxes next to multiple articles</li>
<li>Use the bulk action bar to <strong>Restore All</strong> or <strong>Delete All Permanently</strong></li>
</ol>

<h2>Category Deletion and Recycle Bin</h2>
<p>When you delete a category that contains articles, you are given a choice:</p>
<ul>
<li><strong>Move articles to another category</strong> — The category is deleted, but the articles survive in the new location</li>
<li><strong>Delete articles too</strong> — All articles inside the category are moved to the Recycle Bin along with the category deletion</li>
</ul>