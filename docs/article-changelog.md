---
title: "Article Changelog"
description: "Learn how readers can track article changes through the public changelog, powered by change notes from the editor."
slug: "article-changelog"
status: "PUBLISHED"
createdAt: "2026-02-27T10:22:40.936Z"
updatedAt: "2026-03-21T03:04:46.016Z"
---

<h1>Article Changelog</h1>
<p>The Article Changelog is a visible record of changes made to an article over time. It can be displayed on the public knowledge base to show readers when an article was last updated, who made the changes, and a brief description of what changed. This transparency builds reader trust by demonstrating that your documentation is actively maintained and up to date.</p>

<h2>How the Changelog Works</h2>
<p>Every time a team member saves an article, FinalDoc creates a version entry. The Article Changelog shows a curated list of notable saves — those where a change note was added. Saves without a change note are still recorded in the Version History (for internal use) but do not appear in the public changelog.</p>

<h2>Adding a Change Note When Saving</h2>
<ol>
<li>Open an article in the editor</li>
<li>Make your changes</li>
<li>Click the <strong>Save</strong> button (or press the save shortcut)</li>
<li>A dialog appears with an optional <strong>Change Note</strong> field</li>
<li>Type a brief summary of what you changed (e.g., "Updated installation steps for v3.2", "Corrected pricing information", "Added screenshots")</li>
<li>Click <strong>Save</strong></li>
</ol>
<p>Change notes are optional. If you skip it, the save is recorded internally but doesn't add an entry to the public changelog.</p>

<h2>Viewing the Changelog on the Public KB</h2>
<p>When a reader is viewing an article on the public knowledge base, they can see the changelog in two ways:</p>
<ul>
<li><strong>Last updated badge</strong> — The article page shows "Last updated [date]" near the article title</li>
<li><strong>Changelog section</strong> — At the bottom of the article (when enabled), a collapsible "What changed?" section lists the most recent change notes with dates and author names</li>
</ul>

<h2>Enabling the Public Changelog Display</h2>
<ol>
<li>Open the article in the Documentation editor</li>
<li>Click the <strong>Properties</strong> panel (right side)</li>
<li>Find the <strong>Changelog</strong> toggle</li>
<li>Enable <strong>Show changelog to readers</strong></li>
</ol>
<p>You can control this per-article.</p>

<h2>Viewing Version History (Internal)</h2>
<p>To see all saved versions of an article (not just the ones with change notes):</p>
<ol>
<li>Open the article in the editor</li>
<li>Click <strong>Version History</strong> in the article properties or the ... menu</li>
<li>A timeline of all saved versions appears</li>
<li>Click any version to preview it</li>
<li>Click <strong>Restore</strong> to revert to that version (your current version is saved first so you can undo the restore)</li>
</ol>

<h2>Changelog in PDF Export</h2>
<p>When exporting articles as PDF, you can optionally include the changelog:</p>
<ol>
<li>Open <strong>Toolbox → PDF Export</strong></li>
<li>Select articles to export</li>
<li>In the export options, enable <strong>Include Change Notes</strong></li>
<li>The generated PDF includes a changelog section at the end of each article listing change notes by date</li>
</ol>

<h2>Best Practices for Change Notes</h2>
<ul>
<li>Keep notes brief and specific — "Updated API endpoint from v1 to v2" is better than "Updated"</li>
<li>Note what changed and why when possible — "Added pricing table (Q2 update)"</li>
<li>Use consistent formatting across your team — consider a style guide for change notes</li>
<li>Skip change notes for minor typo fixes or formatting tweaks — save them for meaningful content changes</li>
</ul>