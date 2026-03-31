---
title: "SEO Settings"
description: "Configuring meta tags, sitemap, and social sharing."
slug: "seo-settings"
status: "PUBLISHED"
createdAt: "2026-02-23T18:16:22.801Z"
updatedAt: "2026-03-12T09:35:36.460Z"
---

<h1>SEO Settings</h1>
<p>FinalDoc's SEO Settings let you configure site-wide SEO parameters for your public knowledge base — the title template, default meta description, and social sharing settings. These are the global defaults; individual articles can override them in their own SEO settings.</p>

<h2>Opening SEO Settings</h2>
<ol>
<li>Go to <strong>Settings → Domain &amp; SEO → SEO Settings</strong></li>
</ol>

<h2>Meta Title Template</h2>
<p>The HTML title tag format for article pages. Uses placeholders to dynamically build titles:</p>
<ul>
<li><code>{{article_title}}</code> — Replaced with the article's title</li>
<li><code>{{project_name}}</code> — Replaced with your KB name</li>
<li><code>{{category_name}}</code> — Replaced with the article's category</li>
</ul>

<p>Example templates:</p>
<ul>
<li><code>{{article_title}} | {{project_name}}</code> → "How to Reset Password | Acme Help Center"</li>
<li><code>{{article_title}} - {{project_name}} Docs</code> → "How to Reset Password - Acme Docs"</li>
<li><code>{{category_name}}: {{article_title}} | {{project_name}}</code> → "Account: How to Reset Password | Acme Help Center"</li>
</ul>

<h2>Default Meta Description</h2>
<p>Used for pages that don't have an individual meta description — mainly the KB homepage and category pages. Write a 130–160 character description of your knowledge base overall:</p>
<pre><code>Example: "Find answers to all your Acme Corp questions. Browse guides, tutorials, and API reference documentation for your account and integrations."</code></pre>

<h2>Open Graph Settings</h2>
<p>Open Graph (OG) tags control how your KB pages appear when shared on Twitter, LinkedIn, Slack, and other social platforms.</p>
<ul>
<li><strong>OG Site Name</strong> — Your company/product name (shown in social previews)</li>
<li><strong>Default OG Image</strong> — The image shown in social previews for pages without a Featured Image. Upload a 1200×630px image for best results across all platforms</li>
</ul>
<p>Individual articles use their <strong>Featured Image</strong> as the OG image. The Default OG Image is used for the KB homepage and any articles without a featured image.</p>

<h2>Sitemap</h2>
<p>FinalDoc automatically generates and maintains a sitemap at:</p>
<pre><code>https://yourproject.finaldoc.io/sitemap.xml</code></pre>
<p>Or with a custom domain:</p>
<pre><code>https://docs.yourcompany.com/sitemap.xml</code></pre>
<p>Submit this to Google Search Console and Bing Webmaster Tools. FinalDoc updates the sitemap within minutes when articles are published, updated, or deleted.</p>

<h2>Robots.txt</h2>
<p>FinalDoc generates a standard robots.txt that allows all crawlers. If your KB is private (requires reader login), the robots.txt automatically disallows crawlers from restricted pages — no configuration needed.</p>

<h2>noindex for Draft/Archived Articles</h2>
<p>Draft and archived articles always include <code>noindex</code> meta tags — they're never indexed by search engines even if somehow accessible. Published articles are always indexed.</p>