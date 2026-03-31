---
title: "Video Generation"
description: ""
slug: "video-generation"
status: "PUBLISHED"
createdAt: "2026-02-26T16:41:05.564Z"
updatedAt: "2026-03-27T12:25:46.410Z"
---

<h1>Video Generation</h1>
<p>FinalDoc's Video Studio automatically converts your written documentation articles into professional video presentations. You can also generate videos from free-form text prompts. The AI writes a narration script, generates voiceover audio, creates or captures visual frames for each scene, and assembles everything into a polished MP4 video.</p>

<h2>Opening Video Studio</h2>
<ol>
<li>Click <strong>Video Studio</strong> (under <strong>AI Studio</strong> in the sidebar) in the left sidebar</li>
<li>Under <strong>AI Tools</strong>, click <strong>Video Studio</strong></li>
</ol>

<h2>Two Ways to Create a Video</h2>

<h3>Method 1: Article to Video</h3>
<p>Convert one or more existing KB articles into a video:</p>
<ol>
<li>Click <strong>+ Generate New Video</strong> (the big purple button)</li>
<li>Make sure <strong>Article</strong> mode is selected (not Text)</li>
<li>Work through the 3-step wizard (see below)</li>
</ol>

<h3>Method 2: Text to Video</h3>
<p>Generate a video from a free-form text prompt — no article needed:</p>
<ol>
<li>Click the dropdown arrow next to <strong>+ Generate New Video</strong></li>
<li>Select <strong>Generate from Text</strong></li>
<li>Enter a text prompt describing the video you want</li>
<li>Set duration, aspect ratio, and other settings</li>
<li>Click <strong>Generate</strong></li>
</ol>

<h2>The 3-Step Article Video Wizard</h2>

<h3>Step 1: Content</h3>
<ul>
<li><strong>Select articles</strong> — Browse and search your KB articles. Click to select one or multiple articles. The video will cover all selected articles in order</li>
<li><strong>Video title</strong> — Give the video a title (auto-filled from the first selected article's title)</li>
</ul>

<h3>Step 2: Style</h3>
<ul>
<li><strong>Length preset</strong> — Choose how long the video should be:
  <ul>
    <li>⚡ <strong>Clip</strong> — Under 60 seconds (very short, key points only)</li>
    <li>🎬 <strong>Short</strong> — 1–3 minutes (concise overview)</li>
    <li>🎥 <strong>Classic</strong> — 3–10 minutes (standard documentation video)</li>
    <li>📽️ <strong>Longform</strong> — Over 10 minutes (comprehensive deep dive)</li>
  </ul>
</li>
<li><strong>Aspect ratio</strong> — Choose the video's shape:
  <ul>
    <li><strong>16:9</strong> — Landscape (standard widescreen, good for YouTube, websites, presentations)</li>
    <li><strong>9:16</strong> — Portrait (vertical, good for TikTok, Instagram Reels, mobile)</li>
    <li><strong>1:1</strong> — Square (good for social media like Twitter/X, LinkedIn)</li>
  </ul>
</li>
</ul>

<h3>Step 3: Voice</h3>
<ul>
<li><strong>Voice selection</strong> — Choose from OpenAI's built-in voices:
  <ul>
    <li>🌟 <strong>Nova</strong> — Female, warm</li>
    <li>⚡ <strong>Alloy</strong> — Neutral, balanced</li>
    <li>🌊 <strong>Echo</strong> — Male, deep</li>
    <li>📖 <strong>Fable</strong> — British, expressive</li>
    <li>💎 <strong>Onyx</strong> — Male, authoritative</li>
    <li>✨ <strong>Shimmer</strong> — Female, bright</li>
  </ul>
  If you have ElevenLabs configured (see AI API Keys), additional premium voices appear here.</li>
<li><strong>Voice speed</strong> — Slide to adjust how fast the narrator speaks (default is 1.0x). Useful for complex topics (slow down) or short clips (speed up)</li>
<li><strong>Voice preview</strong> — Click the play button next to any voice to hear a sample before committing</li>
</ul>

<h2>Generation Stages</h2>
<p>After clicking Generate, the video card appears with a progress indicator:</p>
<table>
<thead><tr><th>Stage</th><th>What Happens</th></tr></thead>
<tbody>
<tr><td><strong>Waiting in queue</strong></td><td>Your job is queued — queue position is shown if there are others ahead</td></tr>
<tr><td><strong>Extracting content</strong></td><td>Article content is parsed and structured</td></tr>
<tr><td><strong>Generating script</strong></td><td>AI writes the narration script and scene plan</td></tr>
<tr><td><strong>Generating voiceover</strong></td><td>TTS audio is generated for each scene</td></tr>
<tr><td><strong>Rendering scenes</strong></td><td>Visual frames are created for each scene</td></tr>
<tr><td><strong>Scoring quality</strong></td><td>AI evaluates each scene's quality</td></tr>
<tr><td><strong>Assembling video</strong></td><td>Scenes, audio, transitions, and subtitles are combined</td></tr>
<tr><td><strong>Uploading</strong></td><td>Final MP4 is uploaded to storage</td></tr>
<tr><td><strong>Complete</strong></td><td>Video is ready to watch and download</td></tr>
</tbody>
</table>
<p>Generation typically takes 3–15 minutes depending on length preset and article complexity.</p>

<h2>Managing Videos</h2>
<p>All generated videos appear in the Video Manager grid. Each video card shows the thumbnail, title, duration, status badge, and action buttons: Play, Edit, Download, Delete.</p>

<h2>Bulk Delete</h2>
<ol>
<li>Click the <strong>Select</strong> button in the Video Manager toolbar</li>
<li>Check multiple video cards</li>
<li>Click <strong>Delete (N)</strong> in the bulk action bar</li>
<li>Confirm in the dialog</li>
</ol>

<h2>Video Settings</h2>
<p>Click the <strong>gear icon</strong> in the Video Studio toolbar to configure:</p>
<ul>
<li>Branding (logo, colors, tagline for intro/outro)</li>
<li>App Screen Capture credentials (for live app screenshots)</li>
<li>YouTube and Vimeo export connections</li>
<li>Default quality preferences</li>
</ul>