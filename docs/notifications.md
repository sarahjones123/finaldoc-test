---
title: "Notifications"
description: "Configuring email and in-app notification channels."
slug: "notifications"
status: "PUBLISHED"
createdAt: "2026-02-23T18:16:12.080Z"
updatedAt: "2026-03-21T03:04:41.702Z"
---

<h1>Notifications</h1>
<p>FinalDoc can send you notifications when important things happen in your knowledge base — new feedback submitted, articles awaiting review, team member activity, and more. Configure your notification preferences in Settings.</p>

<h2>Opening Notification Settings</h2>
<ol>
<li>Go to <strong>Settings → General → Notifications</strong></li>
</ol>

<h2>Personal Notification Preferences</h2>
<p>These settings control what emails <em>you</em> personally receive. Each team member can configure their own preferences independently.</p>

<h3>Email Notification Types</h3>
<table>
<thead><tr><th>Notification</th><th>When It's Sent</th></tr></thead>
<tbody>
<tr><td><strong>New feedback (negative)</strong></td><td>A reader submits a thumbs-down on any article</td></tr>
<tr><td><strong>New feedback (all)</strong></td><td>Any feedback submitted (positive or negative)</td></tr>
<tr><td><strong>Article awaiting review</strong></td><td>A review reminder is due for an article</td></tr>
<tr><td><strong>Approval request</strong></td><td>An article is submitted for your approval in a workflow</td></tr>
<tr><td><strong>Article approved or rejected</strong></td><td>A decision is made on an article you submitted for approval</td></tr>
<tr><td><strong>New comment on article</strong></td><td>Someone posts a comment on any article you author or watch</td></tr>
<tr><td><strong>@mention</strong></td><td>You are @mentioned in a comment</td></tr>
<tr><td><strong>New team member</strong></td><td>Someone accepts a team invitation</td></tr>
<tr><td><strong>Reader registered</strong></td><td>A new reader creates an account on your KB</td></tr>
<tr><td><strong>Weekly digest</strong></td><td>Weekly summary of KB activity (sent every Monday)</td></tr>
</tbody>
</table>

<h3>Digest Mode</h3>
<p>For high-volume events like "New feedback — all," enable <strong>Digest Mode</strong> to receive a single daily summary email instead of a separate notification for each event. Digest emails are sent at 9am in your project's configured timezone.</p>

<h2>In-App Notifications</h2>
<p>In-app notifications appear via the bell icon (🔔) in the header. They show for events specifically involving you:</p>
<ul>
<li>@mentions in comments or articles</li>
<li>Approval requests assigned to you</li>
<li>Replies to your comments</li>
<li>Assigned tasks</li>
</ul>
<p>In-app notifications are always active and cannot be disabled.</p>

<h2>Notification Channels (Slack, Teams)</h2>
<p>To receive notifications in Slack or Microsoft Teams, you need to connect those channels. These are project-wide notification channels configured by Admins and Owners:</p>
<ol>
<li>Go to <strong>Settings → General → Notification Channels</strong></li>
<li>Click <strong>Connect Slack</strong> or configure a <strong>Microsoft Teams</strong> webhook URL</li>
<li>Choose which events trigger channel notifications</li>
<li>Click <strong>Save</strong></li>
</ol>
<p>See the <strong>Notification Channels</strong> article for full Slack and Teams setup instructions.</p>

<h2>Turning Off All Email Notifications</h2>
<p>In your Notifications settings, turn off all individual notification toggles, or click <strong>Unsubscribe from all</strong> at the bottom of the page. You will still receive security-related emails (password resets, new device sign-in alerts) regardless of this setting.</p>