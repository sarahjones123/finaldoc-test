---
title: "Smart Article Linking (AI)"
description: "AI analyzes your article and suggests internal links to related content you can insert with one click."
slug: "smart-article-linking-ai"
status: "PUBLISHED"
createdAt: "2026-02-27T10:22:40.982Z"
updatedAt: "2026-03-19T15:48:11.342Z"
---

<h1>Smart Article Linking (AI)</h1>
<p>Smart Linking is an AI-powered feature that automatically identifies opportunities to link articles together. Instead of manually hunting for related content to cross-reference, the AI reads your article and suggests other articles in your knowledge base that are relevant — then inserts the links for you with one click.</p>

<h2>What Smart Linking Does</h2>
<p>When you run Smart Linking on an article:</p>
<ol>
<li>The AI analyzes your article's content — topics, terminology, concepts</li>
<li>It searches your entire knowledge base for articles that are semantically related</li>
<li>It identifies phrases in your article that could be turned into hyperlinks to those related articles</li>
<li>It presents suggestions: the phrase to link, and the target article</li>
<li>You choose which suggestions to accept and which to skip</li>
</ol>

<h2>How to Use Smart Linking</h2>
<ol>
<li>Open an article in the Documentation editor</li>
<li>Look for the <strong>Smart Link</strong> button in the editor toolbar or the Inspector panel (it may look like a chain link with a sparkle icon)</li>
<li>Click it to run the AI analysis</li>
<li>Wait a moment — the AI scans your content and finds related articles</li>
<li>A list of suggestions appears, each showing:
  <ul>
    <li>The exact phrase in your article that would become a link</li>
    <li>The article it would link to</li>
    <li>A confidence score or relevance indicator</li>
  </ul>
</li>
<li>Click <strong>Accept</strong> to insert a link, or <strong>Skip</strong> to ignore the suggestion</li>
<li>Accepted links are inserted into your article automatically</li>
</ol>

<h2>When to Use Smart Linking</h2>
<ul>
<li>After writing a new article — run Smart Linking to connect it to the rest of your KB</li>
<li>After adding content to an existing article — new text may relate to articles that have been added since the article was first written</li>
<li>During a content audit — run it on older articles to ensure they are well-connected</li>
</ul>

<h2>How Suggestions Are Generated</h2>
<p>Smart Linking uses semantic search (vector embeddings) to find related articles — not just keyword matching. This means it can find related content even when the words used are different. For example, an article about "user authentication" can be linked from text that talks about "logging in" or "account access" — the AI understands the conceptual connection.</p>

<h2>Reviewing and Editing Links</h2>
<p>Links inserted by Smart Linking are standard hyperlinks in your article. You can:</p>
<ul>
<li>Click the link and press <strong>Ctrl+K / Cmd+K</strong> to edit or remove it</li>
<li>Delete it like any other link if you decide you do not want it</li>
<li>Change the link destination if the AI suggested the wrong target</li>
</ul>

<h2>Requirements</h2>
<p>Smart Linking requires:</p>
<ul>
<li>An <strong>OpenAI API key</strong> configured in Settings → AI (Ved AI) → AI API Keys, or the default FinalDoc AI to be enabled</li>
<li>At least a few other published articles in your knowledge base (it cannot suggest links to articles that do not exist)</li>
<li>Articles to have content — it cannot analyze empty articles</li>
</ul>