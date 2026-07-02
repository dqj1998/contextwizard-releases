# Changelog

All notable changes to ContextWizard will be documented in this file.

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
