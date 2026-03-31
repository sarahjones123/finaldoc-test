---
title: "February 2026 Release Notes"
description: ""
slug: "february-2026-release-notes"
status: "PUBLISHED"
createdAt: "2026-03-29T03:27:09.899Z"
updatedAt: "2026-03-29T04:00:23.141Z"
---

<h1>February 2026 — AI &amp; Infrastructure</h1>
<p>February was a massive month — the platform went from MVP to production-ready with 18 new features, security hardening, and AI-powered capabilities across every surface.</p>

<h2>New Features</h2>

<h3>AI-Powered Features</h3>
<ul>
<li><strong>RAG Semantic Search</strong> — pgvector-powered search replacing keyword matching, with 249 article embeddings</li>
<li><strong>Reader Chatbot</strong> — AI chatbot on public KB that answers questions using your articles as source of truth</li>
<li><strong>Voice Mode</strong> — Real-time voice conversations with your KB via OpenAI Realtime API (6 voices)</li>
<li><strong>Article Audio</strong> — Text-to-speech for every article with OpenAI TTS (tts-1 nova voice)</li>
<li><strong>AI Search Suggestions</strong> — Smart "Looking for X? Ask me!" prompts when search returns no results</li>
<li><strong>AI Doc Optimizer</strong> — Content health scoring (0-100) with auto-fix suggestions</li>
<li><strong>Doc Autopilot</strong> — Auto-generate documentation from GitHub repositories using AI code analysis</li>
<li><strong>Ticket Analysis</strong> — AI-powered support ticket analysis with ITSM platform connectors</li>
<li><strong>Design Assistant</strong> — Describe a look in plain English, AI generates the theme</li>
<li><strong>Auto-Draft</strong> — Generate draft articles from content gaps detected in search analytics</li>
</ul>

<h3>Video Studio</h3>
<ul>
<li>Article-to-Video generation with AI voiceover</li>
<li>Text-to-Video creation via FAL.ai</li>
<li>Non-Linear Editor (NLE) for scene customization</li>
<li>App screen capture for UI documentation videos</li>
</ul>

<h3>18 Features from Documentation Audit</h3>
<ul>
<li>Scroll memory, featured images, editor shortcuts, paste from Word</li>
<li>Pinned articles, folder colors, bulk actions</li>
<li>Threaded comments, @mentions, inline comments</li>
<li>Fuzzy search (pg_trgm), activity heatmap, contribution timeline</li>
<li>Content growth tracking, review backlog</li>
</ul>

<h3>Batch 2 &amp; 3 Features</h3>
<ul>
<li>Content Health Dashboard, Article Changelog, Smart Linking</li>
<li>Article Reactions (emoji voting), Webhook Events</li>
<li>Bulk API with token auth, Template Library (12 templates)</li>
<li>One-Click Translation (30+ languages), Offline PWA</li>
</ul>

<h2>Infrastructure</h2>
<ul>
<li><strong>Multi-server architecture</strong> — KVM4 + KVM8 with Nginx load balancing</li>
<li><strong>Redis caching</strong> — Sessions, rate limiting, dashboard, analytics, custom domains</li>
<li><strong>Custom domains</strong> — Full provisioning with DNS verify, certbot SSL, Nginx auto-config</li>
<li><strong>Subdomain KB</strong> — Clean paths on *.finaldoc.io subdomains</li>
<li><strong>PDF export overhaul</strong> — Mermaid + ReactFlow diagram rendering, branded templates</li>
</ul>

<h2>Security</h2>
<ul>
<li>bcrypt reader passwords, CSRF protection, IDOR fixes</li>
<li>SSRF/XSS protection, HTML escaping, webhook URL validation</li>
<li>Platform admin controls, owner-only billing</li>
<li>Nginx security headers, 4GB swap, DNS migration</li>
</ul>

<h2>Integrations</h2>
<ul>
<li>Microsoft Teams outgoing webhook with AI Q&amp;A</li>
<li>Slack notifications</li>
<li>OpenClaw AI Agent (WhatsApp, Telegram, Discord, web chat)</li>
<li>GitHub/GitLab/Bitbucket code repository sync</li>
</ul>