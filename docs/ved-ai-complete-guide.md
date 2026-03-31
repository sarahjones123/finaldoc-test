---
title: "Ved AI — Complete Guide"
description: "Complete guide to all 29 AI features in FinalDoc — writing, translation, diagrams, video, voice, ticket analysis, doc autopilot, content health, multi-channel agents, and enterprise configuration."
slug: "ved-ai-complete-guide"
status: "PUBLISHED"
createdAt: "2026-03-21T08:12:37.720Z"
updatedAt: "2026-03-27T10:59:45.857Z"
---

<h1>Ved AI — Complete Guide</h1>
<p>Ved AI is the intelligence layer that powers every corner of FinalDoc. With <strong>29 AI-driven features</strong> spanning content creation, optimization, analytics, video, voice, and multi-channel support, it is the most comprehensive AI suite built for documentation teams.</p>

<div style="background:#f0fdfa;border-left:4px solid #14b8a6;padding:12px 16px;border-radius:4px;margin:16px 0">
  <strong>Why Ved AI?</strong> Every feature works inside FinalDoc — no tab switching, no copy-pasting into ChatGPT, no context loss. Your articles, your brand voice, your data — all in one place.
</div>

<h2>Content Creation &amp; Writing</h2>

<h3>Writer Assistant</h3>
<p>Open any article and click the <strong>AI</strong> button to access 14+ writing actions:</p>
<ul>
<li><strong>Draft</strong> — Generate a full article from a topic or outline</li>
<li><strong>Improve</strong> — Rewrite selected text for clarity and flow</li>
<li><strong>Shorten / Lengthen</strong> — Adjust content length without losing meaning</li>
<li><strong>Simplify / Elaborate</strong> — Change complexity level for your audience</li>
<li><strong>Tone adjustment</strong> — Shift between professional, casual, technical, friendly</li>
<li><strong>Convert bullets to prose</strong> — And vice versa</li>
<li><strong>Generate tags</strong> — Auto-suggest relevant tags for the article</li>
<li><strong>SEO optimize</strong> — Rewrite for search engine visibility</li>
<li><strong>Summarize</strong> — Create concise summaries for previews and metadata</li>
</ul>
<p><a href="/article/ved-ai-writer-assistant">Read the full Writer Assistant guide</a></p>

<h3>One-Click Translation</h3>
<p>Translate any article into 30+ languages with a single click. Title, description, and content are translated in parallel. Supports all major languages with flag emoji indicators in the language selector.</p>
<p><a href="/article/one-click-ai-translation">Read the Translation guide</a></p>

<h3>Auto-Draft from Content Gaps</h3>
<p>When Analytics detects search queries with no matching articles, Ved AI can generate a draft article in one click — filling the gap before readers even notice.</p>
<p><a href="/article/ai-auto-draft-from-content-gaps">Read more</a></p>

<h2>Visual Content</h2>

<h3>Diagram &amp; Chart Generation</h3>
<p>Describe what you need in plain English and Ved AI creates it:</p>
<ul>
<li><strong>Flowcharts</strong> — Process flows, decision trees</li>
<li><strong>Sequence diagrams</strong> — API call flows, user journeys</li>
<li><strong>Architecture diagrams</strong> — System design, infrastructure</li>
<li><strong>ER diagrams</strong> — Database schemas</li>
<li><strong>Mind maps</strong> — Concept exploration</li>
<li><strong>Bar / Line / Pie charts</strong> — Data visualization as SVG</li>
</ul>
<p>Output as interactive Mermaid (editable) or PNG images. Powered by Gemini 2.0 Flash.</p>

<h3>Video Generation</h3>
<p>Turn any article into a narrated video. Select a voice, customize the script, add branding overlays, and export. Supports clips (30s), shorts (1-3min), classic (5-10min), and longform. Powered by FAL.ai.</p>
<p><a href="/article/video-generation">Read the Video guide</a></p>

<h3>Voice Mode &amp; Article Audio</h3>
<p>Readers can <strong>listen</strong> to any article with text-to-speech (6 voices: shimmer, alloy, echo, coral, sage, ash). Or use <strong>Voice Mode</strong> for real-time voice conversations with your KB using the OpenAI Realtime API — ask questions and get spoken answers.</p>

