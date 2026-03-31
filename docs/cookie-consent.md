---
title: "Cookie Consent"
description: "GDPR-compliant cookie consent banner configuration."
slug: "cookie-consent"
status: "PUBLISHED"
createdAt: "2026-02-23T18:16:25.865Z"
updatedAt: "2026-03-12T09:12:47.040Z"
---

<h1>Cookie Consent</h1>
<p>If your knowledge base is accessible to users in the EU (European Union) or other jurisdictions with privacy laws (GDPR, CCPA), you may need to display a cookie consent notice. FinalDoc includes a built-in cookie consent banner you can configure and activate.</p>

<h2>Opening Cookie Consent Settings</h2>
<ol>
<li>Go to <strong>Settings → Domain &amp; SEO → Cookie Consent</strong></li>
</ol>

<h2>Enabling the Cookie Banner</h2>
<ol>
<li>Toggle <strong>Enable Cookie Consent Banner</strong> to ON</li>
<li>Configure the banner:
  <ul>
    <li><strong>Message text</strong> — Your cookie notice text (e.g., "We use cookies to improve your experience. By using our site, you agree to our Privacy Policy.")</li>
    <li><strong>Accept button text</strong> — Default: "Accept All"</li>
    <li><strong>Decline button text</strong> — Default: "Reject Non-Essential" (or hide this button if you only use essential cookies)</li>
    <li><strong>Learn more link</strong> — Link to your privacy policy or cookie policy page</li>
    <li><strong>Banner position</strong> — Bottom bar or bottom-right popup</li>
    <li><strong>Color theme</strong> — Light or dark, or customize to match your branding</li>
  </ul>
</li>
<li>Click <strong>Save</strong></li>
</ol>

<h2>What Cookies FinalDoc Uses</h2>
<p>FinalDoc's knowledge base uses a small number of cookies:</p>
<ul>
<li><strong>Session cookie</strong> — Keeps the reader logged in (essential — cannot be declined)</li>
<li><strong>Theme preference</strong> — Remembers dark/light mode preference (functional — can be declined)</li>
<li><strong>Continue Reading</strong> — Stored in localStorage (not a cookie, no consent needed)</li>
<li><strong>Analytics</strong> — If you have connected Google Analytics or similar, their cookies apply. These require consent</li>
</ul>

<h2>After a Reader Consents</h2>
<p>When a reader clicks Accept, their consent is stored in localStorage. The banner does not appear again for that reader on that device for the duration configured in settings (default: 365 days).</p>
<p>When they click Decline, non-essential cookies and tracking scripts are not loaded for that session.</p>

<h2>Compliance Notes</h2>
<div style="border-left: 4px solid #f59e0b; border-radius: 8px; padding: 16px; margin: 16px 0; background: rgba(245,158,11,0.08);">
<strong>Note:</strong> FinalDoc's cookie consent feature provides the UI mechanism for gathering consent. Actual legal compliance depends on your specific situation, jurisdiction, and how cookies are used on your site. Consult a legal professional for specific compliance requirements.
</div>