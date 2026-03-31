---
title: "Custom Pages"
description: "Build custom static pages like Terms, Privacy, or About for your knowledge base."
slug: "custom-pages"
status: "PUBLISHED"
createdAt: "2026-02-23T18:26:51.851Z"
updatedAt: "2026-03-12T10:41:03.123Z"
---

<h1>Custom Pages (Portal Pages)</h1>
<p>Portal Pages (also called Custom Pages) let you create standalone pages on your public knowledge base that aren't regular articles — pages like a "Contact Us" form, an "About This Documentation" intro page, a status page link, or a glossary of terms. Custom pages appear in the KB navigation alongside your documentation.</p>

<h2>Opening Custom Pages</h2>
<ol>
<li>Click <strong>Toolbox</strong> in the left sidebar</li>
<li>Click <strong>Portal Pages</strong> (under Import &amp; Export)</li>
</ol>

<h2>Creating a Custom Page</h2>
<ol>
<li>Click <strong>+ New Page</strong></li>
<li>Enter a <strong>Page Title</strong> (appears in navigation and browser tab)</li>
<li>Enter a <strong>Slug</strong> — the URL path (e.g., <code>contact-us</code> → accessible at <code>yourproject.finaldoc.io/contact-us</code>)</li>
<li>Choose the <strong>page type</strong>:
  <ul>
    <li><strong>Custom Content</strong> — Write the page using the same rich text editor as articles</li>
    <li><strong>Redirect</strong> — This page redirects to an external URL (useful for linking to an external status page or support portal)</li>
    <li><strong>Embed</strong> — Embeds an external page in an iFrame (e.g., your company's status page)</li>
  </ul>
</li>
<li>Write or configure the page content</li>
<li>Click <strong>Save</strong></li>
</ol>

<h2>Adding a Custom Page to Navigation</h2>
<ol>
<li>After saving the page, go to <strong>Settings → Appearance → Portal Builder → Navigation Options</strong></li>
<li>Enable <strong>Show Custom Pages in Navigation</strong></li>
<li>Or drag the custom page into the navigation structure in the Portal Builder</li>
</ol>

<h2>Use Cases</h2>
<ul>
<li><strong>Contact Us page</strong> — A page with your support email, Calendly link, or embedded contact form</li>
<li><strong>Release Notes</strong> — A custom page listing product version releases (linked from the KB navigation)</li>
<li><strong>Contributing Guide</strong> — For open-source projects, a page explaining how to contribute to the documentation</li>
<li><strong>Changelog</strong> — A running log of documentation updates</li>
<li><strong>Status Page</strong> — A redirect to your Statuspage.io or Better Uptime page</li>
</ul>

<h2>SEO for Custom Pages</h2>
<p>Each custom page has its own SEO settings (title and description meta tags) accessible from the page's edit screen in the Inspector panel. Custom pages are included in your KB's sitemap.xml.</p>

<h2>Page Visibility</h2>
<p>Custom pages follow the same visibility rules as your KB:</p>
<ul>
<li>Public KB — Custom pages are publicly accessible</li>
<li>Private KB — Custom pages require reader login</li>
<li>Mixed — You can configure individual custom pages as public or private in the page settings</li>
</ul>