---
title: "Import & Export Project"
description: "Import content from other platforms or export your knowledge base in multiple formats."
slug: "import-export-project"
status: "PUBLISHED"
createdAt: "2026-02-23T18:26:48.761Z"
updatedAt: "2026-03-12T09:44:30.657Z"
---

<h1>Import and Export</h1>
<p>FinalDoc's Import and Export tools let you bring content in from other platforms or take it out to use elsewhere. Whether you are migrating from Confluence, Zendesk, or Notion, or just want to back up your documentation as Markdown files, these tools handle it.</p>

<h2>Opening Import and Export</h2>
<ol>
<li>Go to <strong>Toolbox</strong> in the left sidebar</li>
<li>Under <strong>Import and Export</strong>, click <strong>Import &amp; Export</strong></li>
</ol>

<h2>Importing Content</h2>
<h3>Supported Import Formats</h3>
<table>
<thead><tr><th>Format</th><th>Best For</th><th>Notes</th></tr></thead>
<tbody>
<tr><td>Markdown (.md)</td><td>Importing from GitHub, Notion, or any Markdown-based tool</td><td>Frontmatter (YAML) is parsed for title and description</td></tr>
<tr><td>HTML (.html)</td><td>Importing from website generators or CMS exports</td><td>Images linked in HTML must be accessible URLs</td></tr>
<tr><td>JSON</td><td>FinalDoc project exports</td><td>Full fidelity — preserves all metadata</td></tr>
<tr><td>Confluence XML</td><td>Migrating from Atlassian Confluence</td><td>Upload the Space Export ZIP from Confluence</td></tr>
<tr><td>Zendesk JSON</td><td>Migrating from Zendesk Guide</td><td>Export from Zendesk and upload the file</td></tr>
<tr><td>DOCX (.docx)</td><td>Importing from Microsoft Word</td><td>Formatting is converted; images may need re-uploading</td></tr>
<tr><td>DITA (.dita)</td><td>Importing from professional technical writing tools</td><td>Supports DITA topic files</td></tr>
</tbody>
</table>

<h3>How to Import</h3>
<ol>
<li>Click the <strong>Import</strong> tab</li>
<li>Select the import format</li>
<li>Upload your file (or paste a URL for online content)</li>
<li>FinalDoc shows a preview of what will be imported — the detected articles, their titles, and any warnings</li>
<li>Choose the <strong>destination category</strong> for the imported articles</li>
<li>Click <strong>Import</strong></li>
<li>Articles are created as Drafts — review them and publish when ready</li>
</ol>

<h2>Exporting Content</h2>
<h3>Supported Export Formats</h3>
<ul>
<li><strong>Markdown</strong> — One .md file per article in a ZIP archive. Great for storing in a git repository</li>
<li><strong>HTML</strong> — One .html file per article</li>
<li><strong>JSON</strong> — Full export with all metadata, suitable for re-importing into another FinalDoc project</li>
<li><strong>PDF</strong> — See the dedicated <strong>PDF Export</strong> article for details</li>
</ul>

<h3>How to Export</h3>
<ol>
<li>Click the <strong>Export</strong> tab</li>
<li>Select which articles to export: all articles, a specific category, or selected articles</li>
<li>Choose the export format</li>
<li>Click <strong>Export</strong></li>
<li>A ZIP file downloads to your computer containing all selected articles in the chosen format</li>
</ol>

<h2>Project Transfer (Full Backup)</h2>
<p>To export your entire project for backup or to migrate to another account:</p>
<ol>
<li>Under <strong>Import and Export</strong>, click <strong>Project Transfer</strong></li>
<li>Click <strong>Export Project</strong></li>
<li>A comprehensive ZIP file is generated containing all articles, categories, settings metadata, and assets</li>
<li>To restore this backup, go to <strong>Settings → Data &amp; Compliance → Backup &amp; Restore</strong> and upload the export file</li>
</ol>