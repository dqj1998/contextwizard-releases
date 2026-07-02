# Privacy & Security

ContextWizard is built on a **local-first, zero-trust architecture**. Your data belongs to you — completely.

## Core Architecture

```
┌──────────────────────────────────────────────────┐
│                  Your Computer                    │
│                                                    │
│   ┌─────────────┐   ┌──────────────────────────┐  │
│   │ AI Platform  │   │   ContextWizard           │  │
│   │ (ChatGPT,    │◄──│   Extension               │  │
│   │  Claude...)  │   │                           │  │
│   └─────────────┘   │   ┌────────────────────┐  │  │
│                      │   │  Local IndexedDB    │  │  │
│                      │   │  (All data stored   │  │  │
│                      │   │   here)             │  │  │
│                      │   └────────────────────┘  │  │
│                      │                           │  │
│                      │   ☁️ Cloud Sync (opt-in) │  │
│                      │   → End-to-end encrypted  │  │
│                      └──────────────────────────┘  │
└──────────────────────────────────────────────────┘
```

## Data Storage

| What | Where | How |
|------|-------|-----|
| Captured conversations | Browser local (IndexedDB) | Encrypted at rest |
| Bookmarks & groups | Browser local (IndexedDB) | Encrypted at rest |
| Prompt templates | Browser local (IndexedDB) | Encrypted at rest |
| Settings & preferences | Browser local (`chrome.storage.local`) | Plain (no sensitive data) |
| Cloud Sync data (optional) | Encrypted remote server | AES-256-GCM, zero-knowledge |

## What We DO

- ✅ Store conversation data **locally on your machine**
- ✅ Use **platform-specific permissions** scoped to AI domains
- ✅ Provide **full transparency** — all stored data is inspectable
- ✅ Comply with **GDPR** privacy requirements
- ✅ Implement **end-to-end encryption** for optional Cloud Sync

## What We DO NOT

- ❌ **Never** upload your data without explicit opt-in
- ❌ **Never** track, analyze, or telemetry your usage
- ❌ **Never** sell or share your data
- ❌ **Never** require accounts for core features
- ❌ **Never** access unrelated websites
- ❌ **Never** modify your AI conversation content (read-only)

## Permissions Explained

| Permission | Why We Need It |
|------------|----------------|
| `storage` / `unlimitedStorage` | Store captured conversations locally |
| `tabs` / `activeTab` | Detect which AI platform tab is active |
| `scripting` | Inject content extractors on AI platform pages |
| `host_permissions` (specific domains) | Read conversation content on supported AI platforms (e.g., chatgpt.com, claude.ai) |
| `identity` | Google SSO for optional Cloud Sync |
| `alarms` / `notifications` | Smart reminders functionality |
| `clipboardRead` / `clipboardWrite` | Context copy features |

## Data Retention

| Scenario | Outcome |
|----------|---------|
| Extension uninstalled | All local data in IndexedDB is removed |
| Cloud Sync cancelled | Remote data retained for 30 days, then permanently deleted |
| Manual deletion | Per-item or bulk deletion immediately removes data |

## Security Best Practices

- **Manifest V3**: Latest Chrome extension framework with improved security model
- **Minimum permissions**: Only requested for core functionality
- **No external network requests**: Extension makes no outbound connections except:
  - To AI platforms you visit (for capture)
  - To Cloud Sync servers (only if you enable it)

## Vulnerability Reporting

If you discover a security issue, please contact us at **support@amipro.me**. We take all reports seriously.
