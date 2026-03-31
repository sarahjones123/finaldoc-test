---
title: "Custom Domain"
description: "Connecting your own domain to your FinalDoc knowledge base."
slug: "custom-domain"
status: "PUBLISHED"
createdAt: "2026-02-23T18:16:21.278Z"
updatedAt: "2026-03-12T08:58:51.330Z"
---

<h1>Custom Domain</h1>
<p>By default, your knowledge base is accessible at <code>yourproject.finaldoc.io</code>. You can replace this with your own domain — for example, <code>docs.yourcompany.com</code> or <code>help.yourcompany.com</code>. This gives your KB a professional look that matches your brand.</p>

<h2>Opening Custom Domain Settings</h2>
<ol>
<li>Go to <strong>Settings</strong> in the left sidebar</li>
<li>Click <strong>Domain &amp; SEO</strong> → <strong>Custom Domain</strong></li>
</ol>

<h2>Step 1: Enter Your Domain</h2>
<ol>
<li>In the Custom Domain field, enter the subdomain you want to use (e.g., <code>docs.yourcompany.com</code>)</li>
<li>Click <strong>Add Domain</strong></li>
</ol>

<h2>Step 2: Verify Domain Ownership (DNS TXT Record)</h2>
<p>FinalDoc needs to verify that you own the domain before issuing an SSL certificate.</p>
<ol>
<li>After adding the domain, FinalDoc shows you a <strong>TXT record</strong> to add to your DNS</li>
<li>Log in to your domain registrar (e.g., Cloudflare, GoDaddy, Namecheap, AWS Route 53)</li>
<li>Add the TXT record to your domain's DNS settings:
  <ul>
    <li><strong>Type</strong>: TXT</li>
    <li><strong>Name/Host</strong>: The subdomain or @ (as shown by FinalDoc)</li>
    <li><strong>Value</strong>: The verification string FinalDoc provides</li>
  </ul>
</li>
<li>DNS changes can take a few minutes to an hour to propagate</li>
<li>Click <strong>Verify DNS</strong> in FinalDoc once you have added the record</li>
</ol>

<h2>Step 3: Point Your Domain to FinalDoc</h2>
<p>After verification, point your subdomain to FinalDoc's servers:</p>
<ol>
<li>In your DNS settings, add a <strong>CNAME record</strong>:
  <ul>
    <li><strong>Type</strong>: CNAME</li>
    <li><strong>Name/Host</strong>: Your subdomain (e.g., <code>docs</code>)</li>
    <li><strong>Value</strong>: <code>app.finaldoc.io</code></li>
  </ul>
</li>
<li>Wait for DNS propagation (a few minutes to a few hours)</li>
<li>Click <strong>Activate Domain</strong> in FinalDoc</li>
</ol>

<h2>Step 4: SSL Certificate</h2>
<p>FinalDoc automatically provisions a free SSL certificate for your custom domain using Let's Encrypt. HTTPS is enabled automatically — you do not need to do anything. This usually completes within a few minutes of domain activation.</p>

<h2>After Activation</h2>
<p>Once active:</p>
<ul>
<li>Your KB is accessible at both <code>yourproject.finaldoc.io</code> and your custom domain</li>
<li>The custom domain is the primary URL shown to readers</li>
<li>The FinalDoc subdomain redirects to your custom domain automatically</li>
</ul>

<h2>Removing a Custom Domain</h2>
<ol>
<li>Go to <strong>Settings → Domain &amp; SEO → Custom Domain</strong></li>
<li>Click <strong>Remove Domain</strong></li>
<li>The domain is deactivated and the SSL certificate is revoked</li>
<li>Your KB returns to being accessible only at its FinalDoc subdomain</li>
</ol>

<div style="border-left: 4px solid #f59e0b; border-radius: 8px; padding: 16px; margin: 16px 0; background: rgba(245,158,11,0.08);">
<strong>Note:</strong> It is not possible to use an apex/root domain (e.g., <code>yourcompany.com</code>) — you must use a subdomain (e.g., <code>docs.yourcompany.com</code>). This is a DNS requirement for CNAME records.
</div>

<h2>Troubleshooting</h2>
<ul>
<li><strong>SSL error after activation</strong> — Wait 10–15 minutes for the certificate to provision. If it persists, contact support</li>
<li><strong>Domain not found</strong> — Check your CNAME record is correct and has propagated (use a tool like dnschecker.org to verify)</li>
<li><strong>Verification fails</strong> — Make sure the TXT record is exactly as shown, and that enough time has passed for DNS propagation</li>
</ul>