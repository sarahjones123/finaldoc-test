---
title: "Video Branding & Export"
description: ""
slug: "video-branding-export"
status: "PUBLISHED"
createdAt: "2026-02-26T16:41:05.588Z"
updatedAt: "2026-03-27T12:25:46.429Z"
---

<h1>Video Branding &amp; Export</h1>
<p>FinalDoc lets you apply your brand identity to every video and export finished videos to external platforms like YouTube and Vimeo. This article covers how to set up video branding and how to export your completed videos.</p>

<h2>Opening Video Settings</h2>
<ol>
<li>Go to <strong>Video Studio (AI Studio section in the sidebar)</strong></li>
<li>Click the <strong>gear icon</strong> in the Video Studio toolbar (top-right of the Video Manager)</li>
</ol>

<h2>Video Branding</h2>
<p>Branding settings control how your videos look — the intro card, outro card, and on-screen identity elements.</p>

<h3>Logo</h3>
<p>Upload your company logo (PNG or SVG, transparent background recommended). The logo appears on:</p>
<ul>
<li>The Title Card scene (intro)</li>
<li>The Outro scene (end card)</li>
<li>Optionally as a watermark in the corner of every scene</li>
</ul>

<h3>Brand Colors</h3>
<p>Set the primary and secondary colors for your videos. These are applied to:</p>
<ul>
<li>Title Card and Outro backgrounds</li>
<li>Text Points bullets and accents</li>
<li>Callout box backgrounds</li>
<li>Section divider color bars</li>
</ul>
<p>Enter hex codes (e.g., <code>#7C3AED</code>) or use the color picker. These default to your Portal Builder brand colors, but you can override them specifically for videos.</p>

<h3>Tagline</h3>
<p>A short text that appears on the Outro scene (e.g., "Trusted by 10,000+ teams" or "Visit docs.yourcompany.com"). Keep it under 80 characters.</p>

<h3>Intro/Outro Toggle</h3>
<p>You can disable the auto-generated intro or outro scenes entirely if you prefer to start and end the video without branded cards.</p>

<h2>App Screen Capture Credentials</h2>
<p>For App Screenshot and App Annotated scene types, FinalDoc needs to be able to access and screenshot your web app. Configure this in the Video Settings under <strong>App Screen Capture</strong>:</p>
<ul>
<li><strong>App URL</strong> — Base URL of your application (e.g., <code>https://app.yourproduct.com</code>)</li>
<li><strong>Login email and password</strong> — Credentials for a test account FinalDoc uses to log in</li>
<li><strong>Login URL</strong> — URL of your login page (if different from the app URL)</li>
</ul>
<p>FinalDoc uses a headless browser to log in and capture screenshots. The credentials are stored encrypted and only used for screenshot capture. See the App Screen Capture article for full setup details.</p>

<h2>Default Quality Preferences</h2>
<p>Set the default quality settings that apply to all new videos:</p>
<ul>
<li><strong>Resolution</strong> — 1080p (Full HD) or 720p (HD)</li>
<li><strong>Frame rate</strong> — 30fps (standard) or 24fps (cinematic)</li>
<li><strong>Audio bitrate</strong> — Higher bitrate = better audio quality but larger file size</li>
</ul>

<h2>YouTube Export</h2>
<p>Connect your YouTube channel to upload completed videos directly from FinalDoc:</p>
<ol>
<li>In Video Settings, click <strong>Connect YouTube</strong></li>
<li>Sign in to your Google account and grant FinalDoc access to your YouTube channel</li>
<li>Once connected, your channel name appears as "Connected"</li>
</ol>
<p>To export a video to YouTube:</p>
<ol>
<li>In the Video Manager, hover over the completed video</li>
<li>Click the <strong>Export</strong> button (or the ... menu → Export to YouTube)</li>
<li>Set the title, description, tags, and privacy setting (Public, Unlisted, or Private)</li>
<li>Click <strong>Upload to YouTube</strong></li>
<li>FinalDoc uploads the video in the background — a notification appears when done</li>
</ol>

<h2>Vimeo Export</h2>
<p>Connect your Vimeo account similarly:</p>
<ol>
<li>In Video Settings, click <strong>Connect Vimeo</strong></li>
<li>Authorize FinalDoc with your Vimeo account</li>
<li>Once connected, export videos via the <strong>Export → Export to Vimeo</strong> option</li>
<li>Set title, description, and privacy (Anyone, Only me, or Password-protected)</li>
</ol>

<h2>Downloading Videos</h2>
<p>You can download videos without connecting any external platform:</p>
<ul>
<li><strong>Download MP4</strong> — Click the <strong>Download</strong> button on any completed video card to download just the MP4 file</li>
<li><strong>Download Bundle</strong> — Downloads a ZIP file containing the MP4 video, all individual scene frame images (PNG), and the SRT subtitle file. Useful if you want to re-edit in another video editor like Premiere Pro, Final Cut, or DaVinci Resolve</li>
</ul>

<h2>Embedding Videos in Your KB</h2>
<p>After generating or downloading a video, you can embed it directly in your documentation articles. See the Embedding Videos article for full instructions on embedding YouTube, Vimeo, and uploaded video files in articles.</p>