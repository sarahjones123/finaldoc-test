---
title: "Video Editor"
description: ""
slug: "video-editor"
status: "PUBLISHED"
createdAt: "2026-02-26T16:41:05.580Z"
updatedAt: "2026-03-21T05:59:19.832Z"
---

<h1>Video Editor (NLE)</h1>
<p>After generating a video, you can open the built-in Non-Linear Editor (NLE) to customize every aspect of the video — reorder scenes, change visuals, edit narration, adjust transitions, add motion effects, upload custom frames or audio, and add background music. Click any video card in Video Studio to open it.</p>

<h2>Editor Layout</h2>

<h3>Preview Panel (Center)</h3>
<p>Shows the current scene's visual at full size. Controls below the preview:</p>
<ul>
<li><strong>Play/Pause</strong> — Preview the current scene or the full video</li>
<li><strong>Skip back/forward</strong> — Jump between scenes</li>
<li><strong>Fullscreen</strong> — Watch in fullscreen mode</li>
<li><strong>Scene counter</strong> — "Scene 3 of 12"</li>
</ul>

<h3>Scene Timeline (Bottom Strip)</h3>
<p>A horizontal row of scene thumbnails showing all scenes in order. Each thumbnail shows:</p>
<ul>
<li>Scene number and duration in seconds</li>
<li>Visual type icon (article image, app screenshot, animated, etc.)</li>
<li>Quality score dot — green (70+), yellow (40–69), red (below 40)</li>
</ul>
<p>Click any thumbnail to jump to that scene. Drag left/right to reorder scenes.</p>

<h3>Inspector Panel (Right)</h3>
<p>Shows properties and controls for the currently selected scene. This is where you make edits.</p>

<h2>Scene Visual Types</h2>
<p>Each scene has a visual type — the kind of graphic shown while the narrator speaks. FinalDoc supports 15 visual types:</p>
<table>
<thead><tr><th>Type</th><th>Description</th></tr></thead>
<tbody>
<tr><td><strong>Title Card</strong></td><td>Branded title card with text (used for intro/section titles)</td></tr>
<tr><td><strong>Article Image</strong></td><td>An image directly embedded in the source article</td></tr>
<tr><td><strong>App Screenshot</strong></td><td>Live screenshot of your web app at a specific URL (requires App Screen Capture setup)</td></tr>
<tr><td><strong>App Annotated</strong></td><td>App screenshot with AI-added annotations/callouts highlighting key UI elements</td></tr>
<tr><td><strong>Text Points</strong></td><td>Animated bullet-point list of key points from the narration</td></tr>
<tr><td><strong>Code</strong></td><td>Syntax-highlighted code block with typewriter animation</td></tr>
<tr><td><strong>Terminal</strong></td><td>Terminal/command-line style animation of commands</td></tr>
<tr><td><strong>Diagram/Image</strong></td><td>AI-generated diagram or illustration relevant to the narration</td></tr>
<tr><td><strong>Callout</strong></td><td>Highlighted callout box with key quote or important note</td></tr>
<tr><td><strong>Stats</strong></td><td>Animated statistics/numbers display</td></tr>
<tr><td><strong>Timeline</strong></td><td>Animated horizontal timeline of events or steps</td></tr>
<tr><td><strong>Quote</strong></td><td>Large styled quote card</td></tr>
<tr><td><strong>Compare</strong></td><td>Side-by-side comparison of two options</td></tr>
<tr><td><strong>Section</strong></td><td>Minimal section divider / transition slide</td></tr>
<tr><td><strong>Outro</strong></td><td>Branded outro card with CTA (call to action)</td></tr>
</tbody>
</table>
<p>To change a scene's visual type, select the scene and use the <strong>Visual Type</strong> dropdown in the Inspector.</p>

