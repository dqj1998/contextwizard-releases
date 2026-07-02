# Cross-Platform Search

Search every captured conversation from every AI platform — all at once.

## Features

- **Full-text search**: Searches titles, summaries, and message bodies
- **Phrase search**: Use quotes `"exact phrase"` for precise matching
- **Keyword matching**: Flexible discovery for partial matches
- **Smart ranking**: Results sorted by relevance and recency
- **Platform filters**: Narrow results to specific AI platforms
- **Workspace filters**: Search within a specific project workspace
- **Time range filters**: Filter by capture date
- **Context previews**: See surrounding conversation without opening it
- **Match type indicators**: Shows why each result matched

## How to Search

1. Open the ContextWizard popup
2. Click in the search bar
3. Type your query
4. Optionally filter by platform or workspace

## Search Tips

| Goal | Do This |
|------|---------|
| Find an exact phrase | `"the specific insight I need"` |
| Search one platform | Use the platform filter dropdown |
| Search one workspace | Switch to workspace-level search |
| Find recent conversations | Use the time range filter |

## Technical Details

The search engine uses **WebAssembly-accelerated indexing** for sub-second query performance across thousands of conversations.
