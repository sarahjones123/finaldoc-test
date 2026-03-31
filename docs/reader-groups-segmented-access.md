---
title: "Reader Groups & Segmented Access"
description: ""
slug: "reader-groups-segmented-access"
status: "PUBLISHED"
createdAt: "2026-02-24T08:32:54.663Z"
updatedAt: "2026-03-12T10:22:53.687Z"
---

<h1>Reader Groups and Segmented Access</h1>
<p>Reader Groups let you create different tiers of access for different types of readers. Instead of giving all logged-in readers access to the same content, you can segment your audience — Enterprise customers see one set of articles, Partners see another, Beta Testers see a third. This is ideal for multi-tier products or when you have customer-only, partner-only, or internal documentation living in the same knowledge base.</p>

<h2>Opening Reader Groups</h2>
<ol>
<li>Go to <strong>Settings</strong> in the left sidebar</li>
<li>Click <strong>Security &amp; Access → Reader Groups &amp; Segmented Access</strong></li>
</ol>

<h2>Creating a Reader Group</h2>
<ol>
<li>Click <strong>+ New Group</strong></li>
<li>Enter a group name (e.g., "Enterprise Customers", "Partners", "Beta Users", "Internal Team")</li>
<li>Optionally add a description to help teammates understand who belongs in this group</li>
<li>Click <strong>Save</strong></li>
</ol>

<h2>Assigning Readers to Groups</h2>

<h3>Manual Assignment</h3>
<ol>
<li>Go to <strong>Settings → Security &amp; Access → Reader Management</strong></li>
<li>Find the reader in the list</li>
<li>Click their email to open their profile</li>
<li>Under <strong>Groups</strong>, click <strong>Add to Group</strong></li>
<li>Select the group(s) they should belong to</li>
<li>Click <strong>Save</strong></li>
</ol>
<p>Or: When inviting a new reader, assign them to a group during the invitation flow.</p>

<h3>Auto-Assignment by Email Domain</h3>
<p>You can automatically add readers to a group based on their email domain — useful if Enterprise customers all have @enterprise-client.com emails:</p>
<ol>
<li>Open the group's settings</li>
<li>Find <strong>Auto-assign by email domain</strong></li>
<li>Enter the email domain(s) (e.g., <code>enterprise-client.com</code>)</li>
<li>Save</li>
</ol>
<p>Any reader who registers or is invited with a matching email domain is automatically added to this group.</p>

<h2>Restricting Content to Groups</h2>
<p>After creating groups, restrict specific categories or articles so only certain groups can see them:</p>
<ol>
<li>Go to <strong>Settings → Security &amp; Access → Content Access &amp; Mixed Visibility</strong></li>
<li>Find the category or article you want to restrict</li>
<li>Click <strong>Restrict Access</strong></li>
<li>Select which group(s) should be able to access this content</li>
<li>Click <strong>Save</strong></li>
</ol>
<p>Readers not in the specified group(s) will see the content as locked or not see it at all — depending on your Mixed Visibility configuration. Logged-in readers who don't have access see an "Unauthorized" message.</p>

<h2>How It Works for Readers</h2>
<ul>
<li>A reader in the "Enterprise" group can see Enterprise-only articles as well as all public articles</li>
<li>A reader in no group can only see content with no group restrictions (or public content, if your KB is Mixed visibility)</li>
<li>A reader can belong to multiple groups — they see all content accessible to any of their groups</li>
</ul>

<h2>Viewing Group Members</h2>
<ol>
<li>Click any group name in the Reader Groups list</li>
<li>You'll see all readers currently in that group with their email, join date, and last login</li>
<li>Click <strong>Remove</strong> to take a reader out of the group (this removes their access to group-restricted content)</li>
</ol>

<h2>Use Cases</h2>
<ul>
<li><strong>Customer tiers</strong>: Free, Pro, and Enterprise customers each see relevant documentation without overlap</li>
<li><strong>Beta program</strong>: Beta testers can see pre-release feature docs that aren't public yet</li>
<li><strong>Partner portal</strong>: Partners see co-branded and partner-specific integration guides</li>
<li><strong>Internal + external</strong>: Your team uses the same KB for internal SOPs (restricted to "Internal" group) and external customer help docs (public)</li>
</ul>