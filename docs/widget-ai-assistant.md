---
title: "Widget AI Assistant"
description: "Enable Ved AI within the widget for intelligent article search and answers."
slug: "widget-ai-assistant"
status: "PUBLISHED"
createdAt: "2026-02-24T03:51:04.098Z"
updatedAt: "2026-03-27T10:59:45.725Z"
---

<h1>Widget AI Assistant</h1>
<p>The Widget AI Assistant is the conversational AI chatbot embedded inside the FinalDoc help widget. When a reader opens the widget on your website and can't find what they need through search, they can chat with the AI — which answers their questions using your knowledge base content as its source of truth.</p>

<h2>How the Widget AI Works</h2>
<ol>
<li>Reader opens the widget on your website</li>
<li>Reader types a question in the chat tab</li>
<li>FinalDoc searches your KB using semantic (vector) search to find the most relevant articles</li>
<li>The AI uses those articles as context to compose a direct, accurate answer</li>
<li>The answer appears in the chat with links to the source articles</li>
</ol>
<p>The AI is grounded in your actual documentation — it does not make things up or answer from general knowledge. If your KB doesn't cover a topic, the AI says so and offers to connect the reader with your team.</p>

<h2>Enabling the AI Assistant in the Widget</h2>
<ol>
<li>Click <strong>External Widget</strong> in the left sidebar</li>
<li>Open your widget configuration</li>
<li>Go to the <strong>Content</strong> tab</li>
<li>Enable <strong>Show AI Assistant (Chat)</strong></li>
<li>Click <strong>Save</strong></li>
</ol>

<h2>Widget AI vs. KB AI Chatbot</h2>
<p>The <strong>Widget AI</strong> appears on your website inside the widget. The <strong>KB AI Chatbot</strong> (Ved AI) appears on your FinalDoc public knowledge base. They use the same AI engine but appear in different places:</p>
<ul>
<li>Widget AI → embedded on your website/app, seen by all site visitors</li>
<li>KB Chatbot → only on your KB (yourproject.finaldoc.io), seen by people already reading docs</li>
</ul>

<h2>Configuring the AI Persona</h2>
<p>In <strong>External Widget → Content → AI Assistant Settings</strong>:</p>
<ul>
<li><strong>AI Name</strong> — Name displayed in the chat header (e.g., "Aria", "Max", "Docs Assistant")</li>
<li><strong>Greeting message</strong> — What the AI says when the chat tab opens (e.g., "Hi! Ask me anything about [Product].")</li>
<li><strong>Fallback message</strong> — What the AI says when it can't find an answer in the KB (e.g., "I'm sorry, I don't have information about that. Would you like to contact our team?")</li>
</ul>

<h2>Knowledge Sources</h2>
<p>The Widget AI searches:</p>
<ul>
<li>All published articles in your knowledge base workspace(s) linked to this widget</li>
<li>Any site content you've added via Widget Site Content configuration</li>
</ul>
<p>To improve AI answer quality, ensure your articles are well-written, have clear headings, and are embedded (Settings → AI → AI Training → Embed All Articles).</p>

<h2>Conversation History</h2>
<p>Widget AI conversations are stored in your FinalDoc database and viewable in <strong>Analytics → Reader Analytics</strong> — select a reader and their chat history appears. Conversations are anonymous if the reader isn't logged in.</p>