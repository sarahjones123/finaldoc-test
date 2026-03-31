---
title: "AI Compliance & Data Handling"
description: "Configure data retention, PII detection, and compliance policies for AI features."
slug: "ai-compliance-data-handling"
status: "PUBLISHED"
createdAt: "2026-02-24T08:32:54.631Z"
updatedAt: "2026-03-12T09:15:11.998Z"
---

<h1>AI Compliance &amp; Data Handling</h1>
<p>This article explains how FinalDoc handles your content when it's sent to AI services — what data goes where, how it's stored, and what controls you have. Important reading if you're in a regulated industry (healthcare, finance, legal) or have strict data governance requirements.</p>

<h2>What Data Is Sent to AI Services</h2>
<p>When AI features are used, FinalDoc sends content to OpenAI's API:</p>
<table>
<thead><tr><th>Feature</th><th>Data Sent</th></tr></thead>
<tbody>
<tr><td><strong>Writer AI (Improve, Expand, etc.)</strong></td><td>The article content (or selected text) being edited</td></tr>
<tr><td><strong>Chatbot</strong></td><td>The reader's question + relevant article content retrieved from your KB</td></tr>
<tr><td><strong>AI Optimizer</strong></td><td>The article being analyzed</td></tr>
<tr><td><strong>Translation</strong></td><td>The article title, description, and content</td></tr>
<tr><td><strong>Embeddings</strong></td><td>Article content (sent to generate vector embeddings)</td></tr>
</tbody>
</table>

<h2>OpenAI Data Processing</h2>
<p>FinalDoc uses the OpenAI API under a data processing agreement. Key points:</p>
<ul>
<li><strong>OpenAI does NOT use API data to train its models</strong> — API data is separate from ChatGPT training data</li>
<li>Requests are retained by OpenAI for up to 30 days for abuse monitoring, then deleted</li>
<li>If you use your own API key (BYOK), OpenAI's data handling policies apply directly to your account</li>
</ul>

<h2>FinalDoc Data Storage</h2>
<ul>
<li>AI-generated content (article text, chatbot responses) is stored in your FinalDoc database when saved</li>
<li>Embeddings (vector representations of your articles) are stored in PostgreSQL with pgvector — on FinalDoc's own server</li>
<li>Chatbot conversation history is stored in the database (if conversation logging is enabled)</li>
</ul>

<h2>Disabling AI Features</h2>
<p>If you need to ensure no article content leaves FinalDoc's servers:</p>
<ol>
<li>Go to <strong>Settings → AI (Ved AI) → AI Configuration</strong></li>
<li>Set <strong>AI Features</strong> to <strong>Disabled</strong></li>
</ol>
<p>This disables all AI-powered features across your project — writer assistant, chatbot, optimizer, translation, and embeddings. Your KB continues to work normally with standard keyword search.</p>

<h2>GDPR / Privacy</h2>
<p>FinalDoc is hosted in the EU-compatible infrastructure. When you submit a GDPR data deletion request:</p>
<ul>
<li>FinalDoc deletes all stored reader data, including chatbot conversation history</li>
<li>OpenAI data retention (30 days max) is governed by OpenAI's GDPR agreements</li>
</ul>

<h2>Questions</h2>
<p>For compliance documentation, DPA (Data Processing Agreement) requests, or security questionnaires, contact <strong>support@finaldoc.io</strong>.</p>