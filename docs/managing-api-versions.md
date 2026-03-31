---
title: "Managing API Versions"
description: "Handle multiple API versions, deprecation notices, and versioned documentation."
slug: "managing-api-versions"
status: "PUBLISHED"
createdAt: "2026-02-24T03:51:14.876Z"
updatedAt: "2026-03-27T10:29:46.727Z"
---

<h1>Managing API Versions</h1>
<p>As your API evolves, you'll have multiple versions (v1, v2, v3). FinalDoc's API Docs section supports maintaining separate documentation for each version simultaneously — readers can switch between versions using a version selector in the API reference.</p>

<h2>Adding an API Version</h2>
<ol>
<li>Go to <strong>API Docs</strong> in the left sidebar</li>
<li>Click <strong>+ Add Version</strong> (or <strong>Import Specification</strong> with a version tag)</li>
<li>Upload or paste your OpenAPI spec for this version</li>
<li>Give the version a <strong>label</strong> (e.g., "v1", "v2.0", "2024-01", "Latest")</li>
<li>Set the version's status:
  <ul>
    <li><strong>Current</strong> — Shown first, labeled as the recommended version</li>
    <li><strong>Legacy</strong> — Still accessible but shown with a deprecation notice</li>
    <li><strong>Beta</strong> — Available but marked as not yet stable</li>
  </ul>
</li>
<li>Click <strong>Save</strong></li>
</ol>

<h2>Version Selector for Readers</h2>
<p>When multiple versions exist, a version dropdown appears in the API reference header. Readers can select the version they're working with. Each version has its own endpoint list and documentation.</p>

<h2>Setting the Default Version</h2>
<ol>
<li>In the API Docs view, click the version you want as the default</li>
<li>Click <strong>Set as Default</strong></li>
</ol>
<p>The default version is what readers see when they first open the API reference — before choosing a version from the dropdown.</p>

<h2>Deprecating a Version</h2>
<p>When you want to phase out an old version:</p>
<ol>
<li>Click on the old version in the API Docs list</li>
<li>Change its status to <strong>Deprecated</strong></li>
<li>Optionally add a <strong>Deprecation notice</strong> — a message shown at the top of the deprecated version's reference page (e.g., "This API version is deprecated. Please migrate to v2 by June 30, 2026.")</li>
<li>Set a <strong>Sunset date</strong> — displayed to readers so they know when support ends</li>
</ol>

<h2>Updating an Existing Version</h2>
<ol>
<li>Click on the version you want to update</li>
<li>Click <strong>Update Specification</strong></li>
<li>Upload or paste the new spec</li>
<li>FinalDoc merges the changes — new endpoints appear, removed endpoints are flagged, changed schemas are updated</li>
</ol>

<h2>Deleting a Version</h2>
<p>Click on a version → <strong>Delete Version</strong>. Confirm the deletion. The version and all its documentation are removed from the public API reference. Make sure readers have had time to migrate before deleting a version.</p>