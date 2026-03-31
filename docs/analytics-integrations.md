---
title: "Analytics Integrations"
description: "Connect Google Analytics, Hotjar, Mixpanel, Segment, and Heap to track reader behavior."
slug: "analytics-integrations"
status: "PUBLISHED"
createdAt: "2026-02-23T18:26:53.382Z"
updatedAt: "2026-03-26T19:01:38.970Z"
---

<h1>Analytics Integrations</h1>
<p>In addition to FinalDoc's built-in analytics, you can connect third-party analytics services to track knowledge base usage in your existing analytics stack. This lets your team see KB data alongside website and product analytics in the tools they already use.</p>

<h2>Opening Analytics Integrations</h2>
<ol>
<li>Go to <strong>Settings</strong> in the left sidebar</li>
<li>Under <strong>Integrations</strong>, click <strong>Analytics</strong></li>
</ol>

<h2>Supported Analytics Platforms</h2>

<h3>Google Analytics 4 (GA4)</h3>
<ol>
<li>In GA4, get your Measurement ID (format: <code>G-XXXXXXXXXX</code>)</li>
<li>In FinalDoc, paste it into the <strong>Google Analytics Measurement ID</strong> field</li>
<li>Click <strong>Save</strong></li>
</ol>
<p>FinalDoc injects the GA4 snippet into your KB pages. GA4 tracks page views, session duration, and bounce rate automatically. Article URLs appear in GA4 as standard page paths.</p>

<h3>Google Tag Manager (GTM)</h3>
<ol>
<li>In GTM, get your Container ID (format: <code>GTM-XXXXXXX</code>)</li>
<li>Paste it into the <strong>GTM Container ID</strong> field in FinalDoc and save</li>
</ol>
<p>GTM loads on every KB page. Use GTM tags to fire any analytics tool, remarketing pixel, or tracking script — without editing FinalDoc's Custom JavaScript field.</p>

<h3>Mixpanel</h3>
<ol>
<li>In Mixpanel, get your Project Token</li>
<li>Paste it into the <strong>Mixpanel Project Token</strong> field in FinalDoc and save</li>
</ol>
<p>FinalDoc sends these events to Mixpanel: <code>KB Page View</code>, <code>KB Article Search</code>, <code>KB Feedback Submitted</code>, <code>KB Chatbot Opened</code>.</p>

<h3>Amplitude</h3>
<ol>
<li>In Amplitude, get your API Key from Settings → Projects</li>
<li>Paste it into the <strong>Amplitude API Key</strong> field in FinalDoc and save</li>
</ol>
<p>FinalDoc fires page view and interaction events to your Amplitude project.</p>

<h3>Segment</h3>
<ol>
<li>In Segment, create a JavaScript source and get the Write Key</li>
<li>Paste it into the <strong>Segment Write Key</strong> field in FinalDoc and save</li>
</ol>
<p>FinalDoc fires standard <code>page()</code> calls on every KB page view and <code>track()</code> calls for search, feedback, and chatbot events. Segment then forwards data to any of your connected downstream tools (Mixpanel, Amplitude, BigQuery, etc.).</p>

<h3>Heap</h3>
<ol>
<li>In Heap, get your App ID from Account → Projects</li>
<li>Paste it into the <strong>Heap App ID</strong> field in FinalDoc and save</li>
</ol>
<p>Heap auto-captures all interactions on your KB pages — clicks, scrolls, form fills — with no additional event configuration required.</p>

<h3>Hotjar</h3>
<ol>
<li>In Hotjar, get your Site ID</li>
<li>Paste it into the <strong>Hotjar Site ID</strong> field in FinalDoc and save</li>
</ol>
<p>Hotjar provides session recordings, heatmaps, and user feedback polls on your KB. Useful for understanding where readers click, how far they scroll, and where they get stuck.</p>

<h3>FullStory</h3>
<ol>
<li>In FullStory, get your Org ID from Admin → General Settings</li>
<li>Paste it into the <strong>FullStory Org ID</strong> field in FinalDoc and save</li>
</ol>
<p>FullStory records reader sessions for playback and frustration signal analysis.</p>

<h3>GoSquared</h3>
<ol>
<li>In GoSquared, get your Project Token from Project Settings</li>
<li>Paste it into the <strong>GoSquared Project Token</strong> field in FinalDoc and save</li>
</ol>
<p>GoSquared provides real-time visitor analytics for your KB.</p>

<h2>Custom Analytics (via JavaScript)</h2>
<p>For any analytics tool not listed above, use <strong>Settings → Appearance → Custom JavaScript</strong> to add the tracking snippet manually. This approach works for any tool that provides a JavaScript snippet — just paste the embed code and it will load on every KB page.</p>

<h2>What Data Is Sent</h2>
<p>FinalDoc sends only non-personally identifiable data to third-party analytics integrations:</p>
<ul>
<li>Page URL (article slug, not full URL)</li>
<li>Page title</li>
<li>Event type (page view, search, feedback)</li>
<li>Search query text</li>
</ul>
<p>Reader email addresses and personal data are <strong>not</strong> sent to third-party analytics integrations.</p>

<h2>Built-in FinalDoc Analytics</h2>
<p>Before connecting third-party tools, check if FinalDoc's native analytics already cover your needs. FinalDoc's built-in analytics (under Analytics in the sidebar) tracks article views, reader sessions, search queries, content gaps, feedback, team performance, and activity heatmaps — all without any external integration required.</p>