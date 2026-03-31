---
title: "Content Migration Guide"
description: "Migrate your documentation from other platforms like Zendesk, Confluence, or WordPress."
slug: "content-migration-guide"
status: "PUBLISHED"
createdAt: "2026-02-24T03:51:25.577Z"
updatedAt: "2026-03-17T04:43:38.774Z"
---

<h1>Content Migration Guide</h1>
<p>Migrating your documentation from another platform to FinalDoc? This guide walks you through the complete migration process — from planning and exporting your existing content to importing it into FinalDoc, cleaning it up, and going live.</p>

<h2>Step 1: Audit Your Existing Content</h2>
<p>Before migrating, assess what you have:</p>
<ul>
<li>How many articles total?</li>
<li>Which articles are outdated and should be deleted rather than migrated?</li>
<li>Is your content organized logically, or does migration provide an opportunity to restructure?</li>
<li>What media (images, files) is embedded in articles?</li>
</ul>
<p>Make a spreadsheet of article titles, current URLs, and migration decisions (migrate, rewrite, skip).</p>

<h2>Step 2: Export from Your Current Platform</h2>
<p>Most platforms have a built-in export feature:</p>
<ul>
<li><strong>Confluence</strong> — Space Tools → Export Space → XML format</li>
<li><strong>Zendesk</strong> — Guide → Manage Articles → Export (CSV or JSON)</li>
<li><strong>Notion</strong> — Export as Markdown + CSV</li>
<li><strong>GitBook</strong> — Space settings → Export as PDF or Markdown</li>
<li><strong>WordPress</strong> — Tools → Export → All content (XML)</li>
</ul>

<h2>Step 3: Import into FinalDoc</h2>
<ol>
<li>Go to <strong>Toolbox → Import / Export → Import Content</strong></li>
<li>Select your export format</li>
<li>Upload the export file</li>
<li>Review the import preview</li>
<li>Configure import settings (target workspace, import as drafts)</li>
<li>Click <strong>Import</strong></li>
</ol>
<p>Import all content as <strong>drafts</strong> first — don't publish until after cleanup.</p>

<h2>Step 4: Clean Up After Import</h2>
<p>After importing, review the content in FinalDoc:</p>
<ul>
<li><strong>Images</strong> — Check that images imported correctly. Broken images need to be re-uploaded to Drive and re-inserted</li>
<li><strong>Links</strong> — Internal links between articles need to be updated to FinalDoc's URL format</li>
<li><strong>Formatting</strong> — Some formatting may not transfer perfectly; spot-check articles and fix layout issues</li>
<li><strong>Categories</strong> — Reorganize the category structure if needed (drag and drop in the sidebar)</li>
</ul>

<h2>Step 5: Set Up Redirects</h2>
<p>If your old documentation was at public URLs (e.g., docs.yourcompany.com/article/old-slug), set up redirects so existing links don't break:</p>
<ol>
<li>Go to <strong>Settings → Domain &amp; SEO → Redirects</strong></li>
<li>Add a redirect for each old URL → new FinalDoc URL</li>
</ol>
<p>See the Redirects article for details.</p>

<h2>Step 6: Go Live</h2>
<ol>
<li>Publish all migrated articles (bulk publish via Documentation → Select All → Publish)</li>
<li>Point your custom domain to FinalDoc (Settings → Domain &amp; SEO → Custom Domain)</li>
<li>Test your KB from a reader's perspective — search, navigate, check links</li>
<li>Remove the old documentation or put up a redirect page</li>
</ol>