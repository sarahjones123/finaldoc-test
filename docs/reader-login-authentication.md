---
title: "Reader Login & Authentication"
description: "How readers authenticate to access private or mixed-visibility knowledge base content."
slug: "reader-login-authentication"
status: "PUBLISHED"
createdAt: "2026-02-23T18:27:05.647Z"
updatedAt: "2026-03-12T13:27:54.089Z"
---

<h1>Reader Login and Authentication</h1>
<p>FinalDoc supports optional reader authentication — requiring visitors to log in before they can access your knowledge base content. You can also use <strong>Mixed Visibility</strong> to make some content public and other content private (login required).</p>

<h2>Site Visibility Options</h2>
<p>Configure visibility in <strong>Settings → Security &amp; Access → Site Visibility</strong>:</p>
<ul>
<li><strong>Public</strong> — Anyone can read all content. No login required. This is the default</li>
<li><strong>Private</strong> — All content requires reader login. Visitors who are not logged in see only the login page</li>
<li><strong>Mixed</strong> — Some content is public, some requires login. Configure which categories or articles are private in <strong>Settings → Security &amp; Access → Content Access &amp; Mixed Visibility</strong></li>
</ul>

<h2>Reader Accounts vs. Team Member Accounts</h2>
<p>FinalDoc has two separate types of accounts:</p>
<ul>
<li><strong>Team members</strong> — Your editors, authors, and admins. They log in to the admin panel at app.finaldoc.io</li>
<li><strong>Readers</strong> — Your customers or end users. They log in to the public knowledge base at your project URL. Readers cannot access the admin panel</li>
</ul>
<p>Reader accounts are managed separately — they do not share the team member login.</p>

<h2>How Readers Create Accounts</h2>
<p>Reader accounts are created in one of two ways:</p>
<ul>
<li><strong>Self-registration</strong> — Readers fill in the sign-up form on your KB login page (if you enable self-registration in Settings → Security &amp; Access → Reader Management)</li>
<li><strong>Admin invite</strong> — You invite readers manually from Settings → Security &amp; Access → Reader Management by entering their email address</li>
</ul>

<h2>The Reader Login Page</h2>
<p>The reader login page is separate from the admin login. It appears at your KB URL when a visitor tries to access private content. The login page:</p>
<ul>
<li>Shows your project logo and brand colors</li>
<li>Has fields for email and password</li>
<li>Has a "Forgot password?" link for self-service password reset</li>
<li>Has a "Create account" link (if self-registration is enabled)</li>
<li>Is fully customizable in <strong>Settings → Appearance → Portal Builder → Login Page</strong></li>
</ul>

<h2>Reader Groups and Segmented Access</h2>
<p>You can organize readers into groups and assign different content access permissions to each group. For example:</p>
<ul>
<li>Group "Customers" — Can access the main documentation</li>
<li>Group "Partners" — Can access documentation plus partner-only resources</li>
<li>Group "Beta Users" — Can access beta documentation that is not yet public</li>
</ul>
<p>Set this up in <strong>Settings → Security &amp; Access → Reader Groups &amp; Segmented Access</strong>.</p>

<h2>Managing Readers</h2>
<p>Go to <strong>Settings → Security &amp; Access → Reader Management</strong> to:</p>
<ul>
<li>See a list of all registered readers with their email, join date, and last login</li>
<li>Invite new readers by email</li>
<li>Remove a reader (blocks their access immediately)</li>
<li>Assign readers to groups</li>
<li>Reset a reader's password on their behalf</li>
<li>Enable or disable self-registration</li>
</ul>

<h2>Read Receipts</h2>
<p>When reader authentication is enabled, FinalDoc can track which articles each reader has read — showing you per-reader reading progress. Enable this in <strong>Settings → General → Read Receipts</strong>. Readers can opt out via their profile settings.</p>

<h2>SAML/SSO Integration</h2>
<p>If your organization uses Single Sign-On (SSO) via SAML 2.0 (e.g., Okta, Azure AD, Google Workspace), you can connect it so readers log in with their existing corporate accounts — no separate FinalDoc password required. Configure this in <strong>Settings → Security &amp; Access → SAML/SSO Configuration</strong>.</p>