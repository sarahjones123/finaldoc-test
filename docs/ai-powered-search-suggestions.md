---
title: "AI-Powered Search Suggestions"
description: "When standard search returns no results, AI semantic search suggests related articles."
slug: "ai-powered-search-suggestions"
status: "PUBLISHED"
createdAt: "2026-02-27T10:22:40.973Z"
updatedAt: "2026-03-21T03:04:45.997Z"
---

<h1>AI-Powered Search Suggestions</h1>
<p>When a reader searches your knowledge base and gets zero results, FinalDoc's AI steps in. Instead of showing an empty "No results" page, it uses semantic AI search to find articles that are conceptually related to the search query — even if the exact words do not appear in any article — and shows them as suggestions.</p>

<h2>How It Works</h2>
<ol>
<li>Reader types a search query</li>
<li>FinalDoc runs the standard search (keyword, full-text, fuzzy)</li>
<li>If zero results are returned, FinalDoc automatically runs a <strong>semantic search</strong> using vector embeddings</li>
<li>The semantic search finds articles that are about the same topic, even with different words</li>
<li>Results appear with a label like "You might be looking for..." or "Related articles:"</li>
</ol>

<h2>Example</h2>
<p>If a reader searches "how to get my password back" and your article is titled "Account Recovery Guide" — the exact words do not match, but the meaning does. The AI finds the article and shows it as a suggestion.</p>

<h2>When It Activates</h2>
<p>AI search suggestions activate automatically when:</p>
<ul>
<li>The standard search returns zero results</li>
<li>AI embeddings have been generated for your articles (see below)</li>
</ul>

<h2>Chatbot Integration</h2>
<p>The AI search also integrates with the Ved AI chatbot. When the chatbot observes a reader searching for something, it shows a "Looking for [query]? Ask me!" prompt on the chat bubble. The reader can click it to instantly send the query to the AI for a more detailed answer.</p>

<h2>Requirements</h2>
<p>For AI search to work, your articles need to be <strong>embedded</strong>:</p>
<ol>
<li>Go to <strong>Settings → AI (Ved AI) → AI Training &amp; Knowledge Management</strong></li>
<li>Click <strong>Embed All Articles</strong></li>
<li>Wait for the process to complete</li>
</ol>
<p>Once embedded, semantic search is available across all published articles. New and updated articles are re-embedded automatically.</p>

<h2>Improving Search Results</h2>
<ul>
<li>Write descriptive article titles and descriptions — they are the most important signals for search relevance</li>
<li>Use the same language your readers use — if readers say "sign in" but your articles say "authenticate", both terms should appear in your content</li>
<li>Ensure articles are well-structured with clear headings — helps both keyword and semantic search</li>
</ul>