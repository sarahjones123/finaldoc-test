---
title: "Widget Contact Form"
description: "Configuring the contact form in the embedded help widget for reader support requests."
slug: "widget-contact-form"
status: "PUBLISHED"
createdAt: "2026-02-24T05:03:42.051Z"
updatedAt: "2026-03-27T10:59:45.604Z"
---

<h1>Widget Contact Form</h1>
<p>The Widget Contact Form is an optional feature that lets readers submit a help request or question directly from within the FinalDoc widget — without leaving your website. When a reader searches and doesn't find an answer, or clicks "Contact Us," a simple form appears for them to type their question. The submission lands in your FinalDoc Feedback inbox (or is forwarded to your helpdesk via webhook).</p>

<h2>Enabling the Contact Form</h2>
<ol>
<li>Click <strong>External Widget</strong> in the left sidebar</li>
<li>Open your widget configuration</li>
<li>Go to the <strong>Content</strong> tab</li>
<li>Enable <strong>Show Contact Form</strong></li>
<li>Configure the form fields (see below)</li>
<li>Click <strong>Save</strong></li>
</ol>

<h2>Contact Form Fields</h2>
<p>Configure which fields appear on the form:</p>
<ul>
<li><strong>Name</strong> — Reader's full name (optional or required)</li>
<li><strong>Email</strong> — Reader's email address (required if you want to respond)</li>
<li><strong>Subject</strong> — Brief topic (optional)</li>
<li><strong>Message</strong> — The main text area for the reader's question (required)</li>
</ul>
<p>Mark fields as Required or Optional using the toggle next to each field name.</p>

<h2>Where Contact Form Submissions Go</h2>
<p>Submissions from the contact form go to:</p>
<ul>
<li><strong>FinalDoc Feedback inbox</strong> — Appears as a feedback entry with type "Widget Contact Form"</li>
<li><strong>Email notification</strong> — If email notifications for feedback are configured in Settings → Notifications</li>
<li><strong>Webhook forwarding</strong> — If you've set up a Webhook for the "feedback.submitted" event, the submission is also sent to your webhook URL (useful for forwarding to Zendesk, Intercom, etc.)</li>
</ul>

<h2>Contact Form Trigger</h2>
<p>Control when the contact form appears:</p>
<ul>
<li><strong>Manual</strong> — A "Contact Us" button in the widget footer that readers click deliberately</li>
<li><strong>After zero results</strong> — Contact form appears automatically when a search returns no results</li>
<li><strong>Both</strong> — Both the button and the auto-trigger are active</li>
</ul>

<h2>Customizing the Form Appearance</h2>
<p>The contact form inherits the widget's color scheme (primary color, button styles). You can customize the form's:</p>
<ul>
<li><strong>Heading text</strong> — e.g., "Didn't find what you need? Ask us!" (custom text in the widget configuration)</li>
<li><strong>Submit button label</strong> — e.g., "Send Message" or "Submit Request"</li>
<li><strong>Success message</strong> — What the reader sees after submitting (e.g., "Thanks! We'll get back to you within one business day.")</li>
</ul>

<h2>Spam Protection</h2>
<p>The contact form includes built-in honeypot spam protection. Submissions that appear automated are automatically rejected. For heavier spam protection, contact FinalDoc support to enable reCAPTCHA on the widget form.</p>