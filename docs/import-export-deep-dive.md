---
title: "Import & Export Deep Dive"
description: ""
slug: "import-export-deep-dive"
status: "PUBLISHED"
createdAt: "2026-02-24T08:37:07.747Z"
updatedAt: "2026-03-12T09:34:05.690Z"
---

<h1>Import &amp; Export Deep Dive</h1>
<p>FinalDoc's Import/Export system lets you bring in content from other platforms (Confluence, Zendesk, Notion, Word, Markdown) and export your entire knowledge base out of FinalDoc in multiple formats. This article covers the full capabilities of the import and export system.</p>

<h2>Opening Import/Export</h2>
<ol>
<li>Click <strong>Toolbox</strong> in the left sidebar</li>
<li>Click <strong>Import / Export</strong></li>
</ol>

<h2>Import: Supported Formats</h2>
<table>
<thead><tr><th>Format</th><th>Source</th><th>What Imports</th></tr></thead>
<tbody>
<tr><td><strong>Markdown (.md)</strong></td><td>Notion, GitHub, GitBook, Docusaurus</td><td>Content, headings, lists, code blocks, links</td></tr>
<tr><td><strong>HTML (.html)</strong></td><td>Any HTML source</td><td>Content and basic formatting</td></tr>
<tr><td><strong>Word (.docx)</strong></td><td>Microsoft Word</td><td>Content, headings, tables, lists, images</td></tr>
<tr><td><strong>Confluence Export</strong></td><td>Confluence XML space export</td><td>Articles, categories/spaces, basic formatting</td></tr>
<tr><td><strong>Zendesk Export</strong></td><td>Zendesk Help Center JSON</td><td>Articles and categories</td></tr>
<tr><td><strong>FinalDoc JSON</strong></td><td>FinalDoc export</td><td>Full fidelity — articles, categories, metadata, settings</td></tr>
<tr><td><strong>DITA (.xml)</strong></td><td>DITA-compliant XML</td><td>Content and structure</td></tr>
</tbody>
</table>

<h2>How to Import</h2>
<ol>
<li>Click <strong>Import Content</strong></li>
<li>Select the import format</li>
<li>Upload your file(s) — or paste content directly for single-article imports</li>
<li>Review the import preview — FinalDoc shows you how many articles and categories will be created</li>
<li>Configure options:
  <ul>
    <li><strong>Target workspace</strong> — Which workspace the imported content goes into</li>
    <li><strong>Target category</strong> — Optional: put all imported articles under a specific category</li>
    <li><strong>Import as drafts</strong> — Don't publish imported articles automatically</li>
    <li><strong>Preserve original structure</strong> — Maintain the original category hierarchy</li>
  </ul>
</li>
<li>Click <strong>Import</strong></li>
<li>A progress bar shows import stages: Parsing → Validating → Creating categories → Creating articles → Uploading media</li>
</ol>

<h2>Export: Supported Formats</h2>
<ul>
<li><strong>FinalDoc JSON</strong> — Full backup including all metadata, settings, versions. Use for migrating to another FinalDoc project or backup</li>
<li><strong>Markdown ZIP</strong> — All articles as .md files in a folder structure matching your categories. Import into GitBook, Notion, or any Markdown-based tool</li>
<li><strong>HTML ZIP</strong> — All articles as standalone HTML files</li>
<li><strong>PDF</strong> — Export all articles as a single PDF or individual PDFs (see the PDF Export article)</li>
</ul>

<h2>How to Export</h2>
<ol>
<li>Click <strong>Export Content</strong></li>
<li>Choose export format</li>
<li>Select scope: all articles, a specific category, or selected articles</li>
<li>Click <strong>Export</strong></li>
<li>A download link appears when ready (large exports may take a minute to prepare)</li>
</ol>