---
title: "KB Navigation & Search"
description: "How sidebar navigation, breadcrumbs, and full-text search work for readers."
slug: "kb-navigation-search"
status: "PUBLISHED"
createdAt: "2026-02-24T03:51:08.755Z"
updatedAt: "2026-03-12T13:27:59.301Z"
---

<h1>KB Navigation and Search</h1>
<p>Great navigation and search make the difference between a knowledge base that readers can actually find answers in versus one that feels like a maze. FinalDoc provides several search and navigation mechanisms to help readers find what they need quickly.</p>

<h2>The Search Bar</h2>
<p>The search bar is the primary way readers find content. It appears prominently at the top of the KB homepage and in the KB header on all pages.</p>

<h3>How Search Works</h3>
<p>FinalDoc uses a multi-layer search system:</p>
<ol>
<li><strong>Keyword matching</strong> — Finds articles that contain the exact words typed</li>
<li><strong>Full-text search</strong> — PostgreSQL full-text search across all article content</li>
<li><strong>Fuzzy matching</strong> — Finds articles even with typos ("installtion" still finds "installation")</li>
<li><strong>Semantic AI search</strong> — Uses vector embeddings to find articles about the same topic even when exact words differ ("how to log in" finds articles about "authentication" and "sign in")</li>
</ol>
<p>Results are ranked by relevance — articles where the search term appears in the title or early in the content rank higher.</p>

<h3>AI Search Suggestions</h3>
<p>If a search returns no results, FinalDoc's AI suggests related articles that might answer the question. This uses semantic similarity to find articles that are conceptually related, even if the words are different. Readers see a "You might be looking for..." section below the empty results.</p>

<h2>The Sidebar Navigation</h2>
<p>The left sidebar shows your full category and article tree:</p>
<ul>
<li>Click a category name to expand it and see articles inside</li>
<li>Click an article title to navigate to it</li>
<li>The current article is highlighted in the sidebar so readers always know where they are</li>
<li>On mobile, the sidebar collapses into a hamburger menu — tap the menu icon to open it</li>
</ul>

<h2>Table of Contents</h2>
<p>For long articles, a <strong>Table of Contents</strong> automatically appears on the right side (on desktop) or as a collapsible section (on mobile). It is built from the article's H2 and H3 headings. Clicking any entry scrolls to that section instantly.</p>
<p>Enable or disable the table of contents in <strong>Settings → Appearance → Article Display → Show Table of Contents</strong>.</p>

<h2>Breadcrumb Navigation</h2>
<p>At the top of every article page, a breadcrumb trail shows the path:</p>
<p><strong>Home → Category → Sub-category → Article Title</strong></p>
<p>Each step is clickable. Breadcrumbs help readers understand where they are in the KB hierarchy and quickly navigate up to a parent category.</p>

<h2>Tags Navigation</h2>
<p>Article tags appear as clickable chips below the article title. Clicking a tag shows a filtered list of all articles with that tag — helping readers find related content beyond the current category structure.</p>

<h2>Reading Progress</h2>
<p>A thin progress bar at the top of each article page shows how far the reader has scrolled through the article. When they scroll to the bottom, the bar is full. This helps readers track their position in long articles.</p>

<h2>Continue Reading</h2>
<p>When a reader visits your KB after a break, FinalDoc remembers where they were and shows a "Continue reading from where you left off" prompt. This uses their browser's local storage and does not require login.</p>

<h2>Keyboard Navigation</h2>
<p>Readers can use keyboard shortcuts for faster navigation:</p>
<ul>
<li><strong>/</strong> or <strong>Ctrl+K</strong> — Focus the search bar from anywhere on the page</li>
<li><strong>Arrow keys</strong> — Navigate search results</li>
<li><strong>Enter</strong> — Open the selected search result</li>
<li><strong>Escape</strong> — Close the search or dismiss a dialog</li>
</ul>