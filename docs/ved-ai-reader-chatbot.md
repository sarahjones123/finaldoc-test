---
title: "Ved AI Reader Chatbot"
description: "AI-powered chatbot for your public knowledge base that helps readers find answers."
slug: "ved-ai-reader-chatbot"
status: "PUBLISHED"
createdAt: "2026-02-23T18:27:02.557Z"
updatedAt: "2026-03-12T13:27:44.965Z"
---

<h1>Ved AI Reader Chatbot</h1>
<p>The Ved AI chatbot is a floating AI assistant on your public knowledge base. Readers click the button in the corner of your KB to open a chat — they type their question and the AI answers using content from your articles, knowledge base Q&amp;A pairs, and your configured style guide. No waiting for a human, no digging through pages — instant answers.</p>

<h2>Enabling the Chatbot</h2>
<ol>
<li>Go to <strong>Settings → AI (Ved AI) → Reader Chatbot</strong></li>
<li>Toggle <strong>Enable Ved AI Chatbot</strong> to ON</li>
<li>The chat button immediately appears on your public knowledge base</li>
</ol>

<h2>How It Answers Questions</h2>
<p>When a reader asks a question, the AI:</p>
<ol>
<li>Searches your knowledge base using semantic vector search to find the most relevant articles and sections</li>
<li>Checks your AI training data (Q&amp;A pairs) for direct answers</li>
<li>Constructs a response using the found content, following your configured style guide</li>
<li>Returns an answer with links to the source articles so readers can dive deeper</li>
</ol>
<p>The AI is grounded in your documentation — it does not make things up or go off-topic. If it cannot find relevant content, it says so and suggests the reader contact support.</p>

<h2>Chatbot Appearance</h2>
<p>Customize the chatbot in <strong>Settings → Appearance → Ved AI Chatbot Customization</strong>:</p>
<ul>
<li><strong>Bot name</strong> — What the chatbot calls itself (default: "AI Assistant" — you can rename it to "Ada", "Max", "Help Bot", etc.)</li>
<li><strong>Bot avatar</strong> — Upload a custom avatar image or use the default AI icon</li>
<li><strong>Greeting message</strong> — The first message shown when the chat opens (e.g., "Hi! I am [name]. What can I help you with today?")</li>
<li><strong>Button style</strong> — Classic round button or Capsule (split Voice/Chat pill)</li>
<li><strong>Button position</strong> — Bottom-right (default) or bottom-left</li>
<li><strong>Color</strong> — Follows your brand accent color set in Design Studio</li>
</ul>

<h2>Voice Mode</h2>
<p>If you use the Capsule button style, readers can switch between Chat (text) and Voice modes:</p>
<ul>
<li><strong>Chat mode</strong> — Standard text-based conversation</li>
<li><strong>Voice mode</strong> — Real-time voice conversation with the AI using OpenAI's Realtime API. The reader speaks, the AI listens and responds in natural speech</li>
</ul>
<p>Configure voice in <strong>Settings → AI (Ved AI) → Reader Chatbot → Voice Settings</strong>:</p>
<ul>
<li>Choose a voice: shimmer, alloy, echo, coral, sage, ash</li>
<li>Preview each voice before selecting</li>
<li>Enable/disable voice mode independently from chat mode</li>
</ul>

<h2>Smart Search Suggestions</h2>
<p>The chatbot also integrates with KB search — when a reader types a search query and the AI detects a question, it shows a "Looking for X? Ask me!" prompt on the chatbot bubble. Readers can click it to instantly send the query to the AI.</p>

<h2>Conversation History</h2>
<p>All conversations are logged and visible in <strong>Feedback → AI Queries</strong>. Review what readers are asking, how the AI responded, and whether readers found the answers helpful.</p>

<h2>Disabling the Chatbot</h2>
<ol>
<li>Go to <strong>Settings → AI (Ved AI) → Reader Chatbot</strong></li>
<li>Toggle <strong>Enable Ved AI Chatbot</strong> to OFF</li>
<li>The chat button disappears from your KB immediately</li>
</ol>