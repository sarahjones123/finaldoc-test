---
title: "AI Configuration"
description: "Enabling and configuring Ved AI assistants."
slug: "ai-configuration"
status: "PUBLISHED"
createdAt: "2026-02-23T18:16:39.597Z"
updatedAt: "2026-03-25T18:41:21.312Z"
---

<h1>AI Configuration</h1>
<p>The AI Configuration page is your single control panel for all AI features in FinalDoc. Choose where your AI requests are processed and configure your provider.</p>

<h2>AI Provider</h2>
<p>Two options are available:</p>

<h3>FinalDoc AI (Default)</h3>
<p>Cloud-hosted, powered by OpenAI GPT-4o-mini. No setup needed — works out of the box with the best quality. Your content is processed securely and not used for AI training.</p>

<h3>Your Private Cloud</h3>
<p>Full privacy — all AI requests route through your own cloud infrastructure. Your data (articles, codebase, translations) never leaves your environment.</p>

<p>Supported providers:</p>
<table>
<thead><tr><th>Provider</th><th>Best For</th></tr></thead>
<tbody>
<tr><td><strong>Azure OpenAI</strong></td><td>Same GPT-4o quality, data stays in your Azure tenant. Recommended for enterprises already on Azure.</td></tr>
<tr><td><strong>AWS Bedrock</strong></td><td>Access Claude, Llama, and other models within your AWS account.</td></tr>
<tr><td><strong>Google Vertex AI</strong></td><td>Gemini models in your Google Cloud Platform.</td></tr>
<tr><td><strong>Custom Endpoint</strong></td><td>Any OpenAI-compatible API — vLLM, LiteLLM, FastChat, or your own server.</td></tr>
</tbody>
</table>

<h2>Setup Guide</h2>
<ol>
<li>Go to <strong>Settings &gt; AI (Ved AI) &gt; AI Configuration</strong></li>
<li>Select <strong>Your Private Cloud</strong></li>
<li>Choose your provider (e.g., Azure OpenAI)</li>
<li>Enter your endpoint URL and API key</li>
<li>Optionally specify a model name</li>
<li>Click <strong>Save</strong></li>
</ol>
<p>All AI features — Writer Assistant, Reader Chatbot, Design Assistant, Translation, Doc Autopilot — will immediately route through your private endpoint.</p>

<h2>Quality Note</h2>
<div style="background:#eff6ff;border-left:4px solid #3b82f6;padding:12px 16px;border-radius:4px;margin:16px 0">
  <strong>Quality depends on the model you choose.</strong> Azure OpenAI with GPT-4o gives identical quality to FinalDoc AI. Other models (Llama, Mistral) may produce different results depending on the model size and capabilities.
</div>

<h2>Need a Provider Not Listed?</h2>
<p>Raise a request and we will add support within 1 week. Contact <strong>support@finaldoc.io</strong>.</p>