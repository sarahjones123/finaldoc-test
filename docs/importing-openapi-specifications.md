---
title: "Importing OpenAPI Specifications"
description: "Import OpenAPI/Swagger specs to auto-generate interactive API documentation."
slug: "importing-openapi-specifications"
status: "PUBLISHED"
createdAt: "2026-02-24T03:51:11.835Z"
updatedAt: "2026-03-19T14:58:26.864Z"
---

<h1>Importing OpenAPI Specifications</h1>
<p>FinalDoc generates your API reference documentation automatically from an OpenAPI (formerly Swagger) specification file. You write the spec in YAML or JSON, and FinalDoc turns it into a beautiful, interactive reference — no manual page creation required.</p>

<h2>Supported Specification Formats</h2>
<ul>
<li><strong>OpenAPI 3.0.x</strong> (recommended) — Modern standard, supports more features</li>
<li><strong>Swagger 2.0</strong> — Legacy format, still supported</li>
<li>Both YAML and JSON are accepted</li>
</ul>

<h2>How to Import</h2>
<ol>
<li>Go to <strong>API Docs</strong> in the left sidebar</li>
<li>Click <strong>+ Import Specification</strong></li>
<li>Choose how to provide the spec:
  <ul>
    <li><strong>Upload file</strong> — Select a .yaml, .yml, or .json file from your computer</li>
    <li><strong>Paste content</strong> — Copy/paste the spec text directly into the text field</li>
    <li><strong>Import from URL</strong> — Provide a URL to your spec (e.g., <code>https://api.yourcompany.com/openapi.json</code>)</li>
  </ul>
</li>
<li>Click <strong>Import</strong></li>
<li>FinalDoc validates the spec — if there are errors (invalid YAML, missing required fields), they appear listed with line numbers</li>
<li>If valid, the spec is processed and your API reference is generated</li>
</ol>

<h2>What FinalDoc Generates from Your Spec</h2>
<ul>
<li>Endpoint list, grouped by tag</li>
<li>Request parameters table (path, query, header, cookie params)</li>
<li>Request body schema with example</li>
<li>Response schema for each status code</li>
<li>Authentication description from the securitySchemes section</li>
<li>Code examples in 6 languages</li>
</ul>

<h2>Enriching the Generated Docs</h2>
<p>The quality of the generated documentation depends entirely on your spec. To get the best results:</p>
<ul>
<li>Write <code>description</code> fields for every endpoint, parameter, and schema property</li>
<li>Include <code>example</code> values for all request/response fields</li>
<li>Use <code>tags</code> to group related endpoints</li>
<li>Define <code>servers</code> with your actual base URL</li>
<li>Use <code>$ref</code> for shared schemas to avoid repetition and keep the spec DRY</li>
</ul>

<h2>Spec Validation Errors</h2>
<p>Common errors when importing:</p>
<ul>
<li><strong>Invalid YAML</strong> — YAML is indentation-sensitive. Use a YAML linter to check before importing</li>
<li><strong>Missing required fields</strong> — OpenAPI requires <code>openapi</code> version, <code>info.title</code>, and <code>paths</code> at minimum</li>
<li><strong>Unresolved $ref</strong> — A schema reference points to something that doesn't exist in the spec</li>
</ul>

<h2>Auto-Sync from URL</h2>
<p>If you imported from a URL, FinalDoc can periodically re-fetch and update the spec automatically. Enable <strong>Auto-sync</strong> in the spec settings and set the sync frequency (daily, weekly). This keeps your API docs always in sync with your latest spec without manual imports.</p>