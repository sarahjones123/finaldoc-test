---
title: "Frequently Asked Questions"
description: "Answers to the most common questions about FinalDoc."
slug: "frequently-asked-questions"
status: "PUBLISHED"
createdAt: "2026-02-23T18:16:45.687Z"
updatedAt: "2026-03-27T10:59:45.743Z"
---

<h1>Frequently Asked Questions</h1>
<p>Answers to the most common questions about FinalDoc.</p>

<h2>Getting Started</h2>

<h3>Is FinalDoc free?</h3>
<p>Yes, FinalDoc has a free plan that lets you create a knowledge base with unlimited articles and readers. Paid plans unlock additional features like custom domains, advanced analytics, AI training, more storage, video generation, and priority support. See <strong>Settings → Billing</strong> for current plan details.</p>

<h3>What is the difference between a Project and a Workspace?</h3>
<p>A <strong>Project</strong> is your top-level knowledge base — it has one public URL, one set of readers, and one team. A <strong>Workspace</strong> is a version of your knowledge base within a project. By default, every project has one workspace. You can create multiple workspaces to have separate content for different audiences (e.g., v1 docs and v2 docs) under the same project.</p>

<h3>Can I have multiple knowledge bases?</h3>
<p>Yes. Each project is a separate knowledge base. You can create as many projects as your plan allows. Switch between projects using the project selector at the top of the sidebar.</p>

<h3>How do I invite team members?</h3>
<p>Go to <strong>Settings → Security &amp; Access → Team Management</strong> and click <strong>Invite Member</strong>. Enter their email, assign a role, and they'll receive an invitation email. Roles include OWNER, ADMIN, EDITOR, AUTHOR, and VIEWER.</p>

<h2>Articles and Content</h2>

<h3>Is there a limit on the number of articles?</h3>
<p>No. All plans, including the free plan, support unlimited articles.</p>

<h3>Can I import content from another platform?</h3>
<p>Yes. FinalDoc can import from Confluence, Zendesk, Notion, Docusaurus, GitBook, plain Markdown files, HTML, Word documents (.docx), and DITA XML. Go to <strong>Toolbox → Import / Export</strong> to import.</p>

<h3>How do I move articles between categories?</h3>
<p>In the Documentation editor, right-click the article in the left panel (or click the ⋮ menu) and select <strong>Move to Category</strong>. You can also drag and drop articles within the article tree.</p>

<h3>What happens to deleted articles?</h3>
<p>Deleted articles go to the <strong>Recycle Bin</strong> (accessible from the Documentation sidebar) where they stay for 30 days before being permanently deleted. You can restore an article from the Recycle Bin at any time during this window.</p>

<h3>Can articles be scheduled to publish automatically?</h3>
<p>Yes. Open an article's Properties panel (right side of the editor), find the <strong>Publish</strong> section, and set a scheduled publish date and time. The article will automatically become Published at that time.</p>

<h2>Public Knowledge Base</h2>

<h3>What URL does my knowledge base have?</h3>
<p>Every project gets a free subdomain at <code>{yoursubdomain}.finaldoc.io</code>. You can also set up a custom domain (e.g., <code>docs.yourcompany.com</code>) in <strong>Settings → Domain &amp; SEO → Custom Domain</strong>.</p>

<h3>Can readers log in to see private content?</h3>
<p>Yes. Enable reader authentication in <strong>Settings → Security &amp; Access → Site Visibility</strong>. Readers create accounts (or are invited) and log in to access content. You can also mix public and private articles using Mixed Visibility mode.</p>

<h3>Can I add a chatbot to my knowledge base?</h3>
<p>Yes. The Ved AI chatbot is built into every FinalDoc knowledge base. Enable and customize it in <strong>Settings → AI (Ved AI) → AI Configuration</strong>. Readers can ask questions and the AI answers using your articles.</p>

<h3>Can readers leave feedback on articles?</h3>
<p>Yes. Enable article ratings in <strong>Settings → Appearance → Portal Builder</strong>. Readers can give a thumbs up/down and leave comments. View all feedback in the <strong>Feedback</strong> section.</p>

