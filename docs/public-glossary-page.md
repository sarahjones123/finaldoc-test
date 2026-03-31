---
title: "Public Glossary Page"
description: ""
slug: "public-glossary-page"
status: "PUBLISHED"
createdAt: "2026-02-24T08:32:54.735Z"
updatedAt: "2026-03-12T10:07:59.024Z"
---

<h1>Public Glossary Page</h1>
<p>FinalDoc automatically generates a public Glossary page on your knowledge base. This page lists all the terms you have defined in the Toolbox → Term Glossary, organized alphabetically, so readers can quickly look up terminology without searching through articles. It's particularly useful for technical products, industry-specific platforms, or any product with its own vocabulary.</p>

<h2>How the Glossary Page Works</h2>
<p>The Glossary page is generated automatically from your term definitions — you do not need to create it manually. Every term you add to the Term Glossary appears on the public page. Terms are sorted alphabetically and grouped by first letter (A, B, C, etc.).</p>

<h2>The Glossary Page URL</h2>
<p>Your Glossary page is always at:</p>
<ul>
<li>FinalDoc subdomain: <code>https://yourproject.finaldoc.io/glossary</code></li>
<li>Custom domain: <code>https://docs.yourcompany.com/glossary</code></li>
</ul>
<p>The URL is the same regardless of how you've organized your categories or articles.</p>

<h2>Adding Terms to the Glossary</h2>
<ol>
<li>Go to <strong>Toolbox</strong> in the left sidebar</li>
<li>Click <strong>Term Glossary</strong> (under Content Blocks)</li>
<li>Click <strong>+ New Term</strong></li>
<li>Enter the <strong>Term</strong> (the word or phrase)</li>
<li>Enter the <strong>Definition</strong> (the plain-language explanation)</li>
<li>Optionally add <strong>Aliases</strong> (alternative names for the same term — e.g., "KB" as an alias for "Knowledge Base")</li>
<li>Click <strong>Save</strong></li>
</ol>
<p>The term immediately appears on the public Glossary page.</p>

<h2>Inline Glossary Tooltips in Articles</h2>
<p>Terms you define in the Glossary are automatically underlined with a dotted line in article text when a reader encounters them. The reader hovers over the underlined term to see the definition in a tooltip — without leaving the page. This is called inline glossary enrichment. It works automatically as long as the term appears exactly (case-insensitive) in the article body.</p>

<h2>Adding the Glossary to Navigation</h2>
<p>You can add a link to the Glossary in your KB header or footer navigation:</p>
<ol>
<li>Go to <strong>Settings → Appearance → Portal Builder</strong></li>
<li>Go to the <strong>Header</strong> section</li>
<li>Click <strong>Add Navigation Link</strong></li>
<li>Set the label to "Glossary" and the URL to <code>/glossary</code></li>
<li>Click <strong>Save</strong></li>
</ol>

<h2>Showing/Hiding the Glossary</h2>
<p>The public glossary page is always generated automatically when you have terms defined. If you have no terms defined in the Term Glossary, the page still exists but is empty. You can also add a link to it anywhere in your KB content by using the URL <code>/glossary</code> as a relative link in any article.</p>

<h2>Managing Terms</h2>
<ul>
<li><strong>Edit a term</strong>: Click the pencil icon next to any term in the Term Glossary to update the definition</li>
<li><strong>Delete a term</strong>: Click the trash icon — the term is removed from the glossary page immediately</li>
<li><strong>Search terms</strong>: Use the search box in the Term Glossary to find a specific term by name</li>
</ul>

<h2>Use Cases</h2>
<ul>
<li>Technical products with acronyms and jargon</li>
<li>Legal or compliance documentation with defined terms</li>
<li>Industry-specific platforms where readers may not know the terminology</li>
<li>Internal wikis where company-specific terms need standardized definitions</li>
</ul>