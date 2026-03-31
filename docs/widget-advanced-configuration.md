---
title: "Widget Advanced Configuration"
description: ""
slug: "widget-advanced-configuration"
status: "PUBLISHED"
createdAt: "2026-02-24T08:37:07.754Z"
updatedAt: "2026-03-27T10:59:45.661Z"
---

<h1>Widget Advanced Configuration</h1>
<p>Beyond the basic installation and visual settings, the FinalDoc widget has advanced configuration options that control its behavior — which pages it shows on, what content it searches, and how it behaves programmatically via JavaScript.</p>

<h2>Opening Widget Configuration</h2>
<ol>
<li>Click <strong>External Widget</strong> in the left sidebar</li>
<li>Click your widget to open its settings</li>
<li>Navigate between tabs: <strong>Design</strong>, <strong>Behavior</strong>, <strong>Content</strong>, <strong>Advanced</strong>, <strong>Install</strong></li>
</ol>

<h2>Behavior Settings</h2>

<h3>Launch Behavior</h3>
<ul>
<li><strong>Auto-open on load</strong> — The widget opens automatically when the page loads (not recommended — intrusive)</li>
<li><strong>Open on scroll</strong> — Widget opens after the user scrolls a certain percentage down the page</li>
<li><strong>Manual only</strong> (default) — Widget only opens when the user clicks the button</li>
</ul>

<h3>Search Mode</h3>
<ul>
<li><strong>Knowledge base only</strong> — Searches only articles from your KB</li>
<li><strong>Site content + KB</strong> — Also searches site content you've configured (see Widget Site Content)</li>
</ul>

<h3>Fallback Behavior</h3>
<ul>
<li><strong>Show AI chatbot if no results</strong> — When search finds no articles, the AI chatbot activates to answer the reader's question directly</li>
<li><strong>Show contact form if no results</strong> — Shows a contact/email form when no articles match</li>
</ul>

<h2>Page-Specific Rules</h2>
<p>Control which pages of your website show the widget:</p>
<ul>
<li><strong>Show on all pages</strong> (default) — Widget appears everywhere the snippet is installed</li>
<li><strong>Show only on these pages</strong> — Enter URL patterns (e.g., <code>/app/*</code>, <code>/dashboard</code>) — widget only shows on matching pages</li>
<li><strong>Hide on these pages</strong> — Enter URL patterns — widget hides on matching pages (e.g., hide on the login page)</li>
</ul>

<h2>JavaScript API</h2>
<p>Control the widget programmatically from your website's JavaScript:</p>
<pre><code>// Open the widget
window.FinalDoc.open();

// Close the widget
window.FinalDoc.close();

// Pre-fill search query
window.FinalDoc.search('password reset');

// Pre-fill chatbot question
window.FinalDoc.ask('How do I reset my password?');

// Listen for events
window.FinalDoc.on('open', () => console.log('Widget opened'));
window.FinalDoc.on('search', (query) => console.log('Searched for', query));</code></pre>
<p>This lets you trigger the widget from your own buttons or in response to user actions in your app.</p>

<h2>Custom Trigger Button</h2>
<p>If you want to use your own button instead of the FinalDoc floating button:</p>
<ol>
<li>In the widget's <strong>Advanced</strong> tab, enable <strong>Hide default button</strong></li>
<li>Add a button or link in your website with an onclick that calls <code>window.FinalDoc.open()</code></li>
<li>The FinalDoc button disappears but the widget panel still works</li>
</ol>

<h2>Allowed Domains</h2>
<p>Enter the domains where your widget is authorized to load (e.g., <code>yourcompany.com</code>, <code>app.yourcompany.com</code>). The widget script checks this list and refuses to load on unauthorized domains — preventing someone from stealing your widget ID and embedding it on their website.</p>