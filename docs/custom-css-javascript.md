---
title: "Custom CSS & JavaScript"
description: "Inject custom CSS and JavaScript into your FinalDoc knowledge base for advanced customization."
slug: "custom-css-javascript"
status: "PUBLISHED"
createdAt: "2026-02-24T05:48:16.832Z"
updatedAt: "2026-03-18T18:57:56.867Z"
---

<h1>Custom CSS &amp; JavaScript</h1>
<p>For customizations beyond what the Portal Builder and Design Studio offer, you can inject custom CSS and JavaScript into your public knowledge base. This lets you make any visual or behavioral changes you need — as long as you know CSS and JavaScript.</p>

<h2>Opening Custom CSS &amp; JavaScript</h2>
<ol>
<li>Go to <strong>Settings → Appearance → Custom CSS &amp; JavaScript</strong></li>
</ol>

<h2>Custom CSS</h2>
<p>CSS entered here is injected into the <code>&lt;head&gt;</code> of every page on your public knowledge base (wrapped in a <code>&lt;style&gt;</code> tag).</p>

<h3>Use Cases for Custom CSS</h3>
<ul>
<li>Override default fonts: <code>body { font-family: 'Your Brand Font', sans-serif; }</code></li>
<li>Hide elements you don't want (e.g., hide the reader feedback widget on certain pages)</li>
<li>Add custom spacing, padding, or layout adjustments</li>
<li>Style article headings with custom colors or underlines</li>
<li>Add a custom announcement bar above the KB header</li>
</ul>

<h3>Example</h3>
<pre><code>/* Make article headings your brand color */
.article-content h1, .article-content h2 {
  color: #7c3aed;
}

/* Add a subtle shadow to the KB header */
.kb-header {
  box-shadow: 0 2px 8px rgba(0,0,0,0.08);
}</code></pre>

<h2>Custom JavaScript</h2>
<p>JavaScript entered here is injected before the closing <code>&lt;/body&gt;</code> tag on every KB page (wrapped in a <code>&lt;script&gt;</code> tag). The script runs after the KB has loaded.</p>

<h3>Use Cases for Custom JavaScript</h3>
<ul>
<li>Inject third-party analytics (Mixpanel, Amplitude, etc.) tracking code</li>
<li>Add a custom chat widget (Crisp, Intercom, etc.) to the KB</li>
<li>Implement custom scroll-to-top button behavior</li>
<li>Add a "print article" button</li>
<li>Integrate with your product's own user session (e.g., auto-log in readers who are logged into your app)</li>
</ul>

<h3>Security Note</h3>
<p>FinalDoc does not sandbox custom JavaScript — it runs with full access to the page. Only add scripts you trust completely. Malicious or buggy custom JavaScript can break your KB for readers.</p>

<div style="border-left: 4px solid #f59e0b; border-radius: 8px; padding: 16px; margin: 16px 0; background: rgba(245,158,11,0.08);">
<strong>Note:</strong> Custom CSS and JavaScript only appear on your public knowledge base. They do not affect the FinalDoc admin interface.
</div>

<h2>Testing Before Saving</h2>
<p>Test your CSS/JavaScript in your browser's developer tools (F12) on the live KB page first. Once it works correctly there, paste it into the Custom CSS/JS field and save.</p>

<h2>Debugging Issues</h2>
<p>If your custom CSS or JS breaks your KB:</p>
<ol>
<li>Go back to Settings → Appearance → Custom CSS &amp; JavaScript</li>
<li>Remove the problematic code</li>
<li>Click Save</li>
<li>The KB returns to normal immediately</li>
</ol>