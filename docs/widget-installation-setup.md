---
title: "Widget Installation & Setup"
description: "Install the FinalDoc help widget on your website or web application."
slug: "widget-installation-setup"
status: "PUBLISHED"
createdAt: "2026-02-24T03:51:00.843Z"
updatedAt: "2026-03-27T10:59:45.698Z"
---

<h1>Widget Installation and Setup</h1>
<p>Installing the FinalDoc help widget on your website takes about 5 minutes. You copy a small JavaScript snippet and paste it into your website's HTML. That is it — the widget loads automatically on every page where the snippet is included.</p>

<h2>Step 1: Create a Widget Configuration</h2>
<ol>
<li>Click <strong>External Widget</strong> in the left sidebar</li>
<li>Click <strong>+ New Widget</strong></li>
<li>Give it a name (e.g., "Main Site Widget")</li>
<li>Select the knowledge base workspace it should search</li>
<li>Configure appearance settings (color, position, name)</li>
<li>Click <strong>Save</strong></li>
</ol>

<h2>Step 2: Get the Install Snippet</h2>
<ol>
<li>Click the <strong>Install</strong> tab in your widget configuration</li>
<li>Copy the JavaScript snippet — it looks like this:
<pre><code>&lt;script&gt;
  window.finaldocConfig = { widgetId: 'YOUR_WIDGET_ID' };
&lt;/script&gt;
&lt;script src="https://app.finaldoc.io/widget.js" async&gt;&lt;/script&gt;</code></pre>
</li>
</ol>

<h2>Step 3: Add the Snippet to Your Website</h2>
<p>Paste the snippet just before the closing <code>&lt;/body&gt;</code> tag on every page where you want the widget to appear. The widget loads asynchronously — it does not slow down your page load.</p>

<h3>For different website platforms:</h3>

<h4>Static HTML</h4>
<p>Paste the snippet in your HTML file before <code>&lt;/body&gt;</code>.</p>

<h4>WordPress</h4>
<ol>
<li>Go to Appearance → Theme Editor → footer.php</li>
<li>Paste before the <code>&lt;/body&gt;</code> tag</li>
<li>Or use a plugin like "Insert Headers and Footers"</li>
</ol>

<h4>Webflow</h4>
<ol>
<li>Project Settings → Custom Code → Footer Code</li>
<li>Paste the snippet there</li>
</ol>

<h4>React/Next.js</h4>
<p>Import the snippet in your root layout component or use a dedicated Script component.</p>

<h4>Shopify</h4>
<ol>
<li>Online Store → Themes → Edit Code</li>
<li>Add to theme.liquid before <code>&lt;/body&gt;</code></li>
</ol>

<h2>Verifying Installation</h2>
<ol>
<li>After adding the snippet, visit your website</li>
<li>You should see the FinalDoc widget button in the corner</li>
<li>Click it to open the widget</li>
<li>Try searching for an article — you should see results from your knowledge base</li>
</ol>
<p>If the widget does not appear, check the browser console for JavaScript errors. The most common issue is the snippet not being placed correctly in the HTML.</p>

<h2>Domain Restriction</h2>
<p>For security, add your website's domain to the <strong>Allowed Domains</strong> list in your widget configuration. This prevents the widget code from loading on unauthorized websites. In the External Widget, find <strong>Allowed Domains</strong> and add your domain (e.g., <code>yourcompany.com</code>).</p>