# TLDR

Here are the setup steps for how to get this SMM system up and running. Dedicated to Chris Larco.

## Overview

1. Prereqs for PART A
2. Setting up PART A (Composition Agent)
3. Prereqs for PART B
4. Setting up PART B (Distribution Agent)
5. End-2-End Testing

## 1. Prereqs for PART A

- Sign up to Airtable (https://airtable.com/)
- Sign up to Dropbox (https://www.dropbox.com/)
- Sign up to n8n (https://n8n.io/)
- Sign up to OpenAI Platform (https://platform.openai.com/) or the Anthropic Console (https://console.anthropic.com/)

## 2. Setting up PART A - The "Composition" Agent

- Download the `n8n/Composition_Agent.json` file from GitHub (https://github.com/COMMAND-LABS/the-best-organic-smm-system-ever/blob/main/n8n/Composition_Agent.json)
    - Import the `Composition_Agent.json` workflow into n8n
    - Connect Airtable
        - Go to the Builder Hub in Airtable
            - Create a `Personal Access Token (PAT)` with the following permissions
              - `data.records:read`
              - `data.records:write`
              - `schema.bases:read`
            - Add the Airtable `PAT` to the Airtable node in n8n
            - Create an API key in the OpenAI Platform (https://platform.openai.com/)
            - Add the OpenAI API key to the OpenAI node in n8n
    - Set up the 3 Airtable tables (check out the `airtable/setup.md` doc for more info)
      - `Composition Prompts`
      - `Content`
      - `Distribution Prompts`

## 3. Prereqs for PART B

- Download & Install Node.js (https://nodejs.org/en/download)
- Download & Install uv (https://docs.astral.sh/uv/getting-started/installation/)
- Sign up to Metricool (https://metricool.com/)
  - We will need the `ADVANCED` plan is it gives you access to the Metricool API
- Download Claude for Desktop (https://claude.ai/download)

## 4. Setting up PART B - The "Distribution" Agent

- Get an API key from Metricool
  - Will be needed in the `claude_desktop_config.json` file
- Get a PAT from Airtable
  - Will be needed in the `claude_desktop_config.json` file
- Set up the `claude_desktop_config.json`
  - macOS: ~/Library/Application Support/Claude/claude_desktop_config.json
  - Windows: %APPDATA%\Claude\claude_desktop_config.json
- Here are the MCP servers needed
  - Airtable
    - https://glama.ai/mcp/servers/@domdomegg/airtable-mcp-server
    - https://github.com/domdomegg/airtable-mcp-server
  - Metricool
    - https://glama.ai/mcp/servers/@metricool/mcp-metricool
    - https://github.com/metricool/mcp-metricool

## 5. End-2-End Testing

Refer to `demo_1`, `demo_2`, and `demo_3`
