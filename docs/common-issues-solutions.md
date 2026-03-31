---
title: "Common Issues & Solutions"
description: "Solutions to frequently encountered problems."
slug: "common-issues-solutions"
status: "PUBLISHED"
createdAt: "2026-02-23T18:16:44.159Z"
updatedAt: "2026-03-21T03:04:45.646Z"
---

<h1>Common Issues and Solutions</h1>
<p>Stuck on something? Here are solutions to the most common problems FinalDoc users encounter.</p>

<h2>Login and Access</h2>

<h3>I forgot my password</h3>
<ol>
<li>Go to app.finaldoc.io</li>
<li>Click <strong>Forgot Password?</strong> below the login form</li>
<li>Enter your email address and click <strong>Send Reset Link</strong></li>
<li>Check your email (including spam) for a password reset link</li>
<li>Click the link and set a new password</li>
</ol>

<h3>I am not receiving emails from FinalDoc</h3>
<ul>
<li>Check your spam/junk folder — FinalDoc emails sometimes end up there</li>
<li>Add hello@finaldoc.io to your safe senders list</li>
<li>If your company uses strict email filtering, ask your IT department to whitelist the finaldoc.io domain</li>
</ul>

<h3>My team member cannot log in</h3>
<ul>
<li>Check that the invite email was sent (go to <strong>Settings → Security &amp; Access → Team Management</strong> and check the member's status)</li>
<li>If the invite shows as "Pending", resend it using the Resend Invite button</li>
<li>Invite links expire after 7 days — cancel the old invite and send a new one if expired</li>
</ul>

<h2>Editor Issues</h2>

<h3>My article content is not saving</h3>
<ul>
<li>Check your internet connection — autosave requires a live connection</li>
<li>Look for an error indicator near the top of the editor (a red "Failed to save" message)</li>
<li>Try pressing Ctrl+S / Cmd+S manually</li>
<li>If saving continues to fail, copy your content, reload the page, and paste it back</li>
</ul>

<h3>Images are not showing in my article</h3>
<ul>
<li>If you see a broken image icon, the image file may have been deleted from Drive — re-upload and re-insert it</li>
<li>If the image was uploaded to an external service (not Drive), check that the URL is still valid and publicly accessible</li>
<li>Very large images may fail to upload — compress them before uploading (recommended max: 5MB per image)</li>
</ul>

<h3>Copy-pasted content has weird formatting</h3>
<ul>
<li>Paste the content using <strong>Ctrl+Shift+V / Cmd+Shift+V</strong> (paste as plain text) to strip all formatting</li>
<li>Or paste normally and then use <strong>Clear Formatting</strong> (Ctrl+Shift+M) on the affected text</li>
<li>For content from Microsoft Word, some complex formatting (tables with merged cells, text boxes) may not convert cleanly — simplify in Word first</li>
</ul>

<h2>Public Knowledge Base</h2>

<h3>My published article is not showing on the public KB</h3>
<ul>
<li>Check the article status — it must be Published (green) not Draft</li>
<li>Check site visibility — if the KB is set to Private, readers must be logged in to see content</li>
<li>Check if the article's category is set to Private in Mixed Visibility settings</li>
<li>Hard refresh the KB page (Ctrl+Shift+R) to bypass browser cache</li>
</ul>

<h3>My custom domain shows an SSL error</h3>
<ul>
<li>SSL certificate provisioning can take 10–30 minutes after domain activation — wait and retry</li>
<li>Check that the CNAME record is pointing to app.finaldoc.io (not to an IP address)</li>
<li>Use dnschecker.org to verify the CNAME has propagated worldwide</li>
<li>If the issue persists more than an hour after setup, contact support</li>
</ul>

<h2>AI Features</h2>

<h3>The AI chatbot says "I don't have information about that" for everything</h3>
<ul>
<li>Your articles may not be embedded yet — go to <strong>Settings → AI (Ved AI) → AI Training</strong> and click <strong>Embed All Articles</strong></li>
<li>Check that you have published articles in your knowledge base (the AI cannot search draft articles)</li>
<li>Verify that AI is enabled in <strong>Settings → AI (Ved AI) → AI Configuration</strong></li>
</ul>

<h3>AI translation is not working</h3>
<ul>
<li>AI features require an active AI plan or an OpenAI API key configured in Settings</li>
<li>Very long articles may timeout — try translating shorter articles first</li>
<li>Check <strong>Settings → AI (Ved AI) → AI Configuration</strong> to make sure the AI service is connected</li>
</ul>

<h2>Getting More Help</h2>
<p>If the above solutions do not help, contact our support team:</p>
<ul>
<li><strong>Email</strong>: support@finaldoc.io</li>
<li><strong>In-app chat</strong>: Click the chat icon on the bottom-right of any page in the admin panel</li>
<li><strong>Response time</strong>: Business days, typically within 24 hours</li>
</ul>