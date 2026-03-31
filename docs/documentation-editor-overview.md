---
title: "Documentation Editor Overview"
description: "An overview of the FinalDoc Documentation editor — layout, toolbar, autosave, the properties panel, and AI writing tools."
slug: "documentation-editor-overview"
status: "PUBLISHED"
createdAt: "2026-02-23T18:13:42.847Z"
updatedAt: "2026-03-21T06:03:10.226Z"
---

<h1>Documentation Editor Overview</h1>
<p>The Documentation editor is where all writing happens. It opens when you click <strong>Documentation</strong> in the left sidebar. The editor is split into three main areas.</p>

<h2>Editor Layout</h2>

<h3>Left Panel — Article Tree</h3>
<p>The left panel shows your knowledge base structure:</p>
<ul>
<li><strong>Categories</strong> — Folder icons. Click to expand/collapse. Drag to reorder.</li>
<li><strong>Articles</strong> — Listed under their parent category. Click to open.</li>
<li><strong>+ button</strong> — Appears on hover next to each category. Click to add an article or subcategory.</li>
<li><strong>⋮ button</strong> — Article/category options: rename, move, duplicate, delete, pin, set colour.</li>
</ul>
<p>You can search articles in the tree using the search box at the top of the left panel.</p>

<h3>Centre — Editor Canvas</h3>
<p>A full-width writing area. Click anywhere to place your cursor and start typing. The editor supports:</p>
<ul>
<li>Rich text (bold, italic, underline, strikethrough, inline code)</li>
<li>Headings (H1–H6)</li>
<li>Bullet and numbered lists (including nested)</li>
<li>Tables (add, remove rows/columns, merge cells)</li>
<li>Images (drag-and-drop or paste from clipboard)</li>
<li>Code blocks with syntax highlighting</li>
<li>Callout blocks (Info, Warning, Success, Error)</li>
<li>Math (LaTeX via KaTeX)</li>
<li>Diagrams (Mermaid)</li>
<li>Embedded videos (YouTube, Vimeo, or direct file)</li>
<li>Horizontal rules, blockquotes</li>
</ul>

<h3>Right Panel — Properties</h3>
<p>Click the <strong>Properties</strong> icon (four-square grid) in the toolbar to toggle the right panel. It contains:</p>
<ul>
<li><strong>Status</strong> — Draft or Published. Change here or use the Publish button.</li>
<li><strong>Description</strong> — Short summary shown in search results and on the KB homepage</li>
<li><strong>Featured Image</strong> — Thumbnail shown in category listings</li>
<li><strong>Draft Writer</strong> — Override the displayed author name</li>
<li><strong>Tags</strong> — Add internal content tags</li>
<li><strong>SEO</strong> — Custom meta title and description</li>
<li><strong>Reactions</strong> — Enable/disable emoji reactions for readers</li>
<li><strong>Tasks</strong> — Assign to-do tasks linked to this article</li>
<li><strong>Reading Progress</strong> — Shows estimated reading time</li>
</ul>

<h2>Toolbar</h2>
<p>The toolbar at the top of the editor contains:</p>
<table>
<thead><tr><th>Button</th><th>Function</th></tr></thead>
<tbody>
<tr><td><strong>Undo/Redo</strong></td><td>Standard undo/redo (also <kbd>Ctrl+Z</kbd> / <kbd>Ctrl+Y</kbd>)</td></tr>
<tr><td><strong>Format dropdown</strong></td><td>Paragraph, Heading 1–6, Code block</td></tr>
<tr><td><strong>Bold, Italic, Underline</strong></td><td>Inline text formatting</td></tr>
<tr><td><strong>Link</strong></td><td>Insert or edit a hyperlink</td></tr>
<tr><td><strong>Image</strong></td><td>Upload or embed an image</td></tr>
<tr><td><strong>Table</strong></td><td>Insert a table</td></tr>
<tr><td><strong>Callout</strong></td><td>Insert an Info/Warning/Success/Error block</td></tr>
<tr><td><strong>AI button</strong></td><td>Opens the AI writing assistant (Ved AI Writer)</td></tr>
<tr><td><strong>History (clock)</strong></td><td>Opens the Version History / Changelog modal</td></tr>
<tr><td><strong>Properties (grid)</strong></td><td>Toggles the right properties panel</td></tr>
<tr><td><strong>Publish</strong></td><td>Publishes the current draft (or opens the publish dialog if already published)</td></tr>
<tr><td><strong>Translate</strong></td><td>One-click AI translation to another language</td></tr>
</tbody>
</table>

<h2>Autosave</h2>
<p>FinalDoc saves your work automatically every few seconds as you type. You&apos;ll see <em>&ldquo;Saved&rdquo;</em> in the top-right corner when the latest version is saved. You never need to press a save button for your draft.</p>

<h2>Publishing</h2>
<ol>
<li>Click the <strong>Publish</strong> button in the toolbar.</li>
<li>Optionally enter a <strong>Change Note</strong> in the dialog (this appears in the article&apos;s public changelog).</li>
<li>Click <strong>Publish</strong> to confirm. The article immediately goes live on your knowledge base.</li>
</ol>
<p>To unpublish, click the <strong>Status</strong> dropdown in the Properties panel and select <strong>Draft</strong>.</p>

<h2>Version History</h2>
<p>Click the <strong>History</strong> (clock) icon to open the Version History modal. Every published version is stored. You can:</p>
<ul>
<li>Preview any version</li>
<li>Restore a previous version with one click</li>
<li>See change notes on the Changelog tab</li>
</ul>

<h2>AI Writing Assistant (Ved AI Writer)</h2>
<p>Select any text in the editor and click the <strong>AI</strong> button (or press <kbd>Ctrl+Shift+A</kbd>) to open the AI writing panel. You can ask it to:</p>
<ul>
<li><strong>Continue writing</strong> — Extend the selected text</li>
<li><strong>Rewrite</strong> — Rephrase while preserving meaning</li>
<li><strong>Summarise</strong> — Condense long text</li>
<li><strong>Fix grammar</strong> — Correct errors</li>
<li><strong>Simplify</strong> — Make content easier to read</li>
<li><strong>Translate</strong> — Convert to another language</li>
<li><strong>Custom prompt</strong> — Type any instruction</li>
</ul>

<h2>Keyboard Shortcuts</h2>
<p>Press <kbd>?</kbd> in the editor to open the full shortcuts reference. Common ones:</p>
<table>
<thead><tr><th>Shortcut</th><th>Action</th></tr></thead>
<tbody>
<tr><td><kbd>Ctrl+B</kbd></td><td>Bold</td></tr>
<tr><td><kbd>Ctrl+I</kbd></td><td>Italic</td></tr>
<tr><td><kbd>Ctrl+K</kbd></td><td>Insert link</td></tr>
<tr><td><kbd>Ctrl+Shift+A</kbd></td><td>Open AI assistant</td></tr>
<tr><td><kbd>Ctrl+Z</kbd></td><td>Undo</td></tr>
<tr><td><kbd>Ctrl+Y</kbd></td><td>Redo</td></tr>
<tr><td><kbd>/</kbd> at start of line</td><td>Open block-type picker</td></tr>
</tbody>
</table>