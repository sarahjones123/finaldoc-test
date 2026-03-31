---
title: "Creating and Managing Articles"
description: "How to create, edit, publish, and delete articles."
slug: "creating-and-managing-articles"
status: "PUBLISHED"
createdAt: "2026-02-23T18:13:42.869Z"
updatedAt: "2026-03-21T06:03:10.254Z"
---

<h1>Creating and Managing Articles</h1>
<p>Articles are the core building blocks of your knowledge base. Each article is a single page of content that your readers can search for, read, and interact with. This guide covers the complete article lifecycle — from creating a blank page to archiving or deleting old content.</p>

<h2>Creating a New Article</h2>
<p>There are several ways to create a new article:</p>
<ul>
<li><strong>From the sidebar</strong> — Click the <strong>+</strong> icon next to a category in the left panel, then choose "New Article"</li>
<li><strong>From the toolbar</strong> — Click the <strong>+ New Article</strong> button at the top of the Documentation page</li>
<li><strong>Keyboard shortcut</strong> — Press <strong>Ctrl+N / Cmd+N</strong> while in Documentation view</li>
</ul>
<p>After clicking, you'll be prompted to enter a title. Type a clear, descriptive title (e.g., "How to Reset Your Password") and press Enter. The article opens immediately in the editor, ready to write.</p>

<h2>Writing and Formatting</h2>
<p>The editor is a rich-text surface — click anywhere and start typing. Use the toolbar at the top to apply formatting:</p>
<ul>
<li><strong>Headings</strong> — Use H1, H2, H3 to structure your content with a clear hierarchy</li>
<li><strong>Bold / Italic / Underline</strong> — Standard text emphasis with Ctrl+B, Ctrl+I, Ctrl+U</li>
<li><strong>Lists</strong> — Bullet lists and numbered lists for step-by-step instructions</li>
<li><strong>Links</strong> — Ctrl+K to insert a hyperlink to an external URL or another article</li>
<li><strong>Images</strong> — Insert images from Drive, paste from clipboard, or drag and drop</li>
<li><strong>Tables</strong> — Insert a table grid for comparing options or showing data</li>
<li><strong>Code blocks</strong> — Syntax-highlighted code with language selection</li>
<li><strong>Callout blocks</strong> — Info, warning, tip, and danger boxes to highlight key points</li>
<li><strong>Dividers</strong> — Horizontal rules to visually separate sections</li>
</ul>

<h2>Article Properties (Inspector Panel)</h2>
<p>The right-side Inspector panel contains article-level settings. Click the panel toggle or press <strong>Ctrl+Shift+I</strong> to open or close it:</p>
<ul>
<li><strong>Description</strong> — A 1–2 sentence summary shown in search results, category listings, and social media previews. Always fill this in</li>
<li><strong>Featured Image</strong> — Displayed as a thumbnail in article lists and used as the Open Graph image for social sharing</li>
<li><strong>Tags</strong> — Keywords for filtering and discoverability. Click "Add tag" to assign existing tags or create new ones</li>
<li><strong>Reading Time</strong> — Auto-calculated from word count, but you can override it manually</li>
<li><strong>Draft Writer</strong> — Set the displayed author name (defaults to the logged-in user)</li>
<li><strong>Slug</strong> — The URL-safe identifier for the article (e.g., "how-to-reset-password"). Auto-generated from title, but can be customized</li>
<li><strong>Change Note</strong> — When saving, you can enter a brief note about what changed. Visible in Version History</li>
</ul>

<h2>Saving</h2>
<p>FinalDoc saves your article <strong>automatically</strong> as you type — you will see a small "Saved" indicator at the top of the editor. You can also save manually at any time with <strong>Ctrl+S / Cmd+S</strong>.</p>
<p>Saved drafts are not visible to readers. Only published articles appear on the public knowledge base.</p>

<h2>Publishing</h2>
<p>When your article is ready for readers to see:</p>
<ol>
<li>Click the <strong>Publish</strong> button in the top-right of the editor</li>
<li>The status badge changes from <strong>Draft</strong> (grey) to <strong>Published</strong> (green)</li>
<li>The article immediately appears on your public knowledge base at your project URL</li>
</ol>
<p>To unpublish a live article, click the <strong>Published</strong> badge and select <strong>Set to Draft</strong>. This removes it from public view instantly without deleting it.</p>

<h2>Version History</h2>
<p>Every time you save an article, FinalDoc creates a version snapshot. To review or restore a previous version:</p>
<ol>
<li>Open the article</li>
<li>Click <strong>Version History</strong> in the right-side Inspector panel</li>
<li>Browse the list of saves with timestamps, author names, and change notes</li>
<li>Click any version to preview it</li>
<li>Click <strong>Restore</strong> to roll back to that version (the current version is saved first as a backup)</li>
</ol>

<h2>Organizing Articles</h2>
<p>Articles live inside categories. You can reorganize them at any time:</p>
<ul>
<li><strong>Drag and drop</strong> — Grab an article in the left panel and drag it to a different category or position</li>
<li><strong>Move article</strong> — Right-click an article → Move to → select destination category</li>
<li><strong>Rename</strong> — Double-click the article title in the sidebar, or edit the Title field at the top of the editor</li>
<li><strong>Duplicate</strong> — Right-click an article → Duplicate (creates a draft copy with "(Copy)" in the title)</li>
</ul>

<h2>Article Status</h2>
<p>Each article has one of these statuses:</p>
<ul>
<li><strong>Draft</strong> — Work in progress. Not visible to readers</li>
<li><strong>Published</strong> — Live and visible on the public knowledge base</li>
<li><strong>In Review</strong> — Submitted for approval (used with the Approval Flow workflow in Toolbox)</li>
<li><strong>Archived</strong> — Hidden from the KB but preserved in the database. Useful for outdated content you might need later</li>
</ul>

<h2>Pinning Articles</h2>
<p>You can pin important articles so they always appear at the top of their category in the public KB:</p>
<ol>
<li>Open the article</li>
<li>In the Inspector panel, find the <strong>Pin Article</strong> toggle and enable it</li>
<li>Pinned articles show a pin icon and appear above non-pinned articles in the same category</li>
</ol>

<h2>Bulk Actions</h2>
<p>To manage multiple articles at once, use <strong>Bulk Actions</strong> in the Documentation view:</p>
<ol>
<li>Click the <strong>Bulk Select</strong> checkbox at the top of the article list (or check individual articles)</li>
<li>Select the articles you want to act on</li>
<li>Choose an action from the toolbar: <strong>Publish All</strong>, <strong>Set to Draft</strong>, <strong>Move to Category</strong>, <strong>Delete</strong>, or <strong>Export</strong></li>
</ol>

<h2>Deleting Articles</h2>
<p>To delete an article:</p>
<ul>
<li>Right-click the article in the sidebar → <strong>Delete</strong></li>
<li>Or open the article → click the three-dot menu → <strong>Delete</strong></li>
</ul>
<p>Deleted articles are moved to the <strong>Recycle Bin</strong>. They are not permanently erased yet — you have 30 days to recover them. Go to <strong>Documentation → Recycle Bin</strong> (the trash icon in the sidebar) to restore or permanently delete them.</p>