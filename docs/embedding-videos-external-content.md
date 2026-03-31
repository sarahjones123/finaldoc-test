---
title: "Embedding Videos & External Content"
description: "How to embed YouTube, Vimeo, iframes, and other external content into articles."
slug: "embedding-videos-external-content"
status: "PUBLISHED"
createdAt: "2026-02-24T05:03:37.333Z"
updatedAt: "2026-03-19T16:00:05.626Z"
---

<h1>Embedding Videos &amp; External Content</h1>
<p>FinalDoc's article editor supports embedding videos and other rich media content from external platforms — YouTube, Vimeo, Loom, and more. You can also embed interactive content like CodePen, Google Slides, Figma, and other iFrame-compatible tools. This section explains how.</p>

<h2>Embedding a YouTube or Vimeo Video</h2>
<ol>
<li>Open an article in the editor</li>
<li>Place your cursor where you want the video to appear</li>
<li>Click the <strong>Insert</strong> menu in the toolbar → <strong>Video Embed</strong></li>
<li>Paste the YouTube or Vimeo URL (e.g., <code>https://www.youtube.com/watch?v=abc123</code>)</li>
<li>Click <strong>Embed</strong></li>
<li>The video appears inline in the editor as a playable embed</li>
</ol>

<h2>Embedding a Loom Recording</h2>
<ol>
<li>In Loom, copy the share URL for your recording</li>
<li>In the FinalDoc editor, click Insert → Video Embed</li>
<li>Paste the Loom URL</li>
<li>Click <strong>Embed</strong></li>
</ol>
<p>Loom recordings embed with the Loom player, including the viewer name and profile.</p>

<h2>Embedding an iFrame (Advanced)</h2>
<p>For platforms that don't have a native embed shortcut (CodePen, Figma, Google Slides, etc.):</p>
<ol>
<li>Get the embed code from the platform (usually a snippet that starts with <code>&lt;iframe</code>)</li>
<li>In the FinalDoc editor, click Insert → <strong>Embed Code</strong> (or <strong>HTML Block</strong>)</li>
<li>Paste the iFrame HTML</li>
<li>Click <strong>Save</strong></li>
</ol>
<p>FinalDoc sanitizes iFrame embeds for security — certain attributes are allowed, others are stripped. Embedded iFrames must use HTTPS.</p>

<h2>Embedding from Drive (Uploaded Videos)</h2>
<p>If you've uploaded an MP4 video to FinalDoc Drive:</p>
<ol>
<li>In the editor, click Insert → <strong>File from Drive</strong></li>
<li>Browse to and select your video file</li>
<li>Click <strong>Insert as Video Player</strong></li>
<li>The video appears with a native HTML5 video player (play/pause, volume, fullscreen)</li>
</ol>

<h2>Video Display Options</h2>
<p>After inserting a video embed, click on it to open its settings:</p>
<ul>
<li><strong>Width</strong> — Full width (fills column), fixed pixel width, or percentage</li>
<li><strong>Caption</strong> — Optional caption text below the video</li>
<li><strong>Autoplay</strong> — Autoplay when the page loads (not recommended — intrusive)</li>
<li><strong>Show controls</strong> — Show/hide the player controls bar</li>
</ul>

<h2>Video Best Practices</h2>
<ul>
<li>Keep embedded videos short (under 5 minutes) — long videos in help articles have low completion rates</li>
<li>Always include a written summary below the video — some readers prefer text, and text is indexed by search engines while video content is not</li>
<li>Use captions/subtitles for accessibility</li>
<li>If embedding from YouTube, use "youtube-nocookie.com" URLs to avoid tracking readers who haven't consented to YouTube cookies</li>
</ul>