---
title: "SAML/SSO Configuration"
description: "Set up Single Sign-On with SAML for enterprise team authentication."
slug: "saml-sso-configuration"
status: "PUBLISHED"
createdAt: "2026-02-23T18:27:10.227Z"
updatedAt: "2026-03-17T04:43:39.904Z"
---

<h1>SAML/SSO Configuration</h1>
<p>FinalDoc supports Single Sign-On (SSO) via SAML 2.0. When SSO is configured, your readers log in using their existing identity provider account (Google Workspace, Microsoft Azure AD, Okta, etc.) — no separate FinalDoc password required. This is a requirement for many enterprise organizations.</p>

<h2>Opening SSO Configuration</h2>
<ol>
<li>Go to <strong>Settings → Security &amp; Access → SAML/SSO Configuration</strong></li>
</ol>

<h2>How SAML SSO Works</h2>
<ol>
<li>Reader visits your knowledge base and clicks "Login"</li>
<li>FinalDoc redirects them to your identity provider's login page</li>
<li>Reader logs in with their corporate credentials</li>
<li>The identity provider sends a SAML assertion back to FinalDoc confirming the reader's identity</li>
<li>FinalDoc logs the reader in automatically based on the assertion</li>
<li>First-time readers are auto-provisioned a reader account in FinalDoc</li>
</ol>

<h2>Configuration Steps</h2>

<h3>Step 1: Get FinalDoc's Service Provider (SP) Details</h3>
<p>In FinalDoc's SAML settings, you will see:</p>
<ul>
<li><strong>SP Entity ID</strong> — A unique identifier for FinalDoc as the service provider</li>
<li><strong>ACS URL (Assertion Consumer Service URL)</strong> — Where your identity provider sends SAML responses</li>
</ul>
<p>Copy these — you need them when configuring your identity provider.</p>

<h3>Step 2: Configure Your Identity Provider</h3>
<p>In your identity provider (Okta, Azure AD, Google Workspace, etc.):</p>
<ol>
<li>Create a new SAML application</li>
<li>Enter the FinalDoc SP Entity ID and ACS URL from Step 1</li>
<li>Set the Name ID format to "Email Address"</li>
<li>Map the following attributes:
  <ul>
    <li>Email → the reader's email address</li>
    <li>First name (optional) → for display in FinalDoc</li>
    <li>Last name (optional)</li>
  </ul>
</li>
<li>Save the application</li>
<li>Download or copy the <strong>IdP Metadata XML</strong> or collect the <strong>IdP Entity ID</strong>, <strong>IdP SSO URL</strong>, and <strong>X.509 Certificate</strong></li>
</ol>

<h3>Step 3: Enter IdP Details in FinalDoc</h3>
<ol>
<li>Back in FinalDoc, paste your identity provider's details:
  <ul>
    <li>Identity Provider Entity ID</li>
    <li>Identity Provider SSO URL</li>
    <li>X.509 Certificate (the public cert from your IdP)</li>
  </ul>
</li>
<li>Click <strong>Save SAML Configuration</strong></li>
</ol>

<h3>Step 4: Test and Enable</h3>
<ol>
<li>Click <strong>Test SSO</strong> to verify the configuration works</li>
<li>A test login flow opens — complete it with an identity provider account</li>
<li>If successful, click <strong>Enable SSO</strong></li>
</ol>

<h2>SSO for Team Members vs. Readers</h2>
<p>FinalDoc SAML SSO is configured separately for:</p>
<ul>
<li><strong>Readers</strong> — Configured in Settings → Security &amp; Access → SAML/SSO Configuration (the one described here)</li>
<li><strong>Team members</strong> — Team member SSO is a separate enterprise configuration. Contact support for team member SSO setup</li>
</ul>

<h2>Availability</h2>
<p>SAML/SSO is available on <strong>Enterprise plans</strong> only. Contact sales if you need SSO on a lower plan.</p>