<h2>AI Features</h2>

<h3>What AI features does FinalDoc include?</h3>
<p>FinalDoc includes:</p>
<ul>
<li><strong>Ved AI Writer</strong> — AI writing assistant in the editor</li>
<li><strong>AI Optimizer</strong> — Quality check and improvement suggestions for articles</li>
<li><strong>AI Auto-Draft</strong> — Generate draft articles from a topic</li>
<li><strong>AI Translation</strong> — One-click article translation into 100+ languages</li>
<li><strong>Ved AI Chatbot</strong> — AI assistant on your public KB that answers reader questions</li>
<li><strong>Voice Mode</strong> — Voice conversation with the AI assistant</li>
<li><strong>Video Studio</strong> — Convert articles to professional videos</li>
<li><strong>Smart Linking</strong> — AI suggests related articles to link</li>
<li><strong>Ticket Analysis</strong> — AI analysis of your support tickets to find content gaps</li>
<li><strong>OpenClaw Agent</strong> — AI chatbot for WhatsApp, Telegram, Slack, Discord, Teams, and WebChat</li>
</ul>

<h3>Does FinalDoc use my content to train AI models?</h3>
<p>No. FinalDoc does not use your knowledge base content to train any AI models. See <strong>Settings → AI (Ved AI) → AI Compliance &amp; Data Handling</strong> for details about how AI features process your content.</p>

<h3>Can I bring my own OpenAI API key?</h3>
<p>Yes. BYOK (Bring Your Own Key) is supported for OpenAI, Anthropic, Azure OpenAI, and Google AI. Go to <strong>Settings → AI (Ved AI) → API Keys (BYOK)</strong>.</p>

<h2>Billing and Plans</h2>

<h3>How do I upgrade my plan?</h3>
<p>Go to <strong>Settings → Billing</strong>. Click <strong>Upgrade Plan</strong> to see available plans and pricing. You can upgrade at any time and the change takes effect immediately.</p>

<h3>Can I cancel my subscription?</h3>
<p>Yes. Go to <strong>Settings → Billing</strong> and click <strong>Cancel Subscription</strong>. Your account moves to the free plan at the end of your current billing period. Your content is not deleted.</p>

<h3>Does FinalDoc offer discounts for nonprofits or startups?</h3>
<p>Contact support at support@finaldoc.io for information about special pricing for nonprofits, open-source projects, and early-stage startups.</p>

<h2>Technical</h2>

<h3>Can I export my content if I leave FinalDoc?</h3>
<p>Yes. Go to <strong>Toolbox → Import &amp; Export</strong> to export your entire knowledge base as Markdown, HTML, or JSON. You own your data and can export it at any time.</p>

<h3>Is there an API?</h3>
<p>Yes. FinalDoc has a full REST API. See <strong>Settings → Data &amp; Compliance → API Tokens</strong> to create API keys, and <strong>API Docs</strong> (in the sidebar) to generate and browse API reference documentation for your project.</p>

<h3>Can I embed the knowledge base in my product?</h3>
<p>Yes — two ways: (1) The <strong>Help Widget</strong> is an embeddable JS widget that adds an AI-powered help button to your website or product. Configure it in <strong>External Widget</strong>. (2) You can also use the public KB's URL directly in an iframe.</p>

<h3>Does FinalDoc have a mobile app?</h3>
<p>No native mobile app, but FinalDoc's admin panel works in mobile browsers. The public knowledge base is a Progressive Web App (PWA) — readers can install it on their phone's home screen for an app-like experience.</p>

<h3>What browsers does FinalDoc support?</h3>
<p>Chrome, Firefox, Edge, and Safari (latest versions). Chrome is recommended for the best editor experience. Internet Explorer is not supported.</p>

<h3>Is there a dark mode?</h3>
<p>Yes. Click your profile avatar in the top-right → <strong>Theme</strong> to switch between light and dark mode. The setting is saved per account and applies across all your projects.</p>