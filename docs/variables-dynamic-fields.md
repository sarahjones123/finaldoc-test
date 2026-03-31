---
title: "Variables (Dynamic Fields)"
description: "Using dynamic variables that auto-update across all articles."
slug: "variables-dynamic-fields"
status: "PUBLISHED"
createdAt: "2026-02-23T18:13:43.228Z"
updatedAt: "2026-03-21T03:42:32.517Z"
---

<h1>Variables (Dynamic Fields)</h1>
<p>Variables (also called Dynamic Fields) are reusable placeholders that you define once and use across many articles. When the value changes, you update it in one place and it updates everywhere it is used automatically — no need to find and replace across articles manually.</p>

<h2>When to Use Variables</h2>
<ul>
<li><strong>Product name</strong> — If your product name changes, update one variable instead of editing hundreds of articles</li>
<li><strong>Version numbers</strong> — Keep documentation current: "This guide covers {{product}} version {{version}}"</li>
<li><strong>Pricing</strong> — "Plans start at {{starter_price}}/month"</li>
<li><strong>Support contact</strong> — "Contact us at {{support_email}}"</li>
<li><strong>URLs</strong> — "Visit {{dashboard_url}} to get started"</li>
</ul>

<h2>Creating a Variable</h2>
<ol>
<li>Go to <strong>Toolbox</strong> in the left sidebar</li>
<li>Under <strong>Content Blocks</strong>, click <strong>Dynamic Fields</strong></li>
<li>Click <strong>+ New Variable</strong></li>
<li>Enter the <strong>variable name</strong> (no spaces — use underscores or camelCase, e.g., <code>product_name</code> or <code>supportEmail</code>)</li>
<li>Enter the <strong>value</strong> — the actual text readers will see (e.g., "FinalDoc Pro" or "support@yourcompany.com")</li>
<li>Click <strong>Save</strong></li>
</ol>

<h2>Using a Variable in an Article</h2>
<p>To insert a variable reference into an article:</p>
<ol>
<li>Open the article in the editor</li>
<li>Place your cursor where the value should appear</li>
<li>Click the <strong>Variables</strong> button in the editor toolbar</li>
<li>Select the variable from the dropdown</li>
<li>The variable is inserted as <code>{{variable_name}}</code> in the editor view</li>
</ol>
<p>In the editor, you will see the variable name as a tag. On the public knowledge base, readers see the actual value — the variable is replaced with its current value when the page is rendered.</p>

<h2>Updating a Variable</h2>
<ol>
<li>Go to <strong>Toolbox → Dynamic Fields</strong></li>
<li>Find the variable and click to edit it</li>
<li>Change the value</li>
<li>Click <strong>Save</strong></li>
<li>All articles using this variable immediately show the new value to readers</li>
</ol>

<h2>Variable Types</h2>
<p>Variables support different content types:</p>
<ul>
<li><strong>Text</strong> — Plain text values (names, email addresses, short phrases)</li>
<li><strong>URL</strong> — Links that can be inserted as clickable hyperlinks</li>
<li><strong>Number</strong> — Numeric values (version numbers, prices)</li>
</ul>