---
title: "Doc Autopilot Overview"
description: "Automatically generate documentation from code, APIs, and data sources."
slug: "doc-autopilot-overview"
status: "PUBLISHED"
createdAt: "2026-02-23T18:13:43.620Z"
updatedAt: "2026-03-27T13:11:31.258Z"
---

<h1>Doc Autopilot Overview</h1>
<p>Doc Autopilot automatically generates documentation by analyzing your codebase, application screens, and repository structure. Point it at a GitHub, GitLab, or Bitbucket repository and it produces complete articles — Getting Started guides, API References, Feature Docs, UI Guides, and Troubleshooting pages — all written by AI based on your actual code.</p>

<div style="background:#eff6ff;border-left:4px solid #3b82f6;padding:12px 16px;border-radius:4px;margin:16px 0">
  <strong>Doc Autopilot vs Code Repositories — what's the difference?</strong><br/>
  <strong>Code Repositories</strong> (Settings → Integrations → Code Repositories) syncs <em>existing markdown files</em> between your repo and FinalDoc. It's a file transfer tool — no AI involved.<br/><br/>
  <strong>Doc Autopilot</strong> (sidebar → AI Studio → Doc Autopilot) <em>reads your source code</em> and generates brand-new documentation using AI. It creates articles that didn't exist before.
</div>

<table>
<thead><tr><th>Feature</th><th>Code Repositories</th><th>Doc Autopilot</th></tr></thead>
<tbody>
<tr><td><strong>What it reads</strong></td><td>Markdown files (<code>.md</code>)</td><td>Source code (JS, Python, Go, etc.)</td></tr>
<tr><td><strong>What it produces</strong></td><td>Imports/exports articles as-is</td><td>AI-generated documentation articles</td></tr>
<tr><td><strong>AI involved?</strong></td><td>No</td><td>Yes — analyzes code structure, APIs, UI</td></tr>
<tr><td><strong>Use case</strong></td><td>Docs-as-code workflow, keep repo and KB in sync</td><td>Bootstrap docs for a new project, auto-document code changes</td></tr>
<tr><td><strong>Where to find it</strong></td><td>Settings → Integrations → Code Repositories</td><td>Sidebar → AI Studio → Doc Autopilot</td></tr>
</tbody>
</table>

<h2>How Doc Autopilot Works</h2>
<ol>
<li><strong>Add a Source</strong> — Connect your GitHub, GitLab, or Bitbucket repository</li>
<li><strong>AI Analyzes</strong> — Doc Autopilot scans your code, detects the framework, finds API endpoints, maps UI pages, reads README and changelog</li>
<li><strong>Generates Docs</strong> — AI creates draft articles based on the analysis: Getting Started, API Reference, Feature Docs, UI Guides, Troubleshooting</li>
<li><strong>Review &amp; Publish</strong> — Review the generated drafts, edit as needed, then publish to your knowledge base</li>
</ol>

<h2>Supported Platforms</h2>
<table>
<thead><tr><th>Platform</th><th>URL Format</th><th>Token Type</th></tr></thead>
<tbody>
<tr><td><strong>GitHub</strong></td><td><code>https://github.com/owner/repo</code></td><td>Personal Access Token with <code>repo</code> scope</td></tr>
<tr><td><strong>GitLab</strong></td><td><code>https://gitlab.com/group/repo</code> or self-hosted URL</td><td>Personal Access Token with <code>read_repository</code> scope</td></tr>
<tr><td><strong>Bitbucket</strong></td><td><code>https://bitbucket.org/owner/repo</code></td><td>App Password with <code>repository read</code> permission</td></tr>
</tbody>
</table>
<p>Public repositories don't require a token. Private repositories need the appropriate access token.</p>

<h2>What Doc Autopilot Detects</h2>
<ul>
<li><strong>Framework</strong> — React, Next.js, Express, Django, Flask, FastAPI, Rails, Spring Boot, and more</li>
<li><strong>API endpoints</strong> — REST routes, GraphQL schemas, OpenAPI specs</li>
<li><strong>UI pages</strong> — React components, Vue pages, route definitions</li>
<li><strong>Tech stack</strong> — Languages, databases, ORMs, cloud services</li>
<li><strong>README &amp; changelog</strong> — Existing documentation and version history</li>
</ul>

<h2>Doc Types Generated</h2>
<ul>
<li><strong>Getting Started</strong> — Installation, setup, and first steps</li>
<li><strong>User Guide</strong> — Feature walkthroughs and how-tos</li>
<li><strong>API Reference</strong> — Endpoint documentation with parameters and responses</li>
<li><strong>Feature Docs</strong> — Individual feature explanations</li>
<li><strong>UI Guides</strong> — Screen-by-screen walkthroughs (with optional app screenshots)</li>
<li><strong>Troubleshooting</strong> — Common issues and solutions</li>
</ul>

<h2>Opening Doc Autopilot</h2>
<h2>Private AI for Sensitive Codebases</h2>
<div style="background:#f0fdfa;border-left:4px solid #14b8a6;padding:12px 16px;border-radius:4px;margin:16px 0">
  <strong>Your code stays private.</strong> If your codebase contains proprietary or sensitive code, you can route all AI processing through your own private cloud infrastructure — Azure OpenAI, AWS Bedrock, Google Vertex AI, or any OpenAI-compatible endpoint. Your source code never leaves your environment.
</div>
<p>To configure a private AI provider:</p>
<ol>
<li>Go to <strong>Settings → AI (Ved AI) → <a href="/article/ai-configuration">AI Configuration</a></strong></li>
<li>Select <strong>Your Private Cloud</strong></li>
<li>Choose your provider and enter your endpoint URL and API key</li>
<li>Click <strong>Save</strong></li>
</ol>
<p>All Doc Autopilot AI requests — code analysis, article generation, and product profiling — will route through your private endpoint. Quality depends on the model you choose; Azure OpenAI with GPT-4o gives identical quality to FinalDoc AI.</p>

<h2>Opening Doc Autopilot</h2>
<p>Click <strong>Doc Autopilot</strong> in the left sidebar under the <strong>AI Studio</strong> section. See <a href="/article/configuring-doc-autopilot-sources">Configuring Doc Autopilot Sources</a> for step-by-step setup.</p>