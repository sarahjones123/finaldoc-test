---
title: "AI Agent (OpenClaw)"
description: "Connect your knowledge base to WhatsApp, Telegram, Slack, Discord, and Teams using the AI Agent."
slug: "ai-agent-openclaw"
status: "PUBLISHED"
createdAt: "2026-03-12T08:32:59.231Z"
updatedAt: "2026-03-26T19:01:38.960Z"
---

<h1>AI Agent (OpenClaw)</h1>
<p>OpenClaw is FinalDoc's AI agent service that lets your knowledge base answer questions automatically on messaging platforms — WhatsApp, Telegram, Slack, Discord, Microsoft Teams, and web chat. Readers send messages on any of these channels and the AI responds using your KB articles. No human required.</p>

<h2>What OpenClaw Does</h2>
<ul>
<li>Reads incoming messages from your connected channels</li>
<li>Searches your KB articles to find the best answer using RAG (retrieval-augmented generation)</li>
<li>Sends a conversational AI response back to the user on that same channel</li>
<li>Keeps conversation history so follow-up questions make sense in context</li>
</ul>
<p>Think of it as your knowledge base coming to life as a live chatbot on any messaging platform your team or customers already use.</p>

<h2>Opening Agent Settings</h2>
<ol>
<li>Go to <strong>Settings</strong> in the sidebar</li>
<li>Under <strong>Integrations</strong>, click <strong>Chat &amp; Support</strong></li>
<li>Click <strong>Configure</strong> on the AI Agent (OpenClaw) card at the top of the page</li>
</ol>

<h2>Provisioning the Agent</h2>
<p>Before you can connect any channels, you need to provision (activate) the OpenClaw agent for your project:</p>
<ol>
<li>On the Agent Settings page, you'll see a "Not yet provisioned" state</li>
<li>Click <strong>Provision Agent</strong></li>
<li>FinalDoc spins up a dedicated agent container for your project (this takes 30–60 seconds)</li>
<li>Once provisioned, the status shows <strong>Active</strong> (green dot)</li>
</ol>
<p>Provisioning is a one-time step. After that, the agent runs 24/7 unless you manually put it to sleep.</p>

<h2>Agent Status</h2>
<p>The Overview tab shows the current agent status:</p>
<ul>
<li><strong>Active</strong> (green) — Agent is running and processing messages</li>
<li><strong>Sleeping</strong> (amber) — Agent is paused to save resources. Messages are not processed while sleeping. Wake it up manually when needed</li>
<li><strong>Provisioning</strong> (blue) — Agent is being set up</li>
<li><strong>Error</strong> (red) — Agent encountered a problem. The error message is shown. Try waking/restarting or contact support</li>
</ul>

<h2>Agent Tabs</h2>
<p>The Agent Settings page has four tabs:</p>
<ul>
<li><strong>Overview</strong> — Agent status, total message count, last active time, and quick actions (Sleep, Wake, Deprovision)</li>
<li><strong>Channels</strong> — Connect and manage messaging platform integrations</li>
<li><strong>Conversations</strong> — View recent conversations across all channels</li>
<li><strong>Usage</strong> — Message counts broken down by channel, and overall usage statistics</li>
</ul>

<h2>Connecting Channels</h2>
<p>Go to the <strong>Channels</strong> tab to connect messaging platforms:</p>

<h3>WhatsApp</h3>
<p>Connect your WhatsApp number by scanning a QR code:</p>
<ol>
<li>Click <strong>Connect WhatsApp</strong></li>
<li>A QR code appears in the control panel</li>
<li>Open WhatsApp on your phone → Settings → Linked Devices → Link a Device</li>
<li>Scan the QR code</li>
<li>The connection is established and the status updates to "Connected"</li>
</ol>

<h3>Telegram</h3>
<ol>
<li>Create a bot by messaging @BotFather on Telegram → /newbot</li>
<li>Copy the bot token BotFather gives you</li>
<li>Click <strong>Connect Telegram</strong> in FinalDoc</li>
<li>Paste the <strong>Bot Token</strong> and save</li>
</ol>

<h3>Slack</h3>
<ol>
<li>Create a Slack app at api.slack.com and install it to your workspace</li>
<li>Get the <strong>Bot OAuth Token</strong> (starts with <code>xoxb-</code>) and the <strong>App-Level Token</strong> (starts with <code>xapp-</code>)</li>
<li>Click <strong>Connect Slack</strong> in FinalDoc</li>
<li>Paste both tokens and save</li>
</ol>

<h3>Discord</h3>
<ol>
<li>Create a Discord application at discord.com/developers</li>
<li>Add a bot to the application and copy the <strong>Bot Token</strong></li>
<li>Invite the bot to your server with the correct permissions</li>
<li>Click <strong>Connect Discord</strong> in FinalDoc and paste the Bot Token</li>
</ol>

<h3>Microsoft Teams</h3>
<ol>
<li>Create an incoming webhook in your Teams channel</li>
<li>Copy the <strong>Webhook URL</strong></li>
<li>Click <strong>Connect Microsoft Teams</strong> in FinalDoc and paste the URL</li>
</ol>

<h3>WebChat</h3>
<p>Embed the agent as a chat widget on any website:</p>
<ol>
<li>Click <strong>Connect WebChat</strong></li>
<li>Enter the <strong>Allowed Origins</strong> (domains where the widget will be embedded, e.g., <code>https://yourcompany.com</code>)</li>
<li>Save — you'll get an embed snippet to add to your site</li>
</ol>

<h2>Sleeping and Waking the Agent</h2>
<ul>
<li><strong>Sleep</strong>: Click <strong>Sleep Agent</strong> to pause the agent. Use this to save resources when you don't need it running 24/7. Messages received while sleeping are not processed</li>
<li><strong>Wake</strong>: Click <strong>Wake Agent</strong> to restart a sleeping agent. It comes back online in a few seconds</li>
</ul>

<h2>Viewing Conversations</h2>
<p>The <strong>Conversations</strong> tab shows recent incoming messages across all channels. Each conversation shows:</p>
<ul>
<li>Channel type (WhatsApp, Telegram, etc.)</li>
<li>User name (as reported by the platform)</li>
<li>Last message preview</li>
<li>Timestamp (how long ago)</li>
</ul>

<h2>Usage Stats</h2>
<p>The <strong>Usage</strong> tab shows total message counts and a breakdown by channel. Use this to see which platforms your users prefer and how active the agent is.</p>

<h2>Deprovisioning</h2>
<p>To permanently remove the agent, click <strong>Deprovision Agent</strong> in the Overview tab and confirm. This deletes the agent container and disconnects all channels. This cannot be undone — you'd need to provision a fresh agent if you want it back.</p>

<h2>How the AI Answers Questions</h2>
<p>OpenClaw uses the same RAG (retrieval-augmented generation) system as FinalDoc's web chatbot:</p>
<ol>
<li>The user's question is converted to a semantic embedding</li>
<li>FinalDoc searches your article embeddings for the most relevant content</li>
<li>The top matching article content is passed to the AI model as context</li>
<li>The AI generates a conversational answer based on your documentation</li>
</ol>
<p>To improve answer quality, make sure your articles are published and that AI embeddings are up to date (Settings → AI → AI Training).</p>