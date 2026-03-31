---
title: "Backup & Restore"
description: "Creating and restoring backups of your documentation."
slug: "backup-restore"
status: "PUBLISHED"
createdAt: "2026-02-23T18:16:35.024Z"
updatedAt: "2026-03-12T13:27:34.593Z"
---

<h1>Backup and Restore</h1>
<p>FinalDoc's Backup and Restore feature lets you create encrypted snapshots of your project and restore from them if something goes wrong. Use backups before major changes, before bulk operations, or on a regular schedule as an insurance policy.</p>

<h2>Opening Backup and Restore</h2>
<ol>
<li>Go to <strong>Settings</strong> in the left sidebar</li>
<li>Click <strong>Data &amp; Compliance</strong> → <strong>Backup &amp; Restore</strong></li>
</ol>

<h2>Creating a Backup</h2>
<ol>
<li>Click <strong>Create Backup Now</strong></li>
<li>Give the backup a <strong>description</strong> (optional but recommended — e.g., "Before bulk delete of old articles" or "Pre-migration snapshot")</li>
<li>Click <strong>Create</strong></li>
<li>The backup runs in the background. A progress indicator shows while it is processing</li>
<li>When complete, the backup appears in the backup list with a timestamp, size, and your description</li>
</ol>
<p>FinalDoc keeps up to <strong>10 backups per project</strong>. When you create backup #11, the oldest one is automatically deleted.</p>

<h2>What Gets Backed Up</h2>
<p>A full backup snapshot includes:</p>
<ul>
<li>All articles (draft and published) with their full content</li>
<li>All categories and their structure</li>
<li>Project settings (branding, AI configuration, domain settings, etc.)</li>
<li>Reader accounts and groups (if reader authentication is enabled)</li>
<li>Glossary terms, snippets, variables, and templates</li>
</ul>
<p>Note: Files in Drive (uploaded images and documents) are stored separately in DigitalOcean Spaces and are not included in the backup snapshot.</p>

<h2>Restoring from a Backup</h2>
<ol>
<li>In the Backup list, find the snapshot you want to restore from</li>
<li>Click <strong>Restore</strong></li>
<li>Choose what to restore:
  <ul>
    <li><strong>Full restore</strong> — Restores everything (articles, settings, readers)</li>
    <li><strong>Articles only</strong> — Restores article content without affecting settings</li>
    <li><strong>Settings only</strong> — Restores project configuration without touching content</li>
  </ul>
</li>
<li>Confirm the restore — a dialog warns you that this will overwrite current data</li>
<li>Click <strong>Restore Now</strong></li>
<li>The restore process runs. When complete, the page reloads with the restored data</li>
</ol>

<div style="border-left: 4px solid #ef4444; border-radius: 8px; padding: 16px; margin: 16px 0; background: rgba(239,68,68,0.08);">
<strong>Warning:</strong> A restore overwrites your current data with the backup snapshot. This is irreversible. Always create a new backup of your current state before restoring, so you can undo the restore if needed.
</div>

<h2>Downloading a Backup</h2>
<p>You can download a backup as an encrypted ZIP file for off-site storage:</p>
<ol>
<li>Find the backup in the list</li>
<li>Click <strong>Download</strong></li>
<li>Save the file securely — it contains all your project data</li>
</ol>
<p>This file can also be uploaded to a different FinalDoc account to migrate your project.</p>

<h2>Automatic Backups</h2>
<p>FinalDoc does not create automatic scheduled backups in the free plan. If you want regular automated backups, you can set a reminder to create them manually, or contact support about Enterprise backup options.</p>