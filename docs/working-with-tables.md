---
title: "Working with Tables"
description: "Creating, formatting, and managing tables in the article editor."
slug: "working-with-tables"
status: "PUBLISHED"
createdAt: "2026-02-24T05:03:34.180Z"
updatedAt: "2026-03-21T03:04:34.072Z"
---

<h1>Working with Tables</h1>
<p>Tables are great for comparing options, showing reference data, mapping fields to values, and displaying structured information. FinalDoc has a full-featured table editor built into the documentation editor.</p>

<h2>Inserting a Table</h2>
<ol>
<li>Place your cursor where you want the table in your article</li>
<li>Click the <strong>Table</strong> button in the editor toolbar</li>
<li>A grid appears — move your mouse over it to select the number of rows and columns you want (e.g., 3 columns × 4 rows)</li>
<li>Click to insert the table</li>
</ol>
<p>The table inserts at the cursor position with the first row automatically styled as a header (bold text, grey background).</p>

<h2>Editing Table Content</h2>
<ul>
<li>Click any cell and start typing</li>
<li>Press <strong>Tab</strong> to move to the next cell to the right</li>
<li>Press <strong>Shift+Tab</strong> to move to the previous cell</li>
<li>Press <strong>Tab</strong> in the last cell of the last row to automatically add a new row</li>
<li>You can apply formatting inside cells: bold, italic, code, links, bullet lists</li>
</ul>

<h2>Adding and Removing Rows/Columns</h2>
<p>Right-click any cell to access the table context menu:</p>
<ul>
<li><strong>Insert row above</strong> — Adds a new empty row above the current row</li>
<li><strong>Insert row below</strong> — Adds a new empty row below the current row</li>
<li><strong>Insert column left</strong> — Adds a column to the left of the current column</li>
<li><strong>Insert column right</strong> — Adds a column to the right of the current column</li>
<li><strong>Delete row</strong> — Removes the entire current row</li>
<li><strong>Delete column</strong> — Removes the entire current column</li>
<li><strong>Delete table</strong> — Removes the entire table (content is lost)</li>
</ul>

<h2>Table Headers</h2>
<p>The first row of a table is treated as the header row by default. Header cells appear in bold with a distinct background color. This also affects how screen readers announce the table to visually impaired users — always use a header row for accessible documentation.</p>

<h2>Merging Cells</h2>
<p>FinalDoc supports basic cell merging for complex table layouts:</p>
<ol>
<li>Click and drag to select multiple adjacent cells</li>
<li>Right-click the selection → <strong>Merge Cells</strong></li>
<li>The selected cells merge into one larger cell</li>
<li>To split a merged cell back, right-click it → <strong>Split Cell</strong></li>
</ol>

<h2>Table Width</h2>
<p>By default, tables stretch to the full width of the content area. For narrow tables with few columns, click the table and look for width controls in the toolbar. You can set a percentage or auto width.</p>

<h2>Tables on Mobile</h2>
<p>Wide tables can be hard to read on small screens. For tables with many columns, consider:</p>
<ul>
<li>Reducing the number of columns (combine related columns)</li>
<li>Using a list format instead for simple key-value data</li>
<li>Adding a note to readers that the table scrolls horizontally on mobile</li>
</ul>

<h2>Example Use Cases</h2>
<table>
<thead><tr><th>Use Case</th><th>Example</th></tr></thead>
<tbody>
<tr><td>Feature comparison</td><td>Compare Free vs Pro vs Enterprise plan features</td></tr>
<tr><td>API reference</td><td>Parameter name, type, required/optional, description</td></tr>
<tr><td>Keyboard shortcuts</td><td>Action, Windows shortcut, Mac shortcut</td></tr>
<tr><td>Status codes</td><td>HTTP code, meaning, when it occurs</td></tr>
<tr><td>Configuration options</td><td>Setting name, default value, description</td></tr>
</tbody>
</table>