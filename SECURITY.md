# Security

Do not commit access tokens, API keys, passwords, personal data, or exported n8n credential bindings.

Set the required values in the n8n runtime environment and keep them out of workflow exports:

- `LINE_RAG_CHANNEL_ACCESS_TOKEN`
- `LINE_MCP_CHANNEL_ACCESS_TOKEN`
- `LINE_MCP_PUSH_TARGET_USER_ID`

Re-bind the required OpenAI, Postgres, Supabase, and MCP credentials in your own n8n instance after importing a workflow. Rotate any credential that has been exposed outside its intended secret store.
