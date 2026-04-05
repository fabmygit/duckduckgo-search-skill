---
name: duckduckgo-search
description: Search the web using DuckDuckGo for current information, news, and facts. No API key required
---

# DuckDuckGo Web Search

## Instructions

When the user asks about current events, recent news, or any topic that needs up-to-date information:

1. Extract a short, specific search query (2-5 words) from the user's question.

2. Call the `run_js` tool with the following parameters:
   - data: A JSON string with the following field:
     - query: String. The search query to look up on DuckDuckGo.

3. The tool returns a list of results. Summarize the top results clearly.

4. Always show title and URL for each result.

## Output Format

Search: "[query]"

1. [Title] - [one sentence summary]
   URL: [URL]

2. [Title] - [one sentence summary]
   URL: [URL]

3. [Title] - [one sentence summary]
   URL: [URL]

Finish with a brief 2-3 sentence synthesis of what was found.

## Notes
- Respond in the same language the user used.
- If results are empty, say so and answer from your own knowledge.
