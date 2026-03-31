---
title: "Reading Progress & Continue Reading"
description: "Automatically save reader scroll position and show a Continue Reading section on the homepage."
slug: "reading-progress-continue-reading"
status: "PUBLISHED"
createdAt: "2026-02-27T10:22:40.929Z"
updatedAt: "2026-03-20T20:14:11.306Z"
---

<h1>Reading Progress and Continue Reading</h1>
<p>FinalDoc includes two features that help readers track their place in your knowledge base: the <strong>Reading Progress Bar</strong> (shows how far through a single article the reader has scrolled) and the <strong>Continue Reading</strong> feature (remembers the last article a reader was on and offers to pick up where they left off).</p>

<h2>Reading Progress Bar</h2>
<p>A thin bar at the very top of each article page (above the header) that fills as the reader scrolls down. When the reader reaches the bottom of the article, the bar is completely filled.</p>

<h3>What It Does</h3>
<ul>
<li>Gives readers a visual indication of how long the article is</li>
<li>Shows their current progress through the article</li>
<li>Helps with long articles — readers can see how much more they have to read</li>
</ul>

<h3>Enabling/Disabling</h3>
<ol>
<li>Go to <strong>Settings → Appearance → Article Display</strong></li>
<li>Find <strong>Show Reading Progress Bar</strong></li>
<li>Toggle it ON or OFF</li>
</ol>
<p>Enabled by default. Most readers find it helpful.</p>

<h2>Continue Reading</h2>
<p>When a reader visits your KB after a previous session, FinalDoc shows a "Continue reading from where you left off" prompt at the top of the homepage. Clicking it takes the reader directly to the last article they were reading.</p>

<h3>How It Works</h3>
<ul>
<li>FinalDoc stores the reader's last visited article URL in their browser's local storage</li>
<li>On their next visit to the KB homepage, FinalDoc checks for this stored URL</li>
<li>If found, shows the "Continue Reading" prompt with the article title</li>
<li>Clicking the prompt takes them directly to that article</li>
<li>The feature works for anonymous readers — no login required</li>
</ul>

<h3>Privacy</h3>
<p>Continue Reading data is stored entirely in the reader's own browser (localStorage). FinalDoc does not send or store this data on the server. It is not visible to you as the KB owner.</p>

<h3>Enabling/Disabling</h3>
<ol>
<li>Go to <strong>Settings → Appearance → Portal Builder → Homepage</strong></li>
<li>Find <strong>Show Continue Reading</strong></li>
<li>Toggle it ON or OFF</li>
</ol>

<h2>Scroll Memory</h2>
<p>Related to reading progress, FinalDoc also remembers a reader's scroll position on an article. If a reader scrolls halfway through a long article, closes the tab, and comes back to the same article URL later, the page automatically scrolls back to approximately where they left off. This uses sessionStorage and only works within the same browser session.</p>