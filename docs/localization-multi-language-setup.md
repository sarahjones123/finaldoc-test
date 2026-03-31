---
title: "Localization & Multi-language Setup"
description: ""
slug: "localization-multi-language-setup"
status: "PUBLISHED"
createdAt: "2026-02-24T08:32:54.677Z"
updatedAt: "2026-03-12T09:07:14.387Z"
---

<h1>Localization and Multi-Language Setup</h1>
<p>FinalDoc supports serving your knowledge base in multiple languages. You can translate article content (using the built-in AI translation), configure language display settings, and let readers switch between language versions of articles on the public KB.</p>

<h2>Opening Localization Settings</h2>
<ol>
<li>Go to <strong>Settings → General → Localization &amp; Multi-language Setup</strong></li>
</ol>

<h2>Setting the Primary Language</h2>
<p>Set your knowledge base's primary/default language — the language most of your content is written in. This is used for:</p>
<ul>
<li>The default language shown to readers who have not selected a preference</li>
<li>SEO language tags in your HTML (<code>lang</code> attribute)</li>
<li>The baseline for translation targets</li>
</ul>

<h2>Enabling Additional Languages</h2>
<ol>
<li>In Localization settings, click <strong>Add Language</strong></li>
<li>Select the language from the dropdown (e.g., Spanish, French, German, Japanese)</li>
<li>Click <strong>Add</strong></li>
</ol>
<p>Adding a language does not automatically translate your content — it makes that language available as a target for translations. You still need to translate articles using the Translation feature (see the <strong>One-Click AI Translation</strong> article).</p>

<h2>Language Selector on the Public KB</h2>
<p>Once multiple languages are enabled and you have translated articles published:</p>
<ol>
<li>In Localization settings, enable <strong>Show Language Selector</strong></li>
<li>A language dropdown appears in the KB header for readers to choose their preferred language</li>
<li>When a reader selects a language, FinalDoc shows the translated version of each article (if available), or falls back to the original language if no translation exists</li>
</ol>

<h2>Organizing Multi-Language Content</h2>
<p>There are two common approaches to organizing translated articles:</p>

<h3>Approach 1: Language-Specific Categories</h3>
<p>Create top-level categories for each language: "Documentation (English)", "Documentación (Español)", "Documentation (Français)". All translated articles for a language go in that category. Simple, but results in duplicate navigation structure.</p>

<h3>Approach 2: Article-Level Translation</h3>
<p>Keep your category structure in the primary language. Translated articles are linked to the originals using FinalDoc's language tagging system. The language selector on article pages lets readers switch between versions. Cleaner structure, better for readers.</p>

<h2>Date and Number Formats</h2>
<p>FinalDoc automatically formats dates and numbers based on the reader's selected language locale. For example, a reader using French will see dates in DD/MM/YYYY format instead of MM/DD/YYYY.</p>