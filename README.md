# Mockuuups MCP Server

The **Mockuuups MCP Server** brings the power of the Model Context Protocol (MCP) to your design workflow, letting you generate stunning mockups instantly—right from your favorite AI chat or automation tool.

## Why Mockuuups MCP?

- **No more context switching:** Create mockups directly in Claude, ChatGPT, or any MCP-compatible tool.
- **Supercharge your workflow:** Automate mockup creation in Make.com, Zapier, and more.
- **For designers, marketers, and developers:** Save time, stay in flow, and deliver beautiful visuals faster.


## Quick Start

1. **Create a Free Developer Account:**  
   [Sign up at Mockuuups Developer Portal](https://mockuuups.studio/api/) to get your API key (50 free credits).

2. **Connect to Your AI Tool:**  
   - **MCP Endpoint URL:** `https://mcp.mockuuups.studio/mcp`
   - **Fallback SSE Endpoint:** `https://mcp.mockuuups.studio/sse` (for older tools)
   - **API Key:** Paste your key when prompted.

3. **Start Generating Mockups:**  
   Just ask your AI assistant, e.g.:  
   > "Take a screenshot of Theverge.com and put it on an iPhone 16 mockup."


## Prerequisites

- A Mockuuups Developer API key ([get one here](https://mockuuups.studio/api/))
- An MCP-compatible host (Claude, ChatGPT, VS Code, etc.)


## Installation

### In Claude, ChatGPT, or Other AI Tools

- Go to "Connect Apps" or "Add Integration" in your tool's settings.
- Enter:
  - **Tool Name:** Mockuuups
  - **MCP Endpoint URL:** `https://mcp.mockuuups.studio/mcp`
  - **API Key:** Your Mockuuups API key

### In Make.com, Zapier, or Custom Automation

- Use the same endpoint and API key in your HTTP or MCP module.
- See [automation examples](https://mockuuups.studio/blog/post/automate-pinterest-content/).


## Configuration

- **API Key:** Found in your Mockuuups Developer dashboard.
- **Endpoints:**
  - MCP: `https://mcp.mockuuups.studio/mcp`
  - SSE (legacy): `https://mcp.mockuuups.studio/sse`


## Tool Reference

The Mockuuups MCP exposes the following tools:

- **generate_mockup**  
  Generate a mockup from a URL or image, specifying device, scene, or mockup ID.

  **Parameters:**
  - `image_url` or `screenshot_url`
  - `mockup_id` (optional)

  **Returns:**  
  - URL to the generated mockup image


## Example Prompts

- "Take this image `[your-public-image-url.png]` and put it on a phone held by a woman."
- "Show me how Dribbble.com looks on a television in a living room."
- "Put a screenshot of new Mockuuups landing on a MacBook Pro on a desk."
- "Put this design `[your-public-image-url.png]` into mockup `ZvMSqqPA3wFkHM3Y`."
