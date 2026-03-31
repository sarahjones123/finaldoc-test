---
title: "API Documentation Overview"
description: "How to create and manage interactive API documentation in FinalDoc."
slug: "api-documentation-overview"
status: "PUBLISHED"
createdAt: "2026-02-23T18:13:43.033Z"
updatedAt: "2026-03-27T10:25:21.796Z"
---

<h1>API Documentation Overview</h1>
<p>The API Docs section of FinalDoc is where you manage interactive API reference documentation for your product. Upload your OpenAPI/Swagger specifications and FinalDoc automatically generates a beautiful, interactive API explorer that your developers can read, test, and copy code from — without any manual work.</p>

<h2>Opening API Docs</h2>
<p>Click <strong>API Docs</strong> (the code/terminal icon) in the left sidebar.</p>

<h2>What You Can Do</h2>
<ul>
<li><strong>Import OpenAPI specs</strong> — Upload your OpenAPI 3.0 (or Swagger 2.0) YAML or JSON specification file</li>
<li><strong>Auto-generated reference</strong> — FinalDoc parses your spec and generates a documented endpoint reference with request/response schemas, examples, and status codes</li>
<li><strong>Interactive API Explorer</strong> — Readers can make live API calls from within the documentation using the "Try it out" interface</li>
<li><strong>Multi-version support</strong> — Maintain separate API documentation for v1, v2, etc.</li>
<li><strong>Code examples</strong> — Auto-generated code snippets in multiple languages (curl, JavaScript, Python, PHP, Ruby, Go)</li>
</ul>

<h2>How to Add API Documentation</h2>
<ol>
<li>In the API Docs view, click <strong>+ Import Specification</strong></li>
<li>Choose your spec format (OpenAPI 3.0, Swagger 2.0)</li>
<li>Upload your YAML or JSON file, or paste the spec content directly</li>
<li>Click <strong>Import</strong></li>
<li>FinalDoc validates and processes the spec, then generates the documentation automatically</li>
<li>Review the generated documentation and publish it to make it visible on your public KB</li>
</ol>

<h2>The Interactive API Explorer</h2>
<p>On the public knowledge base, readers using the API Explorer can:</p>
<ul>
<li>Browse all endpoints organized by tag/group</li>
<li>Expand any endpoint to see parameters, request body schema, and response schemas</li>
<li>Enter their API key and other auth credentials</li>
<li>Fill in request parameters and send real API calls</li>
<li>See the actual response from your API</li>
<li>Copy auto-generated code snippets in their preferred programming language</li>
</ul>

<h2>API Documentation vs. Knowledge Base Articles</h2>
<p>Use <strong>API Docs</strong> for machine-readable, spec-driven reference documentation. Use regular <strong>Documentation</strong> articles for conceptual guides, tutorials, and getting started content that needs narrative explanation. Many teams use both — API reference in API Docs, and integration guides and tutorials in Documentation articles.</p>

<h2>Updating API Documentation</h2>
<p>When your API changes, re-import the updated spec:</p>
<ol>
<li>Go to the spec you want to update</li>
<li>Click <strong>Update Spec</strong></li>
<li>Upload or paste the new specification</li>
<li>FinalDoc merges the changes and updates the documentation</li>
</ol>

<h2>Publishing API Docs on Your Public KB</h2>
<p>After importing your OpenAPI spec and setting up endpoints, you need to <strong>link</strong> the API documentation version to your Knowledge Base version. This makes the API reference visible as an "API" tab on your public knowledge base.</p>
<p>See <a href="/article/linking-api-docs-to-knowledge-base"><strong>Linking API Docs to Your Knowledge Base</strong></a> for step-by-step instructions.</p>