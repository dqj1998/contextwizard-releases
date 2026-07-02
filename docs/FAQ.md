# Frequently Asked Questions

## General

### What is ContextWizard?
ContextWizard is a free, local-first browser extension that automatically captures and organizes your AI conversations across 10+ platforms including ChatGPT, Claude, Gemini, Copilot, Perplexity, Grok, DeepSeek, and Qwen. All data stays on your computer — nothing is uploaded to any cloud server without your explicit consent.

### Is ContextWizard free?
Yes. Core features including unlimited captures, bookmarks, workspaces, search, reminders, and the Context Panel are free. Cloud Sync requires a subscription.

### Does it work offline?
Yes. All local features work fully offline. Only Cloud Sync requires internet access.

### Which browsers are supported?
Google Chrome and Microsoft Edge on desktop (Manifest V3).

### How many AI platforms are supported?
12+ built-in platforms including ChatGPT, Claude, Gemini, Copilot, Perplexity, HuggingChat, Poe, Grok, DeepSeek, Qwen, Kimi, and Manus. You can also add custom platforms via URL patterns.

## Privacy & Data

### Does ContextWizard collect my data?
No. Everything is stored locally on your computer. Cloud Sync is optional and end-to-end encrypted. No tracking, no analytics, no telemetry.

### Can my data be accessed by anyone else?
No. All data is stored locally in your own browser's IndexedDB. It never leaves your machine unless you explicitly enable Cloud Sync.

### What happens if I uninstall?
All locally stored data in IndexedDB is removed. Cloud Sync data is retained in your account for 30 days after cancellation.

### Can I export my data?
Direct export is available from the settings panel. You can export conversations in the app's native format for backup or migration.

### Is data encrypted?
Local data is stored in IndexedDB (not encrypted at rest by the browser itself — standard for local-first extensions). Cloud Sync data is encrypted end-to-end with AES-256-GCM.

## Features

### Can I search across platforms simultaneously?
Yes. A single search queries all captured conversations across ChatGPT, Claude, Gemini, and every other supported platform at once.

### How is this different from browser bookmarks?
Browser bookmarks save URLs only. ContextWizard saves full conversation content with full-text search across all messages and platforms.

### What is the Context Panel (v2.0)?
The Context Panel lets you inject your bookmarked insights directly into a new conversation. Instead of copying and pasting, select the bookmarks you need and they're added to your chat context automatically.

### How do reminders work?
Set a reminder on any bookmarked message with your chosen recurrence (once, daily, weekdays, weekly, monthly). Your browser shows a system notification at the scheduled time. Click it to jump directly to that exact conversation.

### Can I organize conversations?
Yes. Use **Workspaces** for project-level grouping, and **Bookmark Groups** within conversations for precise message-level organization.

### Can I disable auto-capture?
Yes. Switch to manual capture mode in Settings. Save conversations only when you choose.

## Technical

### Does it work with ChatGPT Teams or Enterprise?
It works with chatgpt.com including Teams. Enterprise deployments with custom domains may need configuration.

### Does it slow down my browser?
No. ContextWizard is lightweight and optimized. Content capture uses minimal resources with intelligent debouncing to avoid performance impact.

### Does ContextWizard modify my AI conversation content?
No. ContextWizard is read-only with respect to your conversations. It captures and indexes content but never alters it.

### Are there limits on captures or bookmarks?
No. Free users get unlimited captures, bookmarks, workspaces, search, and reminders.

### Does it support custom AI platforms?
Yes. Add any website as a custom platform by providing its URL pattern. Content extraction works automatically via the universal MessageExtractor fallback.

### Can I delete individual captures or bookmarks?
Yes. Delete any capture, bookmark, or workspace individually. Bulk operations are available.

## Cloud Sync

### How does Cloud Sync work?
Optional paid feature that syncs workspaces and bookmarks across multiple computers. End-to-end encrypted with Google SSO.

### How does the Cloud Sync trial work?
7-day free trial with full sync features. No credit card required. Downgrade anytime. Data preserved for 30 days.

## Compatibility

### What happens to existing conversations when I install?
Previously existing conversations on AI platforms are not retroactively captured. ContextWizard captures conversations from the moment of installation going forward. Your existing platform history remains accessible as before — nothing is deleted or modified.

### Can I use ContextWizard with non-AI websites?
ContextWizard is designed for AI chat platforms. While you can add custom URL patterns, optimal capture requires platform-specific content adapters.
