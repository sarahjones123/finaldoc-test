---
title: "Security Headers & IP Restriction"
description: "Configuring CSP, X-Frame-Options, and IP-based access control."
slug: "security-headers-ip-restriction"
status: "PUBLISHED"
createdAt: "2026-02-23T18:16:33.497Z"
updatedAt: "2026-03-12T13:27:31.453Z"
---

<h1>Security Headers and IP Restriction</h1>
<p>FinalDoc's security settings let you add HTTP security headers to your knowledge base and restrict access to specific IP addresses or ranges. These settings are for organizations with strict security requirements.</p>

<h2>Opening Security Settings</h2>
<ol>
<li>Go to <strong>Settings → Security &amp; Access → Security Headers &amp; IP Restriction</strong></li>
</ol>

<h2>HTTP Security Headers</h2>
<p>FinalDoc can add security headers to all responses from your knowledge base. These headers protect against common web attacks:</p>
<table>
<thead><tr><th>Header</th><th>What It Does</th></tr></thead>
<tbody>
<tr><td><strong>Content-Security-Policy (CSP)</strong></td><td>Controls which scripts, styles, and resources can load. Prevents XSS attacks</td></tr>
<tr><td><strong>X-Frame-Options</strong></td><td>Prevents your KB from being embedded in an iframe on other sites. Prevents clickjacking</td></tr>
<tr><td><strong>X-Content-Type-Options</strong></td><td>Prevents browsers from MIME-sniffing responses. Set to "nosniff"</td></tr>
<tr><td><strong>Referrer-Policy</strong></td><td>Controls how much referrer information is sent when readers navigate away</td></tr>
<tr><td><strong>HSTS</strong></td><td>Forces all connections to use HTTPS. Prevents SSL stripping attacks</td></tr>
</tbody>
</table>
<p>FinalDoc enables a sensible default set of security headers for all knowledge bases. You can customize or add additional headers here.</p>

<h2>IP Restriction</h2>
<p>IP restriction lets you limit access to your knowledge base to specific IP addresses or CIDR ranges — useful for internal documentation that should only be accessible from your office network or VPN.</p>

<h3>Configuring IP Restrictions</h3>
<ol>
<li>In Security Headers settings, find the <strong>IP Allowlist</strong> section</li>
<li>Click <strong>Add IP</strong></li>
<li>Enter an IP address (e.g., <code>192.168.1.1</code>) or CIDR range (e.g., <code>192.168.0.0/24</code>)</li>
<li>Add a label (e.g., "Office Network", "VPN")</li>
<li>Click <strong>Add</strong></li>
<li>Repeat for all allowed IPs/ranges</li>
<li>Click <strong>Enable IP Restriction</strong> to activate</li>
</ol>

<div style="border-left: 4px solid #ef4444; border-radius: 8px; padding: 16px; margin: 16px 0; background: rgba(239,68,68,0.08);">
<strong>Important:</strong> Before enabling IP restriction, make sure your own current IP address is in the allowlist, or you will lock yourself out of the knowledge base. Always add your IP first, then enable restriction.
</div>

<h2>Disabling IP Restriction</h2>
<ol>
<li>In the IP Restriction settings, click <strong>Disable IP Restriction</strong></li>
<li>The KB is immediately accessible from any IP again</li>
</ol>