<h2>Content Intelligence</h2>

<h3>Content Health &amp; Doc Optimizer</h3>
<p>Ved AI scans every article and assigns a <strong>health score (0-100)</strong> based on structure, title quality, description, content depth, tags, and SEO. Suggestions are categorized by severity (high / medium / low) and can be auto-applied with one click.</p>
<p><a href="/article/ai-optimizer">Read the Optimizer guide</a></p>

<h3>Smart Article Linking</h3>
<p>Analyzes your article content and suggests contextually relevant internal links with confidence scores. Strengthens your KB's interconnectedness and helps readers discover related content.</p>
<p><a href="/article/smart-article-linking-ai">Read more</a></p>

<h3>Duplicate Detection</h3>
<p>Before publishing, Ved AI checks for semantically similar articles in your KB — preventing redundancy and keeping your documentation clean.</p>

<h3>AI-Powered Search Suggestions</h3>
<p>When a reader's search returns no results, Ved AI uses semantic search (pgvector + RAG) to suggest related articles and offers to answer the question directly via chatbot.</p>
<p><a href="/article/ai-powered-search-suggestions">Read more</a></p>

<h2>Contextual Task Creation</h2>
<p>Create tasks directly from the context where you spot issues — no need to switch to the dashboard.</p>
<ul>
<li><strong>From the Editor</strong> — Click the <strong>Task</strong> button in the editor toolbar. A modal opens with the title pre-filled ("Review: Article Name") and the article pre-linked. Choose the task type (Content Review, Content Update, Translation, Screenshot Update, Link Fix, SEO) and priority before creating.</li>
<li><strong>From Feedback</strong> — Click the task icon on any reader feedback item. Creates a "Content Update" task with the feedback message as the description and the article pre-linked. Negative feedback is automatically marked as HIGH priority.</li>
<li><strong>From AI Suggestions</strong> — The dashboard AI tab surfaces stale articles, negative feedback, and content gaps. Click <strong>Accept</strong> to instantly convert any suggestion into a real task.</li>
</ul>
<p>All tasks appear in the dashboard Tasks card and can be managed via the slide-over detail panel or Kanban board.</p>

<h2>Reader-Facing AI</h2>

<h3>Reader Chatbot (RAG)</h3>
<p>An AI chatbot embedded in your public knowledge base that answers reader questions using your articles as the source of truth. Features:</p>
<ul>
<li>Retrieval-Augmented Generation with pgvector semantic search</li>
<li>Source attribution — shows which articles the answer came from</li>
<li>Conversation persistence and history</li>
<li>Feedback voting (helpful / not helpful)</li>
<li>Customizable name, welcome message, colors, position, and button style (peek / static / capsule)</li>
</ul>
<p><a href="/article/ved-ai-reader-chatbot">Read the Chatbot guide</a></p>

<h3>Design Assistant (Vibe Coding)</h3>
<p>Describe the look you want in plain English — "make it dark with glassmorphism and a purple accent" — and Ved AI generates the theme, CSS, header/footer, hero section, and animations. No design skills needed.</p>
<p><a href="/article/ved-ai-design-assistant">Read more</a></p>

<h2>Documentation Automation</h2>

<h3>Doc Autopilot</h3>
<p>Automatically generate entire knowledge bases from:</p>
<ul>
<li><strong>GitHub repos</strong> — Analyzes code, README, and structure to create Getting Started, API Reference, and Feature docs</li>
<li><strong>Live apps</strong> — Takes screenshots and generates UI guides</li>
<li><strong>APIs</strong> — Reads endpoints and creates API documentation</li>
</ul>
<p>Supports 6 doc types: Getting Started, User Guide, API Reference, Feature Docs, UI Guides, Troubleshooting. Auto-syncs via GitHub webhooks.</p>
<p><a href="/article/doc-autopilot-overview">Read the Autopilot guide</a></p>

