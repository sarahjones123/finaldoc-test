---
title: "AI Training & Knowledge Management"
description: ""
slug: "ai-training-knowledge-management"
status: "PUBLISHED"
createdAt: "2026-02-24T08:32:54.601Z"
updatedAt: "2026-03-12T09:00:28.225Z"
---

<h1>AI Training and Knowledge Management</h1>
<p>FinalDoc's AI gets smarter over time by learning from your specific documentation and the questions your readers ask. The AI Training section lets you add custom Q&amp;A pairs, review AI interactions, and train the AI to give better answers — tailored to your product and your readers.</p>

<h2>Opening AI Training</h2>
<ol>
<li>Go to <strong>Settings → AI (Ved AI) → AI Training &amp; Knowledge Management</strong></li>
</ol>

<h2>What Is the AI Knowledge Base?</h2>
<p>The AI Knowledge Base is a collection of question-and-answer pairs that the AI uses when answering reader queries. When a reader asks something that closely matches a Q&amp;A in the knowledge base, the AI uses that answer directly (rather than generating one from scratch). This gives you precise control over how the AI answers specific questions.</p>

<h2>Adding Q&amp;A Pairs Manually</h2>
<ol>
<li>In the AI Training view, click <strong>+ Add Knowledge Entry</strong></li>
<li>Enter the <strong>question</strong> — write it in the same language and style your readers use</li>
<li>Enter the <strong>answer</strong> — write the exact answer you want the AI to give for this question</li>
<li>Optionally add a <strong>source</strong> — the URL or article name this answer comes from</li>
<li>Click <strong>Save</strong></li>
</ol>
<p>The AI can now use this Q&amp;A pair when readers ask similar questions. Semantic similarity matching means even questions phrased differently are matched — you do not need to list every possible phrasing.</p>

<h2>Adding Q&amp;A from Query Insights</h2>
<p>You can promote helpful AI conversations to the knowledge base:</p>
<ol>
<li>Go to <strong>Feedback → AI Queries</strong></li>
<li>Find a conversation where the AI gave a good answer that a reader rated as helpful</li>
<li>Click <strong>Add to Training</strong></li>
<li>The Q&amp;A pair is added to the AI Knowledge Base for future use</li>
</ol>

<h2>Auto-Learning from Feedback</h2>
<p>Enable <strong>Auto-Learn</strong> to have FinalDoc automatically add Q&amp;A pairs from positively-rated AI conversations:</p>
<ol>
<li>In AI Training settings, find <strong>Auto-Learn from Positive Feedback</strong></li>
<li>Toggle it ON</li>
<li>When readers rate an AI response as helpful, it is added to the knowledge base automatically</li>
</ol>

<h2>Bulk Embedding (RAG Setup)</h2>
<p>FinalDoc uses RAG (Retrieval-Augmented Generation) for AI answers — it searches your articles using vector embeddings before generating a response. To enable this, your articles need to be embedded (converted to vector representations):</p>
<ol>
<li>In AI Training settings, click <strong>Embed All Articles</strong></li>
<li>FinalDoc processes all published articles and creates embeddings in the background</li>
<li>Progress is shown — this may take a few minutes for large KBs</li>
<li>Once complete, the AI can semantically search your entire documentation</li>
</ol>
<p>Articles are re-embedded automatically when they are updated. New articles are embedded when published.</p>

<h2>Review Queue</h2>
<p>The review queue shows AI Q&amp;A pairs flagged for human review — for example, answers that were rated as unhelpful, or auto-learned pairs that have not been reviewed by a human. Click any item to review, edit, approve, or delete it.</p>

<h2>Embedding Statistics</h2>
<p>At the bottom of the AI Training page, see embedding statistics:</p>
<ul>
<li>Total articles embedded</li>
<li>Total knowledge Q&amp;A entries</li>
<li>Total embedding chunks (each article is split into chunks for more precise search)</li>
</ul>