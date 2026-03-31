---
title: "Notification Channels"
description: "Configure email, Slack, and webhook notifications for your documentation events."
slug: "notification-channels"
status: "PUBLISHED"
createdAt: "2026-02-24T03:51:20.996Z"
updatedAt: "2026-03-21T03:04:42.400Z"
---

<h1>Notification Channels</h1>
<p>FinalDoc can send notifications to your team when important things happen in your knowledge base. You can receive notifications via email, Slack, and Microsoft Teams. Configure which channels are active and what events trigger notifications in Settings.</p>

<h2>Opening Notification Channels</h2>
<ol>
<li>Go to <strong>Settings</strong></li>
<li>Click <strong>General → Notification Channels</strong></li>
</ol>

<h2>Available Channels</h2>

<h3>Email (Default)</h3>
<p>Email is the default channel and requires no additional setup. Notifications are sent to each team member's account email address. To configure which email events are active, see <strong>Settings → General → Notifications</strong> where you can toggle individual notification types on or off and choose Digest vs. Instant delivery.</p>

<h3>Slack</h3>
<p>Connect Slack to receive notifications posted to a Slack channel:</p>
<ol>
<li>In Notification Channels, find <strong>Slack</strong></li>
<li>Click <strong>Connect Slack</strong></li>
<li>You are redirected to Slack's OAuth page — log in and select your workspace and the channel where notifications should be posted</li>
<li>Authorize FinalDoc to post messages</li>
<li>You are redirected back to FinalDoc with Slack connected</li>
<li>Choose which events trigger Slack notifications (see list below)</li>
<li>Click <strong>Save</strong></li>
<li>Click <strong>Send Test Message</strong> to verify — a test notification is posted to the configured channel</li>
</ol>

<h3>Microsoft Teams</h3>
<p>For notification alerts in a Teams channel:</p>
<ol>
<li>In your Microsoft Teams, go to the channel where you want notifications</li>
<li>Click the + icon → <strong>Connectors → Incoming Webhook</strong></li>
<li>Create the webhook and copy the Webhook URL</li>
<li>In FinalDoc → Notification Channels → Microsoft Teams, paste the webhook URL</li>
<li>Configure which events trigger Teams notifications</li>
<li>Click <strong>Save</strong></li>
</ol>
<p>Note: The Teams Outgoing Webhook (for AI Q&amp;A) is a separate integration from Teams notifications. See the Microsoft Teams Integration article for the AI Q&amp;A setup.</p>

<h3>In-App Notifications</h3>
<p>FinalDoc also shows in-app notifications via the bell icon in the header. These appear for events that specifically involve you — @mentions, approval requests, and items assigned to you. In-app notifications are always active and cannot be disabled.</p>

<h2>Available Notification Events</h2>
<p>You can choose which of these events trigger notifications on each channel:</p>
<table>
<thead><tr><th>Event</th><th>Triggered When</th></tr></thead>
<tbody>
<tr><td>New reader feedback (negative)</td><td>A reader submits a thumbs-down on any article</td></tr>
<tr><td>New reader feedback (all)</td><td>Any feedback submitted (positive or negative)</td></tr>
<tr><td>Article awaiting review</td><td>A review reminder is due for an article</td></tr>
<tr><td>Approval request</td><td>An article is submitted for approval in the workflow</td></tr>
<tr><td>Article approved or rejected</td><td>An approval decision is made on your article</td></tr>
<tr><td>New comment on article</td><td>Someone posts a comment on an article</td></tr>
<tr><td>@mention</td><td>You are @mentioned in a comment or article</td></tr>
<tr><td>New team member</td><td>Someone accepts a team invitation</td></tr>
<tr><td>Reader registered</td><td>A new reader creates an account on your KB</td></tr>
<tr><td>Feedback score alert</td><td>An article's feedback score drops below your threshold</td></tr>
<tr><td>AI training complete</td><td>Bulk embedding or training finishes</td></tr>
<tr><td>Backup complete</td><td>An automated backup finishes successfully</td></tr>
<tr><td>Weekly digest</td><td>Weekly summary of KB activity (every Monday 9am)</td></tr>
</tbody>
</table>

<h2>Digest Mode</h2>
<p>For high-volume notification types (like "New feedback — all"), enable <strong>Digest Mode</strong> instead of individual notifications. Digest mode sends a single daily summary email at 9am instead of a separate notification for each event. This prevents inbox overload on active knowledge bases.</p>

<h2>Per-User vs. Project-Wide Notifications</h2>
<ul>
<li><strong>Project-wide notifications</strong> (Slack, Teams) — Configured by Admins and Owners. Go to the same channel for all configured events regardless of who caused the event</li>
<li><strong>Personal email notifications</strong> — Each team member can configure their own personal notification preferences by clicking their avatar → Notification Preferences. Only affects their own email inbox</li>
</ul>