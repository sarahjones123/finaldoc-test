---
title: "KB SEO & Custom Domain"
description: "Optimize your knowledge base for search engines and set up a custom domain."
slug: "kb-seo-custom-domain"
status: "PUBLISHED"
createdAt: "2026-02-24T03:51:10.307Z"
updatedAt: "2026-03-17T04:42:46.380Z"
---

<h1>KB SEO and Custom Domain</h1>
<p>A well-optimized knowledge base attracts organic search traffic — readers find your help articles through Google and Bing instead of having to know your URL. This guide covers SEO best practices for FinalDoc and how to configure a custom domain for your KB.</p>

<h2>SEO Settings</h2>
<h3>Opening SEO Settings</h3>
<ol>
<li>Go to <strong>Settings → Domain &amp; SEO → SEO Settings</strong></li>
</ol>

<h3>Meta Title Template</h3>
<p>The HTML title that appears in browser tabs and search results for your KB pages. Configure a template like:</p>
<pre><code>[Article Title] - [Project Name] Help Center</code></pre>
<p>This creates titles like "How to Reset Password - Acme Corp Help Center" — which is more descriptive than just the article title alone.</p>

<h3>Default Meta Description</h3>
<p>Used for pages that do not have an article description (like the KB homepage). Write a 130–160 character description of your knowledge base.</p>

<h3>Sitemap</h3>
<p>FinalDoc automatically generates a sitemap.xml at <code>https://yourproject.finaldoc.io/sitemap.xml</code>. This file lists all your published articles and categories, helping search engines find and index all your content. Submit this URL to Google Search Console and Bing Webmaster Tools.</p>

<h3>Robots.txt</h3>
<p>FinalDoc generates a standard robots.txt that allows all search engines to crawl all published content. If your KB is private (requires reader login), the robots.txt disallows crawling of restricted pages.</p>

<h3>Canonical URLs</h3>
<p>FinalDoc adds canonical tags to all article pages to prevent duplicate content issues when your KB is accessible via both the FinalDoc subdomain and your custom domain.</p>

<h2>Custom Domain</h2>
<p>See the dedicated <strong>Custom Domain</strong> article for full setup instructions. In brief:</p>
<ol>
<li>Settings → Domain &amp; SEO → Custom Domain</li>
<li>Add your domain (e.g., docs.yourcompany.com)</li>
<li>Add a TXT verification record to your DNS</li>
<li>After verification, add a CNAME pointing to app.finaldoc.io</li>
<li>Activate — SSL is provisioned automatically</li>
</ol>

<h2>Article-Level SEO</h2>
<p>Each article has its own SEO settings in the Inspector panel:</p>
<ul>
<li><strong>Description</strong> — The meta description for this specific article. If empty, uses the project default</li>
<li><strong>Slug</strong> — The URL path (e.g., /how-to-reset-password). Keep it short, lowercase, and keyword-rich</li>
<li><strong>Featured Image</strong> — Used as the Open Graph image when the article is shared on social media</li>
</ul>

<h2>SEO Best Practices for Knowledge Bases</h2>
<ul>
<li><strong>Write descriptive titles</strong> — "Password Reset" is weak. "How to Reset Your Account Password" is better</li>
<li><strong>Fill in every description</strong> — Empty descriptions harm click-through rates from search results</li>
<li><strong>Use H2/H3 headings</strong> — Structured content ranks better and enables rich results</li>
<li><strong>Update stale content</strong> — Fresh content ranks better than old content</li>
<li><strong>Internal linking</strong> — Link between related articles using Smart Linking</li>
<li><strong>Image alt text</strong> — Always fill in alt text on images</li>
</ul>