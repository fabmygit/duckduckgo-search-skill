-----

## name: duckduckgo-search
description: Search the web for current information about any topic, person, website or event.

# DuckDuckGo Web Search

## Instructions

Call the `run_js` tool with the following exact parameters:

- script name: index.html
- data: A JSON string with the following fields:
  - query: String. The search query extracted from the user’s request.
  - lang: String. The 2-letter language code (e.g. “en”, “de”, “fr”).

**Constraints:**

- Always call run_js — never answer from memory alone.
- Summarize the results in 2-3 sentences.
- Always respond in the same language as the user.
- If no results found, say so briefly.
