---
title: "Widget Builder Overview"
description: "How to create and configure an embeddable help widget for your website."
slug: "widget-builder-overview"
status: "PUBLISHED"
createdAt: "2026-02-23T18:13:43.384Z"
updatedAt: "2026-03-27T10:59:45.769Z"
---

<h1>External Widget Overview</h1>
<p>The FinalDoc Widget is an embeddable help assistant you can add to any website or web application. Visitors to your site see a small button in the corner — they click it to open a help panel that lets them search your knowledge base and chat with the AI assistant — without leaving your site.</p>

<h2>Opening the External Widget</h2>
<p>Click <strong>External Widget</strong> (the puzzle piece icon) in the left sidebar.</p>

<h2>What the Widget Does</h2>
<p>When a visitor opens your widget, they can:</p>
<ul>
<li><strong>Search your knowledge base</strong> — Type a question and see relevant articles immediately</li>
<li><strong>Browse articles</strong> — Navigate through categories to find what they need</li>
<li><strong>Chat with AI</strong> — Ask questions in natural language and get instant AI-powered answers based on your documentation</li>
<li><strong>Contact support</strong> — Submit a support request or contact form directly from the widget (if enabled)</li>
</ul>

<h2>Creating a Widget Configuration</h2>
<ol>
<li>In the External Widget, click <strong>+ New Widget</strong></li>
<li>Give it a name (internal — e.g., "Main Site Widget" or "Checkout Page Widget")</li>
<li>Connect it to your knowledge base project (or a specific workspace/version)</li>
<li>Configure the appearance (position, color, launcher text)</li>
<li>Configure which features are enabled (search, AI chat, contact form)</li>
<li>Click <strong>Save</strong></li>
</ol>

<h2>Widget Settings</h2>
<ul>
<li><strong>Position</strong> — Bottom-right (default) or bottom-left</li>
<li><strong>Launcher type</strong> — Icon only, icon + text ("Help"), or text button</li>
<li><strong>Color</strong> — The widget button and header color (should match your site's brand)</li>
<li><strong>Title</strong> — What appears at the top of the open widget (e.g., "Help Center")</li>
<li><strong>Greeting message</strong> — The AI's opening message when a visitor starts a chat</li>
<li><strong>Knowledge base access</strong> — Which workspace(s) the widget searches</li>
<li><strong>AI enabled</strong> — Toggle the AI chat feature on/off</li>
<li><strong>Contact form</strong> — Toggle the contact/support request form</li>
</ul>

<h2>Installing the Widget on Your Website</h2>
<ol>
<li>After saving, go to the <strong>Installation</strong> tab</li>
<li>Copy the provided JavaScript snippet</li>
<li>Paste it inside the <code>&lt;body&gt;</code> tag of your website (just before the closing <code>&lt;/body&gt;</code> tag)</li>
<li>The widget appears automatically on your site within a few seconds</li>
</ol>
<p>The snippet is unique to your widget configuration. Do not share it — it is tied to your project.</p>

<h2>Restricting the Widget to Specific Domains</h2>
<p>To prevent the widget code from being used on unauthorized websites:</p>
<ol>
<li>In the Widget settings, find <strong>Allowed Domains</strong></li>
<li>Add your website domain(s) (e.g., <code>yourcompany.com</code>, <code>app.yourcompany.com</code>)</li>
<li>The widget only loads on the listed domains — it shows a blank/blocked state anywhere else</li>
</ol>

<h2>Multiple Widget Configurations</h2>
<p>You can create different widget configurations for different parts of your site — for example, a lightweight version for the marketing site and a more detailed version for the app dashboard. Each configuration gets its own JavaScript snippet.</p>

<h2>Widget Analytics</h2>
<p>Widget usage (searches, questions asked, articles opened) is tracked in <strong>Analytics → Article &amp; Reader Analytics</strong>. Widget sessions are identified by origin domain.</p>