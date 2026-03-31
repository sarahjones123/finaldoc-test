---
title: "Linking API Docs to Your Knowledge Base"
description: ""
slug: "linking-api-docs-to-knowledge-base"
status: "PUBLISHED"
createdAt: "2026-03-27T10:25:21.768Z"
updatedAt: "2026-03-27T10:29:46.753Z"
---

<h1>Linking API Docs to Your Knowledge Base</h1>
<p>After importing an OpenAPI spec, your API documentation lives as a separate version in FinalDoc. To make it visible on your public knowledge base, you need to <strong>link</strong> the API documentation version to your KB version. Once linked, an <strong>API</strong> tab appears in your public KB header, giving readers access to your interactive API reference alongside your regular documentation.</p>

<h2>Prerequisites</h2>
<ul>
<li>You have at least one <strong>Knowledge Base version</strong> (e.g., v1.0) with published articles</li>
<li>You have at least one <strong>API documentation version</strong> created by importing an OpenAPI/Swagger spec</li>
<li>The API documentation version is set to <strong>Published</strong> and <strong>Public</strong> visibility</li>
</ul>

<h2>Step-by-Step: Link API Docs to KB</h2>

<h3>1. Open Knowledge Bases Settings</h3>
<ol>
<li>Click <strong>Settings</strong> in the left sidebar</li>
<li>Under <strong>General</strong>, click <strong>Knowledge Bases</strong></li>
</ol>
<p>You'll see two sections: <strong>Knowledge base</strong> (your regular docs) and <strong>API documentation</strong> (your imported specs).</p>

<h3>2. Open Your KB Version</h3>
<ol>
<li>Find your KB version (e.g., <strong>v1.0</strong>) under the "Knowledge base" section</li>
<li>Click the <strong>three-dot menu</strong> (⋮) on the version card</li>
<li>Select <strong>Edit</strong> to open the version settings</li>
</ol>

<h3>3. Link the API Documentation</h3>
<ol>
<li>In the version settings, look for the <strong>Linked API Documentation</strong> dropdown</li>
<li>Select the API documentation version you want to link (e.g., "Beta — E-commerce API")</li>
<li>Click <strong>Save</strong></li>
</ol>

<h3>4. Verify on Your Public KB</h3>
<ol>
<li>Click <strong>View Site</strong> in the top navigation bar</li>
<li>Your public KB should now show an <strong>API</strong> tab in the header (next to "Docs")</li>
<li>Click the <strong>API</strong> tab to see your interactive API reference with all endpoints, request/response schemas, and code examples</li>
</ol>

<h2>What Readers See</h2>
<p>Once linked, your public KB displays:</p>
<ul>
<li><strong>Docs tab</strong> — Your regular knowledge base articles and categories</li>
<li><strong>API tab</strong> — Interactive API reference with endpoints grouped by resource, request builders, and code examples in 6 languages (cURL, JavaScript, Python, PHP, Ruby, Go)</li>
</ul>
<p>Readers can switch between tabs seamlessly. The API tab shows the same interactive explorer available in the admin panel, including the "Try It" feature if configured.</p>

<h2>Requirements for the API Tab to Appear</h2>
<p>The API tab will only appear on the public KB when <strong>all</strong> of these conditions are met:</p>
<table>
<thead><tr><th>Condition</th><th>Where to Check</th></tr></thead>
<tbody>
<tr><td>KB version is linked to an API doc version</td><td>Settings → Knowledge Bases → Edit KB version → Linked API Documentation</td></tr>
<tr><td>API doc version status is <strong>Published</strong></td><td>Settings → Knowledge Bases → API documentation section</td></tr>
<tr><td>API doc version visibility is <strong>Public</strong></td><td>Settings → Knowledge Bases → API documentation section</td></tr>
</tbody>
</table>

<h2>Unlinking API Docs</h2>
<p>To remove the API tab from your public KB:</p>
<ol>
<li>Go to <strong>Settings → Knowledge Bases</strong></li>
<li>Edit your KB version</li>
<li>Set <strong>Linked API Documentation</strong> to "None"</li>
<li>Click <strong>Save</strong></li>
</ol>
<p>The API tab will disappear from the public KB immediately.</p>

<h2>Multiple Versions</h2>
<p>Each KB version can link to a different API documentation version. This is useful when you have multiple API versions (e.g., v1 and v2) and want to show the correct API reference alongside the matching documentation version.</p>

<h2>Troubleshooting</h2>

<h3>API tab doesn't appear on public KB</h3>
<ul>
<li>Verify the API doc version is <strong>Published</strong> (not Draft)</li>
<li>Verify the API doc version visibility is <strong>Public</strong> (not Private)</li>
<li>Verify the KB version has the API doc version selected in <strong>Linked API Documentation</strong></li>
<li>Try refreshing the public KB page (Ctrl+Shift+R)</li>
</ul>

<h3>API tab shows "No endpoints"</h3>
<ul>
<li>Check that your OpenAPI spec was imported correctly — go to <strong>API Docs</strong> in the sidebar and verify endpoints are listed</li>
<li>Ensure at least one endpoint exists in the linked API documentation version</li>
</ul>