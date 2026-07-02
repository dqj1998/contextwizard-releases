# Cloud Sync (Optional)

Optionally keep workspaces and bookmarks synchronized across multiple computers.

> **Note**: Cloud Sync is a paid subscription feature. Core features (capture, search, bookmarks, workspaces, reminders) are free and work entirely offline.

## How It Works

- All data is **end-to-end encrypted** in transit and at rest
- Uses **Google SSO** for authentication — no third-party services needed
- Syncs workspaces, bookmarks, and bookmark groups across devices
- Captured conversation content is not synced (remains local)

## Security

| Layer | Protection |
|-------|------------|
| **In transit** | TLS 1.3 encryption |
| **At rest** | AES-256-GCM encryption |
| **Key management** | Client-side key derivation, server never sees raw keys |
| **Authentication** | Google OAuth 2.0 only |

## Free Trial

- **7-day free trial** with full sync features
- **No credit card required**
- Downgrade anytime
- Data preserved for **30 days** after cancellation

## Enabling Cloud Sync

1. Open ContextWizard → Settings → Cloud Sync
2. Click **"Sign in with Google"**
3. After authentication, sync starts automatically
4. Install ContextWizard on other machines and sign in with the same Google account
