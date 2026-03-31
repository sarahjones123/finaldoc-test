---
title: "Troubleshooting Integrations"
description: "Common integration issues and how to resolve them."
slug: "troubleshooting-integrations"
status: "PUBLISHED"
createdAt: "2026-02-24T05:03:43.627Z"
updatedAt: "2026-03-27T10:59:45.799Z"
---

<h1>Troubleshooting Integrations</h1>
<p>FinalDoc integrates with many external services — Slack, Microsoft Teams, Zendesk, webhooks, custom analytics, SSO, and more. Integration issues are usually caused by incorrect credentials, network restrictions, or configuration mismatches. This guide covers common integration problems and how to fix them.</p>

<h2>Webhook Issues</h2>

<h3>Webhook Not Receiving Events</h3>
<ol>
<li>Go to <strong>Settings → Integrations → Automation &amp; Subscriptions</strong></li>
<li>Click on the webhook → <strong>Delivery Logs</strong></li>
<li>Look at recent delivery attempts — were they successful (2xx) or failing (4xx/5xx/timeout)?</li>
</ol>
<p>Common causes:</p>
<ul>
<li><strong>Server not running</strong> — Your webhook endpoint URL is down. Verify the server is running and publicly accessible</li>
<li><strong>Firewall blocking FinalDoc</strong> — Your server firewall is blocking FinalDoc's IP. Temporarily whitelist all IPs to test, then restrict to FinalDoc's IP ranges</li>
<li><strong>Wrong URL</strong> — Check the webhook URL for typos. It must be an HTTPS URL (not HTTP)</li>
<li><strong>SSL certificate error</strong> — Your server's SSL certificate is expired or self-signed. FinalDoc requires valid SSL</li>
</ul>

<h3>Webhook Signature Verification Failing</h3>
<p>If your server is receiving webhooks but rejecting them:</p>
<ul>
<li>Double-check that your webhook secret in FinalDoc matches the secret your server uses for HMAC verification</li>
<li>Ensure you're verifying the raw request body (before JSON parsing) against the signature</li>
<li>Check that you're using HMAC-SHA256, not SHA1 or MD5</li>
</ul>

<h2>Microsoft Teams Integration Issues</h2>

<h3>Bot Not Responding to @mentions</h3>
<ol>
<li>Verify the Teams webhook URL in <strong>Settings → Integrations → Microsoft Teams</strong> is correct and not expired</li>
<li>In Teams, check the channel where FinalDoc is configured — type @FinalDoc and see if it shows up</li>
<li>Re-generate the webhook URL from Teams (Apps → FinalDoc → Configure) and update it in FinalDoc settings</li>
</ol>

<h2>SAML/SSO Issues</h2>

<h3>SSO Login Redirects to Error Page</h3>
<ul>
<li>Check that the ACS URL in your identity provider exactly matches the one in FinalDoc's SSO settings</li>
<li>Verify the X.509 certificate hasn't expired</li>
<li>Ensure the Name ID format is set to "Email Address" in your IdP</li>
<li>Test the SSO connection using the <strong>Test SSO</strong> button before enabling it for all users</li>
</ul>

<h2>Slack Notifications Not Working</h2>
<ol>
<li>Go to <strong>Settings → Integrations → Chat & Support</strong></li>
<li>Click the Slack connection → <strong>Test Connection</strong></li>
<li>If the test fails: the Slack token may have been revoked. Disconnect and reconnect Slack</li>
<li>If the test succeeds but you're still not getting notifications: check notification settings in <strong>Settings → General → Notifications</strong> to ensure the correct notification types are enabled for Slack</li>
</ol>

<h2>Third-Party Analytics Not Tracking</h2>
<ul>
<li>Verify the Measurement ID or token in <strong>Settings → Integrations → Analytics</strong> is correct</li>
<li>Check browser developer tools → Network tab while visiting your KB. Look for requests to analytics.google.com, mixpanel.com, etc.</li>
<li>Ad blockers commonly block analytics — test in incognito mode</li>
<li>GA4 data has a 24–48 hour delay — events sent today may not appear in GA4 reports until tomorrow</li>
</ul>

<h2>Getting More Help</h2>
<p>For integration issues not covered here, contact support@finaldoc.io with the integration name, the error you're seeing, and any relevant logs from your end. Include the webhook delivery logs screenshot from FinalDoc if relevant.</p>