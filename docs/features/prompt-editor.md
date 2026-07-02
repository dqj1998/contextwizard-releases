# Prompt Editor & Privacy Guard

Manage reusable prompt templates with built-in auto-redaction to keep sensitive data safe.

## Prompt Templates

- **Create** new prompt templates for different use cases
- **Edit** and organize prompts in a dedicated editor
- **Reuse** proven prompts across any AI platform
- Organize templates by category or project

## Auto-Redaction

Define custom redaction rules that automatically replace sensitive information with placeholders before sending:

| Redaction Type | Example | Placeholder |
|----------------|---------|-------------|
| API Keys | `sk-abc123...` | `[API_KEY_REDACTED]` |
| Passwords | `myP@ssw0rd` | `[PASSWORD_REDACTED]` |
| Private Tokens | `ghp_xxxx...` | `[TOKEN_REDACTED]` |
| Custom patterns | Any regex pattern | Customizable |

## How It Works

1. Open the **Prompt Editor** from the dashboard
2. Create or edit a prompt template
3. Define redaction rules (built-in + custom)
4. Copy the prompt — sensitive data is automatically redacted when you paste
5. The redacted prompt is safe to use on any AI platform

## Use Cases

| Scenario | Benefit |
|----------|---------|
| **Code review prompts** | Redact proprietary function names or internal API keys |
| **Business strategy prompts** | Redact confidential revenue figures |
| **Personal assistant prompts** | Redact private contact details or addresses |
| **Reusable research prompts** | Keep methodology while stripping identifying information |
