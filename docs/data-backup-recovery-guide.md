---
title: "Data Backup & Recovery Guide"
description: ""
slug: "data-backup-recovery-guide"
status: "PUBLISHED"
createdAt: "2026-02-24T08:37:07.794Z"
updatedAt: "2026-03-12T11:15:01.520Z"
---

<h1>Data Backup &amp; Recovery Guide</h1>
<p>FinalDoc lets you create manual backups of your project data at any time and restore from any backup point if something goes wrong. Use backups before major changes, before bulk operations, or on a regular schedule as a safety net.</p>

<h2>Opening Backup &amp; Restore</h2>
<ol>
<li>Go to <strong>Settings → Data &amp; Compliance → Backup &amp; Restore</strong></li>
</ol>

<h2>Manual Backups</h2>
<p>FinalDoc does not run automatic scheduled backups. You create backups manually whenever you want a snapshot:</p>
<ol>
<li>Go to <strong>Settings → Data &amp; Compliance → Backup &amp; Restore</strong></li>
<li>Click <strong>Create Backup Now</strong></li>
<li>Optionally add a label (e.g., "Before major article restructure")</li>
<li>Click <strong>Create</strong></li>
<li>FinalDoc generates the backup — this takes 30 seconds to 2 minutes depending on project size</li>
<li>The backup appears in the backup list with a green "Complete" badge</li>
</ol>
<p>FinalDoc stores up to <strong>10 backups per project</strong>. When you create backup #11, the oldest one is automatically deleted. Create backups regularly and download important ones for offline storage.</p>

<h2>When to Create a Backup</h2>
<ul>
<li>Before deleting or restructuring a large number of articles</li>
<li>Before performing a bulk import (in case the import creates unwanted changes)</li>
<li>Before making major settings changes (branding, security, domain)</li>
<li>Periodically as a routine safety measure (e.g., weekly)</li>
</ul>

<h2>What a Backup Contains</h2>
<ul>
<li>All articles (all drafts, published, and archived)</li>
<li>All categories and their structure</li>
<li>Project settings and configuration</li>
<li>Reader accounts and groups</li>
<li>Feedback and comments</li>
<li>Custom branding settings</li>
<li>Media references (Drive file metadata — not the actual files, which are stored separately on DigitalOcean Spaces CDN)</li>
</ul>

<h2>Restoring from Backup</h2>
<ol>
<li>In the backup list, find the backup you want to restore from</li>
<li>Click <strong>Restore</strong> next to it</li>
<li>Choose what to restore:
  <ul>
    <li><strong>Articles only</strong> — Restores article content and categories. Good for recovering accidentally deleted articles</li>
    <li><strong>Settings only</strong> — Restores project configuration. Good if settings got accidentally changed</li>
    <li><strong>Full restore</strong> — Restores everything. Use carefully — this overwrites all current data</li>
  </ul>
</li>
<li>FinalDoc creates a new backup of the current state before restoring (safety backup)</li>
<li>Click <strong>Confirm Restore</strong></li>
<li>The restore process runs. A progress bar shows completion</li>
</ol>

<div style="border-left: 4px solid #ef4444; border-radius: 8px; padding: 16px; margin: 16px 0; background: rgba(239,68,68,0.08);">
<strong>Warning:</strong> A full restore overwrites all current articles, settings, and data. Work done after the backup date will be lost. Always confirm you're restoring from the right backup before proceeding.
</div>

<h2>Downloading a Backup</h2>
<p>Click the <strong>Download</strong> button next to any backup to download it as a JSON file. Store this file offline as an additional safety copy, or use it to migrate the project to another FinalDoc account.</p>