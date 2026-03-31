---
title: "Code Blocks, Diagrams & Math"
description: "Adding code snippets with syntax highlighting, Mermaid diagrams, and LaTeX formulas."
slug: "code-blocks-diagrams-math"
status: "PUBLISHED"
createdAt: "2026-02-23T18:13:42.918Z"
updatedAt: "2026-03-21T06:06:23.614Z"
---

<h1>Code Blocks, Diagrams, and Math</h1>
<p>FinalDoc provides specialized blocks for technical content — syntax-highlighted code, visual diagrams generated from text, and mathematical equations. This article explains how to use each one.</p>

<h2>Code Blocks</h2>
<h3>Inserting a Code Block</h3>
<ol>
<li>Place your cursor on an empty line (or where you want the code block)</li>
<li>Click the <strong>Code Block</strong> button in the toolbar (looks like <code>&lt;/&gt;</code>)</li>
<li>Or press <strong>Ctrl+Shift+K</strong> on Windows / <strong>Cmd+Shift+K</strong> on Mac</li>
<li>A code block appears with a language selector in the top-right corner</li>
</ol>

<h3>Selecting a Programming Language</h3>
<p>Click the language dropdown in the top-right of the code block. Available languages include:</p>
<p>JavaScript, TypeScript, Python, Java, C, C++, C#, Go, Rust, PHP, Ruby, Swift, Kotlin, SQL, Bash/Shell, HTML, CSS, JSON, YAML, XML, Markdown, and more.</p>
<p>Selecting a language enables syntax highlighting — keywords, strings, and comments appear in different colors to make code easier to read.</p>

<h3>Writing Code</h3>
<p>Click inside the block and type your code. The editor respects indentation and preserves whitespace. Press <strong>Tab</strong> to indent (inserts spaces, not a tab character, to keep things consistent across browsers).</p>

<h3>Copy Button</h3>
<p>Readers see a <strong>Copy</strong> button in the top-right corner of each code block when they hover over it. Clicking it copies the entire code block to their clipboard — essential for documentation that provides commands or configuration snippets.</p>

<h3>Inline Code</h3>
<p>For short pieces of code within a sentence (like a function name, variable, or command), use <strong>inline code</strong> formatting instead of a full code block:</p>
<ol>
<li>Select the text you want to format as code</li>
<li>Press <strong>Ctrl+Shift+C / Cmd+Shift+C</strong></li>
<li>Or click the inline code button (the backtick button) in the toolbar</li>
</ol>
<p>The text appears in a monospace font with a subtle background — for example: <code>npm install finaldoc</code>.</p>

<h2>Diagrams (Mermaid)</h2>
<p>FinalDoc renders <strong>Mermaid</strong> diagrams — a text-based diagramming language. Write diagram code and FinalDoc renders a visual diagram automatically.</p>

<h3>Inserting a Mermaid Diagram</h3>
<ol>
<li>Click the <strong>Diagram</strong> button in the toolbar</li>
<li>Select <strong>Mermaid Diagram</strong></li>
<li>A diagram block appears with example code</li>
<li>Edit the code to describe your diagram</li>
<li>The visual preview updates in real time</li>
</ol>

<h3>Diagram Types You Can Create</h3>
<table>
<thead><tr><th>Diagram Type</th><th>Mermaid Keyword</th><th>Best For</th></tr></thead>
<tbody>
<tr><td>Flowchart</td><td><code>graph TD</code> or <code>flowchart LR</code></td><td>Step-by-step processes, decision trees</td></tr>
<tr><td>Sequence Diagram</td><td><code>sequenceDiagram</code></td><td>API interactions, system communication flows</td></tr>
<tr><td>ER Diagram</td><td><code>erDiagram</code></td><td>Database schemas and data relationships</td></tr>
<tr><td>Class Diagram</td><td><code>classDiagram</code></td><td>Object-oriented code structure</td></tr>
<tr><td>Gantt Chart</td><td><code>gantt</code></td><td>Project timelines and schedules</td></tr>
<tr><td>State Diagram</td><td><code>stateDiagram-v2</code></td><td>Application states and transitions</td></tr>
<tr><td>Pie Chart</td><td><code>pie</code></td><td>Simple percentage breakdowns</td></tr>
</tbody>
</table>

<h3>AI-Generated Diagrams</h3>
<p>You can describe a diagram in plain English and let the AI generate the Mermaid code for you:</p>
<ol>
<li>Click the Diagram button → <strong>AI Diagram</strong></li>
<li>Type a description like "Create a sequence diagram showing how a user logs in with OAuth"</li>
<li>Click <strong>Generate</strong></li>
<li>The AI writes the Mermaid code and renders the diagram</li>
<li>Edit the code if needed to refine the result</li>
</ol>

<h2>Mathematical Equations (LaTeX)</h2>
<p>FinalDoc renders LaTeX math equations using <strong>KaTeX</strong> — the same math rendering used by Wikipedia and Notion.</p>

<h3>Inserting a Math Block</h3>
<ol>
<li>Click the <strong>Math</strong> button in the toolbar (Σ symbol)</li>
<li>A math block appears</li>
<li>Type your LaTeX equation inside the block</li>
<li>The rendered equation appears as you type</li>
</ol>

<h3>Inline Math</h3>
<p>For equations within a sentence, use the inline math option. Wrap your LaTeX in single dollar signs: <code>$E = mc^2$</code> — it renders the equation inline with the text.</p>

<h3>LaTeX Examples</h3>
<table>
<thead><tr><th>LaTeX Code</th><th>Renders As</th></tr></thead>
<tbody>
<tr><td><code>E = mc^2</code></td><td>E = mc²</td></tr>
<tr><td><code>\frac{1}{2}mv^2</code></td><td>½mv²</td></tr>
<tr><td><code>\sum_{i=1}^{n} i</code></td><td>Sum from 1 to n</td></tr>
<tr><td><code>\sqrt{a^2 + b^2}</code></td><td>Square root of (a² + b²)</td></tr>
</tbody>
</table>