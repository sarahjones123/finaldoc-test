---
title: "Video Scene Types"
description: ""
slug: "video-scene-types"
status: "PUBLISHED"
createdAt: "2026-02-26T16:41:05.575Z"
updatedAt: "2026-03-19T16:00:08.089Z"
---

<h1>Video Scene Types</h1>
<p>Every scene in a FinalDoc video has a <strong>visual type</strong> — this is the kind of graphic or animation shown on screen while the narrator speaks. When you edit a video in the Video Editor (NLE), you can change any scene to any of the 15 available visual types. This article explains what each type looks like and when to use it.</p>

<h2>How to Change a Scene's Visual Type</h2>
<ol>
<li>Open the Video Editor by clicking any video in Video Studio</li>
<li>Click the scene you want to change in the timeline strip at the bottom</li>
<li>In the Inspector panel on the right, find the <strong>Visual Type</strong> dropdown</li>
<li>Select a new visual type from the list</li>
<li>The preview updates immediately to show the new type</li>
<li>Click <strong>Reassemble Video</strong> to rebuild the final video with your changes</li>
</ol>

<h2>All 15 Visual Types</h2>

<h3>1. Title Card</h3>
<p>A branded title card with large text — typically used for intro slides, section headers, or chapter dividers. Shows your video title and can include your logo or brand colors. Great for the first scene of any video or when transitioning between major topics.</p>

<h3>2. Article Image</h3>
<p>An image that was directly embedded in the source article. If your KB article has screenshots or diagrams, FinalDoc extracts them and uses them as visuals. This is the most "native" scene type — your actual documentation images appear in the video.</p>

<h3>3. App Screenshot</h3>
<p>A live screenshot of your web app at a specific URL, captured automatically during video generation. This requires App Screen Capture to be set up (see the App Screen Capture setup article). The screenshot shows your actual product UI at the URL you configured for this scene, giving viewers a real look at the product.</p>

<h3>4. App Annotated</h3>
<p>Same as App Screenshot, but with AI-added visual annotations — arrows, callout boxes, or highlight circles that draw attention to specific UI elements. Use this when you want to point out a specific button, menu item, or feature within the screenshot. Annotations are generated automatically based on what the narrator is describing.</p>

<h3>5. Text Points</h3>
<p>An animated bullet-point list of key takeaways from the narrator's script for this scene. The points appear one at a time as the narrator speaks. Ideal for scenes that cover a list of features, steps, or benefits — it helps viewers follow along with the spoken content.</p>

<h3>6. Code</h3>
<p>A syntax-highlighted code block with a typewriter animation — the code appears character by character as the narrator explains it. Supports multiple programming languages. Use this for developer documentation, API examples, or any scene where code is the main point.</p>

<h3>7. Terminal</h3>
<p>A terminal/command-line style animation showing commands being typed out in a dark terminal window with a blinking cursor. Perfect for CLI guides, installation instructions, or any step that requires running commands in a terminal.</p>

<h3>8. Diagram/Image</h3>
<p>An AI-generated diagram, illustration, or infographic that's relevant to what the narrator is saying. FinalDoc's AI creates a custom visual (using Gemini) based on the scene's narration text. Good for explaining concepts, architectures, flows, or anything that benefits from a diagram but where you don't have one ready.</p>

<h3>9. Callout</h3>
<p>A highlighted callout box displaying a key quote, important warning, or critical note from the narration. The text appears prominently against a colored background. Use for "Pro tip" moments, important warnings, or key facts you want viewers to remember.</p>

<h3>10. Stats</h3>
<p>An animated statistics display where numbers count up visually (e.g., "10,000+ users", "99.9% uptime"). Each number animates from zero to its final value. Use when your narration mentions impressive numbers or metrics that you want to emphasize visually.</p>

<h3>11. Timeline</h3>
<p>An animated horizontal timeline of events, steps, or milestones. Each item appears in sequence as the narrator mentions it. Great for explaining a process with multiple stages, a history of events, or a step-by-step workflow where order matters.</p>

<h3>12. Quote</h3>
<p>A large styled quote card — oversized text in quotation marks against a clean background. Use when the narration references an important quote, a testimonial, or a key statement you want to give visual weight to.</p>

<h3>13. Compare</h3>
<p>A side-by-side comparison of two options, showing their differences in two columns. Automatically extracts comparison data from the narration. Perfect for "Feature A vs. Feature B", "Before vs. After", or "Free vs. Paid" type explanations.</p>

<h3>14. Section</h3>
<p>A minimal section divider slide — a clean transition between major parts of the video. Usually shows a short section title against a simple background. Use between chapters or major topic changes to give viewers a visual pause and orientation cue.</p>

<h3>15. Outro</h3>
<p>A branded outro card shown at the end of the video, with a call-to-action (CTA) message (e.g., "Visit our docs", "Try it free", or "Contact support"). Includes your branding colors and can be customized in Video Settings → Branding.</p>

<h2>Choosing the Right Visual Type</h2>
<table>
<thead><tr><th>Scene Content</th><th>Recommended Type</th></tr></thead>
<tbody>
<tr><td>Introduction / chapter start</td><td>Title Card or Section</td></tr>
<tr><td>Your product's UI</td><td>App Screenshot or App Annotated</td></tr>
<tr><td>Images from your article</td><td>Article Image</td></tr>
<tr><td>A list of features or steps</td><td>Text Points</td></tr>
<tr><td>Code examples</td><td>Code</td></tr>
<tr><td>Terminal commands</td><td>Terminal</td></tr>
<tr><td>Concepts without an image</td><td>Diagram/Image</td></tr>
<tr><td>Important tips or warnings</td><td>Callout</td></tr>
<tr><td>Numbers and metrics</td><td>Stats</td></tr>
<tr><td>Multi-step processes</td><td>Timeline</td></tr>
<tr><td>Testimonials or key quotes</td><td>Quote</td></tr>
<tr><td>Comparing options</td><td>Compare</td></tr>
<tr><td>End of video</td><td>Outro</td></tr>
</tbody>
</table>

<h2>Tips</h2>
<ul>
<li>Mix visual types throughout your video to keep viewers engaged — don't use the same type for every scene</li>
<li>Use App Screenshot for the most important UI moments so readers see your actual product, not AI-generated art</li>
<li>Code and Terminal scenes have automatic syntax highlighting — FinalDoc detects the language from the narration context</li>
<li>After changing scene types in the editor, always click Reassemble Video to apply the changes to the final MP4</li>
</ul>