<h2>Motion Effects</h2>
<p>Add motion to a scene's visual (Ken Burns-style camera effects):</p>
<ul>
<li><strong>Subtle Zoom</strong> — Slow gentle zoom in over the scene duration</li>
<li><strong>Zoom In</strong> — More pronounced zoom toward center</li>
<li><strong>Zoom Out</strong> — Start close, pull back</li>
<li><strong>Pan Right</strong> — Camera pans from left to right</li>
<li><strong>Pan Left</strong> — Camera pans from right to left</li>
<li><strong>Pan Down</strong> — Camera pans downward</li>
<li><strong>Dolly In</strong> — Cinematic push in toward subject</li>
</ul>
<p>Select the effect from the <strong>Motion Effect</strong> dropdown in the Inspector panel for the selected scene.</p>

<h2>Transitions</h2>
<p>Control how one scene transitions to the next. Select from 15 options in the <strong>Transition</strong> dropdown:</p>
<ul>
<li><strong>Fade</strong> — Classic crossfade</li>
<li><strong>Fade Black</strong> — Fade to black then fade in</li>
<li><strong>Slow Fade</strong> — Longer crossfade</li>
<li><strong>Dissolve</strong> — Soft dissolve blend</li>
<li><strong>Slide Right / Slide Left</strong> — Slides next scene in from side</li>
<li><strong>Smooth Right / Smooth Left</strong> — Smoother slide variant</li>
<li><strong>Wipe Right</strong> — Hard wipe</li>
<li><strong>Circle</strong> — Iris/circle open</li>
<li><strong>Radial</strong> — Radial sweep</li>
<li><strong>Zoom In</strong> — Zooms into the next scene</li>
<li><strong>Split H</strong> — Horizontal split open</li>
<li><strong>Reveal Right</strong> — Reveal wipe</li>
<li><strong>None</strong> — Hard cut (instant switch)</li>
</ul>
<p>You can also set <strong>Transition Duration</strong> (in seconds) for each scene transition.</p>

<h2>Editing Narration</h2>
<ol>
<li>Select a scene in the timeline</li>
<li>In the Inspector, click the <strong>Narration</strong> text field</li>
<li>Edit the text</li>
<li>Click <strong>Regenerate Audio</strong> — the TTS voiceover regenerates for just this scene</li>
</ol>

<h2>Uploading Custom Frames</h2>
<p>Replace a scene's AI-generated visual with your own image:</p>
<ol>
<li>Select the scene</li>
<li>In the Inspector, click <strong>Upload Custom Frame</strong></li>
<li>Select an image file (JPG, PNG, WebP)</li>
<li>Your image replaces the AI-generated visual for this scene</li>
</ol>

<h2>Uploading Custom Audio</h2>
<p>Replace the AI voiceover for a scene with your own recorded audio:</p>
<ol>
<li>Select the scene</li>
<li>In the Inspector, click <strong>Upload Custom Audio</strong></li>
<li>Select an audio file (MP3, WAV)</li>
<li>Your audio replaces the TTS for this scene</li>
</ol>

<h2>Background Music</h2>
<p>Add background music that plays underneath the narration for the whole video:</p>
<ul>
<li><strong>From library</strong> — Browse FinalDoc's built-in music library. Click any track to preview and select</li>
<li><strong>Upload your own</strong> — Upload an MP3 or WAV file</li>
<li><strong>AI generated</strong> — Generate custom background music via AI</li>
<li><strong>Volume control</strong> — Adjust how loud the background music is relative to the narration (so narration is always audible)</li>
<li><strong>Remove music</strong> — Click the X to remove background music</li>
</ul>

<h2>Reassembling the Video</h2>
<p>After making edits (changing scenes, narration, transitions, music), click <strong>Reassemble Video</strong> in the editor toolbar. This rebuilds the full MP4 with all your changes applied. Reassembly takes 1–5 minutes.</p>

<h2>Downloading</h2>
<p>Click <strong>Download</strong> to download the video as an MP4 file. You can also click the <strong>Download Bundle</strong> option to download all scene frames + the SRT subtitle file as a ZIP.</p>