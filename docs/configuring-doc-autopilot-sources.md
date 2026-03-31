---
title: "Configuring Doc Autopilot Sources"
description: ""
slug: "configuring-doc-autopilot-sources"
status: "PUBLISHED"
createdAt: "2026-02-24T18:29:42.079Z"
updatedAt: "2026-03-27T13:11:31.265Z"
---

<h1>Configuring Doc Autopilot Sources</h1>
<p>A "source" in Doc Autopilot is a code repository that you want to generate documentation from. Each source connects to a GitHub, GitLab, or Bitbucket repository and specifies which branch and folder to analyze.</p>

<h2>Adding a Source</h2>
<ol>
<li>Click <strong>Doc Autopilot</strong> in the left sidebar (under AI Studio)</li>
<li>In the sidebar, expand <strong>Configuration</strong> → click <strong>Sources</strong></li>
<li>Click <strong>Add Source</strong></li>
<li>Fill in the source details (see below)</li>
<li>Click <strong>Save</strong></li>
</ol>

<h2>Source Fields</h2>
<table>
<thead><tr><th>Field</th><th>Required</th><th>Description</th></tr></thead>
<tbody>
<tr><td><strong>Name</strong></td><td>Yes</td><td>A descriptive name for this source (e.g., "Backend API", "Frontend App")</td></tr>
<tr><td><strong>Repository URL</strong></td><td>Yes</td><td>Full URL to the repository. Supports:<br/>
• GitHub: <code>https://github.com/owner/repo</code><br/>
• GitLab: <code>https://gitlab.com/group/repo</code> (or self-hosted)<br/>
• Bitbucket: <code>https://bitbucket.org/owner/repo</code></td></tr>
<tr><td><strong>Branch</strong></td><td>No</td><td>Branch to analyze (default: <code>main</code>)</td></tr>
<tr><td><strong>Path</strong></td><td>No</td><td>Subfolder to analyze (e.g., <code>src</code>, <code>backend</code>). Leave empty for the entire repo</td></tr>
<tr><td><strong>Access Token</strong></td><td>For private repos</td><td>Authentication token for private repositories:<br/>
• <strong>GitHub</strong>: Personal Access Token (<code>ghp_...</code>) with <code>repo</code> scope<br/>
• <strong>GitLab</strong>: Personal Access Token (<code>glpat-...</code>) with <code>read_repository</code> scope<br/>
• <strong>Bitbucket</strong>: App Password with <code>repository read</code> permission<br/>
Public repos don't need a token.</td></tr>
<tr><td><strong>App URL</strong></td><td>No</td><td>Live application URL for screen capture (e.g., <code>https://app.example.com</code>). Used to generate UI guide screenshots.</td></tr>
<tr><td><strong>Doc Types</strong></td><td>Yes</td><td>Which types of documentation to generate: Getting Started, User Guide, API Reference, Feature Docs, UI Guides, Troubleshooting</td></tr>
</tbody>
</table>

<h2>Generating Documentation</h2>
<p>After adding a source:</p>
<ol>
<li>Click the source name to select it</li>
<li>Click <strong>Generate</strong> (or the play button)</li>
<li>Doc Autopilot will:
  <ul>
  <li>Fetch the file tree from your repository</li>
  <li>Download and analyze relevant source files</li>
  <li>Detect the framework, API endpoints, UI pages, and tech stack</li>
  <li>Generate draft articles using AI</li>
  </ul>
</li>
<li>Review generated docs under <strong>Generation → Generated Docs</strong></li>
<li>Click <strong>Accept</strong> on each article to publish it to your knowledge base, or edit it first</li>
</ol>

<h2>Testing a Source</h2>
<p>Before generating, you can test the connection:</p>
<ol>
<li>Select the source</li>
<li>Click <strong>Test Connection</strong></li>
<li>Doc Autopilot will try to fetch the file tree — if it succeeds, you'll see the file count. If it fails, you'll see the specific error (wrong token, repo not found, branch missing, etc.)</li>
</ol>

<h2>Multiple Sources</h2>
<p>You can add multiple sources per project — for example, one for your backend repo and another for your frontend repo. Each source generates documentation independently. Generated articles from different sources all go into the same knowledge base.</p>

<h2>Re-generating After Code Changes</h2>
<p>When your code changes, you can re-run Doc Autopilot on the same source. It will analyze the updated code and generate new or updated drafts. Existing accepted articles are not overwritten — new generated items appear as separate drafts that you can compare with the current version.</p>

<div style="background:#eff6ff;border-left:4px solid #3b82f6;padding:12px 16px;border-radius:4px;margin:16px 0">
  <strong>Tip:</strong> If you just want to sync existing markdown files (not generate new docs from code), use <strong>Code Repositories</strong> in Settings → Integrations instead. See <a href="/article/extensions">Extensions</a> for setup instructions.
</div>

<div style="background:#f0fdfa;border-left:4px solid #14b8a6;padding:12px 16px;border-radius:4px;margin:16px 0">
  <strong>Privacy:</strong> If your code is sensitive, configure a private AI provider at <strong>Settings → AI → <a href="/article/ai-configuration">AI Configuration</a></strong> so your source code is processed entirely within your own cloud infrastructure.
</div>