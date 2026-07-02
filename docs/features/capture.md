# Automatic Capture

ContextWizard automatically saves your AI conversations as you chat across supported platforms.

## How It Works

- **Real-time detection**: Uses MutationObserver to detect new messages on supported AI platforms
- **Platform-specific selectors**: Each platform has custom CSS selectors for accurate content extraction
- **Universal fallback**: A general-purpose MessageExtractor works for custom or unrecognized platforms
- **Intelligent deduplication**: Prevents duplicate saves when revisiting or reloading conversations
- **Debounced saving**: Balances responsiveness with storage efficiency

## Capture Modes

| Mode | Behavior |
|------|----------|
| **Auto** (default) | Captures every conversation continuously without intervention |
| **Manual** | Only saves when you explicitly trigger capture |

To switch to manual mode → Settings → Capture Mode → Manual.

## What Gets Captured

- **Conversation title** (auto-detected from the page)
- **Full message content** — both your prompts and the AI's responses
- **Platform identifier** (ChatGPT, Claude, Gemini, etc.)
- **Timestamp** of when the conversation occurred
- **Visual thumbnail** — automated screenshot of the conversation

## Visual Indicator

When ContextWizard is actively capturing on a page, you'll see a small indicator showing capture activity. This can be toggled in Settings.

## Platform Configuration

- Enable/disable platforms individually from Settings → Platforms
- Add custom platforms by providing a URL pattern
- View capture status for each platform
