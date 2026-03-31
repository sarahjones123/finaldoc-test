---
title: "Exporting Analytics Data"
description: "Export analytics reports as CSV for external reporting and analysis."
slug: "exporting-analytics-data"
status: "PUBLISHED"
createdAt: "2026-02-24T03:50:51.643Z"
updatedAt: "2026-03-19T15:28:45.010Z"
---

<h1>Exporting Analytics Data</h1>
<p>You can export analytics data from FinalDoc as CSV files for offline analysis, custom reporting, or sharing with stakeholders. Most analytics views in FinalDoc include an Export button so you can download data to a spreadsheet.</p>

<h2>What Can Be Exported</h2>
<table>
<thead><tr><th>Analytics View</th><th>What's Included in the Export</th></tr></thead>
<tbody>
<tr><td><strong>Article Analytics</strong></td><td>Each article: title, views, unique readers, avg time on page, feedback score, reaction counts, last updated date</td></tr>
<tr><td><strong>Reader Analytics</strong></td><td>Each reader: email, articles read, total reading time, first visit date, last visit date, country</td></tr>
<tr><td><strong>Search Analytics</strong></td><td>Each search query: query text, count, results returned, zero-results flag, last searched date</td></tr>
<tr><td><strong>Feedback</strong></td><td>Each feedback entry: article title, rating (thumbs up/down), comment text, reader email, submission date</td></tr>
<tr><td><strong>Audit Log</strong></td><td>Each log entry: action type, user, affected resource, timestamp, IP address</td></tr>
<tr><td><strong>Team Performance</strong></td><td>Each team member: articles created/updated/published, words written, avg quality score, last active date</td></tr>
</tbody>
</table>

<h2>How to Export</h2>
<ol>
<li>Navigate to the analytics view you want to export (e.g., <strong>Analytics → Article &amp; Reader Analytics</strong>)</li>
<li>Apply any filters you want (date range, specific categories, etc.)</li>
<li>Click the <strong>Export CSV</strong> button in the top-right of the table</li>
<li>The browser downloads a <code>.csv</code> file immediately</li>
</ol>
<p>The export reflects the current filter state — if you've filtered to a specific date range, only data for that period is exported.</p>

<h2>Opening the CSV File</h2>
<p>CSV files open in Excel, Google Sheets, or any spreadsheet application:</p>
<ul>
<li><strong>Google Sheets</strong>: File → Import → Upload → select the CSV file</li>
<li><strong>Microsoft Excel</strong>: Open Excel → File → Open → browse to the file. If characters look wrong, use the Text Import Wizard (files are UTF-8 encoded)</li>
<li><strong>Apple Numbers</strong>: Double-click the CSV file — Numbers opens it automatically</li>
</ul>

<h2>API Access to Analytics Data</h2>
<p>For automated exports (daily reports, BI tool integration, dashboards), use the FinalDoc REST API's analytics endpoints. You can query article analytics, reader data, and search data programmatically and pipe it into your own reporting tools. See the <strong>Analytics API Reference</strong> article for endpoint documentation and example queries.</p>

<h2>Scheduled Exports</h2>
<p>Automatic scheduled exports (daily or weekly email reports sent as CSV attachments) are available on Business and Enterprise plans. Configure them in <strong>Settings → Notifications → Analytics Reports</strong>. Set the frequency (daily/weekly), recipients (email addresses), and which analytics data to include.</p>

<h2>Data Retention</h2>
<p>FinalDoc stores analytics data for:</p>
<ul>
<li><strong>Article views and search data</strong>: 12 months on paid plans, 30 days on free plan</li>
<li><strong>Reader session data</strong>: 90 days on paid plans, 30 days on free plan</li>
<li><strong>Audit logs</strong>: 90 days on paid plans, 30 days on free plan</li>
</ul>
<p>Export data before it ages out if you need long-term historical records.</p>