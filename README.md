# TLDR

Accompanying repo for the "Best Organic Social Media Marketing System Ever" YouTube video

## How to setup the system

1. Sign up for a free Airtable account
2. Set up Airtable table according to the `airtable/setup.md` doc
3. Sign up for an n8n account
4. Import the `n8n/Composition_Agent.json` & `n8n/Campaign_Composition_Agent.json` workflows into n8n
  - 2-week FREE trial followed by ~$20/month
5. Sign up for free Dropbox account
6. Sign up for Advanced Metricool account
  - 2-week FREE trial followed by ~$45/month
7. Download `Claude for Desktop`
8. Connect `Claude for Desktop` to the needed Airtable & Metricool MCP servers (MAKE SURE TO AUDIT THE MCP SERVERS)
    - https://glama.ai/mcp/servers/@domdomegg/airtable-mcp-server
    - https://github.com/domdomegg/airtable-mcp-server
    - https://glama.ai/mcp/servers/@metricool/mcp-metricool
    - https://github.com/metricool/mcp-metricool

## Diagrams

Peep `diagrams/SMM_team_of_agents.png`

## Agent A Components (Composition Agent)

- `Airtable` (https://airtable.com/)
- `Dropbox` (https://www.dropbox.com/)
- `n8n` (https://n8n.io/)
- `OpenAI` (https://platform.openai.com/) or `Anthropic API` (https://console.anthropic.com/)

## Agent B Components (Distribution Agent)

- `Airtable` (https://airtable.com/)
- `Dropbox` (https://www.dropbox.com/)
- `Metricool` (https://metricool.com/)
- `Claude for Desktop` (https://claude.ai/download)

## MCP

- https://docs.anthropic.com/en/docs/mcp
- On Mac, you configure the MCP setup in the `~/Library/Application Support/Claude/claude_desktop_config.json` file
