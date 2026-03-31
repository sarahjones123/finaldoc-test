---
title: "Offline Reading (PWA)"
description: "Install the knowledge base as a Progressive Web App for offline article access."
slug: "offline-reading-pwa"
status: "PUBLISHED"
createdAt: "2026-02-27T10:22:40.958Z"
updatedAt: "2026-03-21T03:06:19.355Z"
---

<h1>Offline Reading (PWA)</h1>
<p>FinalDoc's public knowledge base is a Progressive Web App (PWA). This means readers can install it on their device and continue reading articles even when they have no internet connection — as long as they previously visited those articles while online.</p>

<h2>How Offline Reading Works</h2>
<ol>
<li>A reader visits your knowledge base with an internet connection</li>
<li>The browser automatically caches the app shell (navigation, layout, fonts) and any articles the reader has viewed</li>
<li>If the reader returns to the KB while offline, the cached content loads from the device storage</li>
<li>The reader sees a small banner at the top indicating "You are offline — showing cached content"</li>
</ol>

<h2>Installing the PWA</h2>
<p>On mobile devices, readers may be prompted to "Add to Home Screen" — this installs the KB as an app icon on their phone's home screen. On desktop Chrome, a small install button appears in the address bar.</p>
<p>After installing:</p>
<ul>
<li>The KB opens in its own window (not inside a browser tab)</li>
<li>It feels like a native app</li>
<li>Previously viewed articles are available offline</li>
</ul>

<h2>What Works Offline</h2>
<ul>
<li>Previously visited articles (full content, images that were cached)</li>
<li>Navigation between cached articles</li>
<li>The KB layout and branding</li>
</ul>

<h2>What Requires Internet</h2>
<ul>
<li>Searching (search queries are sent to the server)</li>
<li>AI chatbot conversations</li>
<li>Articles not previously visited</li>
<li>Reader login/logout</li>
<li>Submitting feedback</li>
</ul>

<h2>Cache Behavior</h2>
<p>The service worker uses different strategies for different content:</p>
<ul>
<li><strong>App shell</strong> (layout, navigation, fonts): Cache-first — always loads from cache even when online, checks for updates in the background</li>
<li><strong>Articles</strong>: Network-first — tries to get the latest from the server; falls back to cache if offline</li>
</ul>
<p>This means readers always see the latest article content when online, but can fall back to cached versions when not connected.</p>

<h2>From the Admin Perspective</h2>
<p>The PWA functionality is enabled by default on all FinalDoc knowledge bases — there is nothing to configure. Your readers get offline support automatically.</p>
<p>If you want to see the service worker in action, open your browser's Developer Tools → Application → Service Workers when viewing your KB. You will see the FinalDoc service worker registered and active.</p>