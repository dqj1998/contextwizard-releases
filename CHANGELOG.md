# Changelog

All notable changes to ContextWizard will be documented in this file.

## [2.1.0] — 2026-07-04

### 🎉 Feature: Open in Bookmark Manager

Quickly navigate to any bookmark in the dedicated Bookmark Manager window.

- **One-click access**: Click the "Open in Bookmark Manager" button from bookmark hover preview or chat list
- **Auto-scroll & highlight**: The Bookmark Manager opens and scrolls directly to the selected bookmark with a pulse highlight
- **Smart window management**: Reuses existing Bookmark Manager window if already open

### 🧠 Improved Context Extraction

Better context injection with enhanced language support and matching accuracy.

- **CJK Support**: Intl.Segmenter-powered tokenization for Chinese, Japanese, and Korean text
- **URL Normalization**: Path-prefix matching for more accurate conversation association
- **Content Fallback**: Content-based matching when URL matching fails

### ⏰ Reminder Reliability

More dependable reminder scheduling and processing.

- **Race Condition Prevention**: Lock mechanism prevents concurrent reminder alarm processing
- **Accurate Monthly Reminders**: Improved `getNextNthWeekdayForMonth` calculation for monthly recurrence
- **Storage Cleanup Protection**: Bookmarked conversations are now protected from being pruned during storage cleanup

### 🌐 i18n Updates

- Bookmark Manager button labels added to all 12 supported languages

### 🔄 Context Panel Refresh

The floating context panel now has a manual refresh button, giving you control over when bookmark data is reloaded.

- **Refresh button**: Reload bookmarks from storage without reopening the panel
- **Real-time sync**: Bookmark group expansion and conversation filtering happen on the fly
- **Visual feedback**: Spinning indicator during refresh, toast notification with result count

### 🔖 Bookmark Reliability Improvements

More robust bookmark handling across all AI platforms.

- **Better injection**: Bookmark context now replaces stale content instead of being silently skipped — re-injecting always delivers fresh context
- **SPA-friendly markers**: Bookmarks now work reliably on Copilot and other single-page apps where content loads asynchronously (retries with backoff, on-the-fly marker creation)
- **Direct Gemini links**: Opening a Gemini bookmark from the manager now reliably loads the full conversation — no more blank pages
- **Conversation deduplication**: Fixed rare cases where conversations with changing URLs (e.g. Gemini) could create duplicate entries

### 🐛 Bug Fixes

- Fixed PLATFORMS re-declaration issue that could cause errors on double injection
- Wrapped platforms.js in IIFE to fix illegal top-level return in popup.html context

---

## [2.0.0] — 2026-07-02

### 🎉 Major: Bookmark Context Chat

ContextWizard v2.0 bridges the gap between saving insights and using them. Your bookmarks are now directly actionable — inject them into any conversation with zero friction.

#### 🧠 Context Panel (New)
- **Floating Context Panel**: A panel appears next to your chat input displaying relevant bookmarks. Select the ones you need, and your AI gets the full picture without you ever leaving the page.
- **Keyboard Navigation**: Full keyboard support (Tab, arrows, Space, Enter, Escape) for power users.
- **Smart Context Injection**: The panel automatically shows the most relevant bookmarks for your current conversation topic.
- **Automatic Content Trimming**: Bookmark content is trimmed automatically to fit within conversation context limits.

#### 🔄 Session Management
- Tab-level session isolation — research notes for Project A never mix with Project B
- Each bookmark group maintains its own session state

#### 🔧 Popup Redesign
- New tab-based layout for faster navigation
- Conversations and bookmarks are one click away
- Improved visual hierarchy and information density

#### 📁 Bookmark Group Enhancements
- **Rename groups** directly from the UI
- **Start a chat** right from your bookmark list
- **Jump back** to where you bookmarked something in a conversation with one click

#### 🛡️ Permissions
- No new permissions required for v2.0.0
- All features continue to work locally
- No data is sent externally unless Cloud Sync is explicitly enabled

### 🐛 Bug Fixes
- Fixed duplicate capture issue on conversation reload
- Improved platform detection reliability
- Enhanced bookmark deletion undo behavior
- Fixed rare IndexedDB write conflicts under heavy load

---

## [1.x] — Previous Releases

### [1.5.0] — 2026-05-XX

- Added cross-platform bookmarks with custom groups
- Introduced bookmark group management (rename, delete, undo)
- Added instant-undo support for bookmark operations
- Improved search ranking algorithm
- Added platform filter to search results
- Fixed content extraction for Claude follow-up messages

### [1.4.0] — 2026-04-XX

- Added Prompt Editor with template management
- Introduced auto-redaction for sensitive data (API keys, passwords, tokens)
- Added custom redaction rules configuration
- Enhanced options page with data statistics
- Added export/import functionality for conversations
- Performance improvements for large conversation histories

### [1.3.0] — 2026-03-XX

- Added smart reminders with recurrence options
- Browser notifications for scheduled reminders
- Click notification to jump to exact bookmarked message
- Added reminder management interface
- Fixed notification timing on browser sleep/wake

### [1.2.0] — 2026-02-XX

- Added AI Workspaces with project-level organization
- Drag-and-drop conversation management
- Auto-suggest workspace names from conversation content
- Workspace-level search filtering
- Added support for Grok (grok.com)
- Added support for DeepSeek (chat.deepseek.com)

### [1.1.0] — 2026-01-XX

- Introduced full-text search across all platforms
- WebAssembly-accelerated search engine
- Search suggestions and smart ranking
- Context previews in search results
- Added support for Perplexity, HuggingChat, Poe
- Platform toggle controls in dashboard
- i18n support with 12 languages

### [1.0.0] — 2025-12-XX

- 🎉 Initial release
- Automatic conversation capture for ChatGPT, Claude, Gemini
- Real-time MutationObserver-based content detection
- Local IndexedDB storage
- Basic conversation list and management
- Cross-platform support foundation
- Manifest V3 compliant
- Minimum required permissions philosophy
