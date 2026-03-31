---
title: "App Screen Capture for Videos"
description: ""
slug: "video-app-screen-capture"
status: "PUBLISHED"
createdAt: "2026-02-26T16:41:05.584Z"
updatedAt: "2026-03-27T12:25:46.441Z"
---

<h1>App Screen Capture for Videos</h1>
<p>FinalDoc's Video Studio can automatically take live screenshots of your web application during video generation. When a scene's narration describes a specific UI screen (e.g., "Navigate to Settings → Notifications"), the video generator opens your app in a headless browser, navigates there, and captures a real screenshot — giving your video authentic, up-to-date visuals of your actual product UI.</p>

<h2>How App Screen Capture Works</h2>
<ol>
<li>During video generation, the AI identifies which scenes reference specific pages or features in your app</li>
<li>For each such scene, the system launches a headless Chrome browser</li>
<li>It logs into your app using the URL and credentials you've configured</li>
<li>The AI uses multi-strategy navigation to reach the right screen: it first tries to navigate directly to a known URL, then falls back to clicking menus and links intelligently based on the narration</li>
<li>A screenshot is captured at the correct screen</li>
<li>That screenshot becomes the visual for the scene in the video</li>
</ol>

<h2>Configuring App Screen Capture</h2>
<ol>
<li>Click <strong>Video Studio</strong> (under <strong>AI Studio</strong> in the sidebar) in the left sidebar</li>
<li>Click <strong>Video Studio</strong></li>
<li>Click the <strong>gear icon</strong> in the Video Studio toolbar</li>
<li>Find <strong>App Screen Capture</strong></li>
<li>Enter the following:</li>
</ol>
<ul>
<li><strong>App URL</strong> — The base URL of your application (e.g., <code>https://app.yourproduct.com</code>)</li>
<li><strong>Login email</strong> — An email for a dedicated demo/test account</li>
<li><strong>Login password</strong> — The password for that test account</li>
<li><strong>Login page URL</strong> — Where the login form is (e.g., <code>https://app.yourproduct.com/login</code>)</li>
</ul>
<ol start="6">
<li>Click <strong>Save &amp; Test</strong> — FinalDoc verifies it can log in and take a screenshot</li>
<li>If the test is successful, you'll see a thumbnail of your app's logged-in state</li>
</ol>

<h2>Security Recommendations</h2>
<p>Create a dedicated demo account in your app specifically for App Screen Capture:</p>
<ul>
<li>Use an email like <code>finaldoc-demo@yourcompany.com</code></li>
<li>Give it admin-level or appropriate access so it can navigate to all screens you want to show</li>
<li>Populate it with realistic demo data so screenshots look like a real user's account</li>
<li>Do not use a real employee's credentials or an account with access to sensitive production data</li>
</ul>

<h2>Navigation Strategies</h2>
<p>The video generator uses multiple strategies to navigate to the right screen:</p>
<ol>
<li><strong>Direct URL navigation</strong> — If the AI identifies a specific URL from the narration, it navigates there directly (fastest and most reliable)</li>
<li><strong>Click navigation</strong> — The AI clicks menus, links, and buttons in sequence based on the narration's described path</li>
<li><strong>Fallback</strong> — If navigation fails, the scene falls back to an AI-generated diagram instead of an app screenshot</li>
</ol>

<h2>When App Screenshots Are Used</h2>
<p>App Screen Capture only activates when:</p>
<ul>
<li>It is configured with valid credentials</li>
<li>The AI determines a scene should show your UI (based on the narration content)</li>
<li>The scene's visual type is set to <strong>App Screenshot</strong> or <strong>App Annotated</strong></li>
</ul>
<p>For Article-to-Video, the AI automatically selects App Screenshot for scenes that describe product UI. For scenes that are more conceptual (definitions, background, etc.), it uses other visual types like Text Points or Diagram.</p>

<h2>App Annotated Screenshots</h2>
<p>The <strong>App Annotated</strong> scene type takes the same screenshot but adds AI-generated annotations — arrows, callout boxes, and highlight circles that draw attention to specific UI elements mentioned in the narration. This is particularly useful for instructional videos where you want to point readers to "click this button" or "find this menu item".</p>

<h2>Supported App Types</h2>
<p>App Screen Capture works with any modern web application that:</p>
<ul>
<li>Has a login page with email + password</li>
<li>Runs in a standard web browser (not a native desktop or mobile app)</li>
<li>Is accessible from FinalDoc's servers (not behind an IP allowlist or firewall)</li>
</ul>
<p>It does NOT work with apps that require:</p>
<ul>
<li>OAuth-only or SSO-only login (no email/password option)</li>
<li>Two-factor authentication (2FA) on every login</li>
<li>IP allowlist restrictions that don't include FinalDoc's infrastructure</li>
<li>Desktop (Windows/Mac) or mobile native apps</li>
</ul>

<h2>Troubleshooting</h2>
<ul>
<li><strong>Test fails immediately</strong> — Double-check your login URL, email, and password. Make sure the account doesn't have 2FA enabled</li>
<li><strong>Logged in but wrong screen captured</strong> — The AI couldn't navigate to the target screen. Try using more explicit navigation in your article text (e.g., "Go to Settings → Notifications" is clearer than "go to notifications")</li>
<li><strong>Screenshots look different from what readers see</strong> — The headless browser viewport is 1440×900. If your app is responsive, it may look slightly different. Test your app at that resolution</li>
<li><strong>Screenshots are outdated</strong> — Regenerate the video to capture fresh screenshots of your current UI</li>
</ul>