# Supported Platforms

ContextWizard supports **12+ AI platforms out of the box**, plus custom platforms via URL patterns.

## Built-in Platforms

| Platform | URL | Status |
|----------|-----|--------|
| **ChatGPT** | chatgpt.com | ✅ Full support |
| **Claude** | claude.ai | ✅ Full support |
| **Gemini** | gemini.google.com | ✅ Full support |
| **Microsoft Copilot** | copilot.microsoft.com | ✅ Full support |
| **Perplexity** | perplexity.ai | ✅ Full support |
| **HuggingChat** | huggingface.co/chat | ✅ Full support |
| **Poe** | poe.com | ✅ Full support |
| **Grok** | grok.com | ✅ Full support |
| **DeepSeek** | chat.deepseek.com | ✅ Full support |
| **Qwen (通义千问)** | chat.qwen.ai | ✅ Full support |
| **Kimi** | kimi.com | ✅ Full support |
| **Manus** | manus.im | ✅ Full support |

## Custom Platforms

You can add any AI chat website by providing its URL pattern. The universal **MessageExtractor** fallback enables content capture on platforms without custom adapters.

### To add a custom platform:
1. Open ContextWizard → Settings → Platforms
2. Click **"Add Custom Platform"**
3. Enter a name and URL pattern (e.g., `*://mysite.com/chat/*`)
4. Save — capture will start working automatically

## Platform Detection

ContextWizard automatically detects when you're on a supported platform and displays a visual indicator. Each platform uses custom CSS selectors optimized for accurate content extraction.

## Upcoming Support

We regularly add support for new platforms through updates. Request a platform by opening a GitHub issue or contacting support@amipro.me.