<h3>Ticket Analysis</h3>
<p>Connect your support channels (Zendesk, Intercom, etc.) and Ved AI analyzes incoming tickets to identify:</p>
<ul>
<li>Common issue clusters and trends</li>
<li>Severity distribution</li>
<li>Knowledge gaps — tickets that could be deflected with better docs</li>
<li>Specific article recommendations per ticket</li>
</ul>
<p><a href="/article/ticket-analysis-overview">Read the Ticket Analysis guide</a></p>

<h2>Multi-Channel AI Agent</h2>

<h3>OpenClaw Agent</h3>
<p>Deploy Ved AI as a standalone agent on external channels:</p>
<table>
<thead><tr><th>Channel</th><th>Integration</th></tr></thead>
<tbody>
<tr><td><strong>WhatsApp</strong></td><td>QR code pairing</td></tr>
<tr><td><strong>Telegram</strong></td><td>Bot token</td></tr>
<tr><td><strong>Slack</strong></td><td>OAuth app</td></tr>
<tr><td><strong>Discord</strong></td><td>Bot integration</td></tr>
<tr><td><strong>Microsoft Teams</strong></td><td>Outgoing webhook</td></tr>
<tr><td><strong>WebChat</strong></td><td>Embeddable widget</td></tr>
</tbody>
</table>
<p>Each channel receives AI-powered Q&amp;A backed by your knowledge base. Includes sleep/wake mode, usage analytics, and conversation routing.</p>
<p><a href="/article/ai-agent-openclaw">Read the Agent guide</a></p>

<h2>Analytics &amp; Insights</h2>

<h3>Content Gap Analysis</h3>
<p>Analyzes search queries across your KB to identify unanswered questions. Ranks gaps by frequency and priority. One-click draft generation for each gap.</p>
<p><a href="/article/search-analytics-content-gaps">Read more</a></p>

<h3>AI Insights Panel</h3>
<p>Real-time AI-generated insights from your KB metrics: trends, anomalies, recommendations, and summaries with actionable next steps.</p>

<h3>Feedback &amp; Query Insights</h3>
<p>Analyzes patterns in reader feedback and chatbot queries. Identifies sentiment trends and surfaces recommendations to improve content.</p>
<p><a href="/article/ved-ai-feedback-query-insights">Read more</a></p>

<h2>Enterprise Configuration</h2>
<p>All AI configuration is managed from a single page: <strong>Settings &gt; AI &gt; AI Configuration</strong>.</p>
<table>
<thead><tr><th>Setting</th><th>What It Controls</th></tr></thead>
<tbody>
<tr><td><strong>AI Provider</strong></td><td>Choose FinalDoc AI (cloud) or Your Private Cloud (Azure OpenAI, AWS Bedrock, Google Vertex AI, custom endpoint)</td></tr>
<tr><td><strong>Brand Voice &amp; Style Guide</strong></td><td>Define tone, personality, and terminology for consistent AI outputs</td></tr>
<tr><td><strong>Prompt Templates</strong></td><td>Customize prompts for each AI action type</td></tr>
<tr><td><strong>Compliance &amp; Data Handling</strong></td><td>Data retention, PII masking, privacy settings, audit logging</td></tr>
<tr><td><strong>Usage Dashboard</strong></td><td>Real-time usage metrics, cost breakdown, token tracking by feature</td></tr>
<tr><td><strong>AI Training</strong></td><td>Manually train AI with Q&amp;A pairs, review queues, and auto-learning from feedback</td></tr>
</tbody>
</table>
<p>Find all settings under <strong>Settings &gt; AI (Ved AI)</strong>.</p>

<h2>Technology Stack</h2>
<ul>
<li><strong>LLMs</strong> — OpenAI GPT-4o-mini (writing &amp; chat), Gemini 2.0 Flash (diagrams), Claude (via BYOK)</li>
<li><strong>Embeddings</strong> — OpenAI text-embedding-3-small (1536 dimensions)</li>
<li><strong>Vector Search</strong> — pgvector on PostgreSQL for semantic retrieval</li>
<li><strong>Voice</strong> — OpenAI TTS (tts-1 nova) + Realtime API for voice chat</li>
<li><strong>Video</strong> — FAL.ai queue system for video generation</li>
<li><strong>Streaming</strong> — Server-sent events (SSE) for real-time AI responses</li>
</ul>