---
title: "Paste from External Sources"
description: ""
slug: "paste-from-external-sources"
status: "PUBLISHED"
createdAt: "2026-02-24T08:32:54.697Z"
updatedAt: "2026-03-12T08:48:54.576Z"
---

<h1>Paste from External Sources</h1>
<p>You can paste content into the FinalDoc editor from almost any source — Word documents, Google Docs, Notion, websites, HTML editors, and plain text. FinalDoc cleans up the formatting automatically so you do not end up with messy inline styles.</p>

<h2>Pasting from Microsoft Word</h2>
<ol>
<li>Open your Word document and select the content you want</li>
<li>Copy it (<strong>Ctrl+C / Cmd+C</strong>)</li>
<li>Click inside the FinalDoc editor where you want to paste</li>
<li>Paste (<strong>Ctrl+V / Cmd+V</strong>)</li>
</ol>
<p>FinalDoc strips Word-specific XML and converts formatting to clean HTML:</p>
<ul>
<li>Headings (H1, H2, H3) are preserved</li>
<li>Bold, italic, and underline are preserved</li>
<li>Bullet lists and numbered lists are preserved</li>
<li>Tables are preserved (basic structure)</li>
<li>Font colors, font sizes, and spacing overrides are stripped (your KB theme controls these)</li>
<li>Tracked changes and comments are stripped</li>
</ul>

<h2>Pasting from Google Docs</h2>
<p>Same process — select, copy, paste. Google Docs formatting converts cleanly:</p>
<ul>
<li>All heading levels, lists, tables, and basic formatting carry over</li>
<li>Images: Google Docs images may not paste directly (they require special auth). Use <strong>Paste as plain text</strong> then insert images separately from Drive</li>
</ul>

<h2>Pasting from Notion</h2>
<p>Copy content from Notion pages and paste directly. Notion-specific blocks (toggles, databases, callouts) will be simplified to their closest FinalDoc equivalent.</p>

<h2>Pasting from a Website</h2>
<p>When you copy text from a webpage and paste it, the HTML formatting comes with it. FinalDoc keeps useful formatting (headings, bold, lists) and strips site-specific styles (colors, fonts, margins).</p>

<h2>Pasting as Plain Text</h2>
<p>If you want to paste without any formatting at all — just the raw text:</p>
<ul>
<li>Windows: Press <strong>Ctrl+Shift+V</strong></li>
<li>Mac: Press <strong>Cmd+Shift+V</strong></li>
<li>Or paste normally, then click the small paste options icon that appears → choose "Paste as plain text"</li>
</ul>

<h2>Pasting Images</h2>
<p>If you take a screenshot (with a tool like Snagit, ShareX, macOS screenshot, or Windows Snipping Tool) and copy it to your clipboard:</p>
<ol>
<li>Click in the editor where you want the image</li>
<li>Press <strong>Ctrl+V / Cmd+V</strong></li>
<li>The image is detected and uploaded to your Drive automatically, then inserted at the cursor</li>
</ol>

<h2>Pasting Code</h2>
<p>When you paste code from an IDE, terminal, or another page:</p>
<ul>
<li>If you paste into a <strong>code block</strong> (already inserted), the code pastes as-is with correct indentation</li>
<li>If you paste into a regular text area, the code is inserted as plain text with no highlighting</li>
<li>For best results, insert a code block first (<strong>Ctrl+Shift+K</strong>), then paste your code inside it</li>
</ul>

<h2>Import vs. Paste</h2>
<p>For large documents (entire articles or documentation sections), consider using the <strong>Import</strong> feature in Toolbox instead of pasting. Import handles Markdown files, HTML files, Confluence XML exports, Zendesk exports, DOCX files, and DITA files — and creates articles with proper structure automatically.</p>