#### Author: Kiwi.com

# Kiwi.com Flight Search

This is the Kiwi.com flight search MCP server. Search and book flights directly from your favorite AI assistant!

## About this MCP Server

The [Kiwi.com](https://kiwi.com) MCP server allow you to search and book for flights using the Kiwi.com flights search engine.

The MCP server exposes a single tool: search-flight. This allows you to get instant access to a curated list of the best flights for your trip based on:

1.  Round-trip or one-way flight
2.  Origin / destination (city or airport)
3.  Travel dates
4.  Flexibility up to +/- 3 days
5.  Number and types of passengers (adult, child, infant)
6.  Cabin class (economy, premium economy, business, first class)

Simply ask your AI assistant something like:

*   “Can you help me book a first-class ticket from Paris to Rome tomorrow?”
*   “Find me the best options for our family vacation. I need a round-trip flight for my husband, me and our two children from Vienna to London, August 3 to 10.”

You can also narrow your query by choosing your preferred airport, or enlarge it by specifying that your dates are flexible. Each result includes a booking link directly to the flight chosen.

## Installation Guide

<details>
<summary>Claude Teams</summary>

### Manual steps

*Note: Only workspace owners and admins have permission to add custom connectors*

- Navigate to **Settings > Connectors**
- Toggle to **Organization connectors** at the top of the page
- At the bottom of the page, click on **Add custom connector** and fill the following information:
  - Name: `kiwi-com-flight-search`
  - Remote MCP server URL: `https://mcp.kiwi.com`

- Click **Add** to finish the setup

</details>

<details>
<summary>Claude Pro and Max</summary>
  
### Manual steps

- Navigate to **Settings > Connectors**
- Click **Add custom connector** at the bottom of the section
- Enter the URL of the remote MCP server: `https://mcp.kiwi.com`
- Click **Add** to finish the setup
- If using Claude desktop, restart to make sure changes take effect

</details>

<details>
<summary>OpenAI ChatGPT</summary>

#### Manual steps:

*Note: In Team, Enterprise, and Edu workspaces, only workspace owners and admins have permission*

- Navigate to **Settings > Connectors**
- Add a custom connector with the server URL: `https://mcp.kiwi.com`
- It should then be visible in the **Composer > Deep research** tool
- You may need to add the server as a source

*Connectors can only be used with **Deep Research***

</details>

<details>
<summary>Cursor</summary>

#### One-click installation:

Open this link in a browser: cursor://anysphere.cursor-deeplink/mcp/install?name=kiwi-com-flight-search&config=eyJ1cmwiOiJodHRwczovL21jcC5raXdpLmNvbSJ9

#### Manual steps:

- Go to **Settings > Cursor Settings > Tools & Integrations**
- Under **MCP tools**, click **Add Custom MCP**
- Paste the configuration into **mcp.json**
- Save the file to apply the configuration
- Restart **Cursor** if prompted

#### Configuration:

```json
{
  "mcpServers": {
    "kiwi-com-flight-search": {
      "url": "https://mcp.kiwi.com"
    }
  }
}
```

</details>

<details>
<summary>VS Code</summary>

#### One-click installation:

[<img src="https://img.shields.io/badge/VS_Code-VS_Code?style=flat-square&label=Install%20Server&color=0098FF" alt="Install in VS Code">](https://insiders.vscode.dev/redirect?url=vscode:mcp/install?%7B%22type%22%3A%22http%22%2C%22name%22%3A%22kiwi-com-flight-search%22%2C%22version%22%3A%220.0.1%22%2C%22description%22%3A%22This%20is%20the%20Kiwi.com%20flight%20search%20MCP%20server.%20Search%20and%20book%20flights%20directly%20from%20your%20favorite%20AI%20assistant!%22%2C%22url%22%3A%22https%3A%2F%2Fmcp.kiwi.com%22%2C%22author%22%3A%22Kiwi.com%22%2C%22tags%22%3A%5B%22kiwi-com-flight-search%22%2C%22mcp%22%2C%22server%22%5D%2C%22categories%22%3A%5B%22mcp%22%5D%7D) 
and click on **Install**

#### Manual steps:

Use the command line:

```bash
code --add-mcp '{"type":"http","name":"kiwi-com-flight-search","version":"0.0.1","description":"This is the Kiwi.com flight search MCP server. Search and book flights directly from your favorite AI assistant!","url":"https://mcp.kiwi.com","author":"Kiwi.com","tags":["kiwi-com-flight-search","mcp","server"],"categories":["mcp"]}'
```

Then go to Extensions, find the **Kiwi.com Flight Search** MCP server in the list, open the menu with right-click and click on and **Start Server**.

</details>

<details>
<summary>Claude Code</summary>

#### Manual steps:

Use the command line to add the MCP server:

```bash
claude mcp add --transport http kiwi-com-flight-search https://mcp.kiwi.com
```

</details>

<details>
<summary>Cline</summary>

#### Manual steps:

- Click on the **Cline** icon in the VSCode sidebar
- Click on the **MCP Servers** tab
- Click on the **Remote Servers** tab
- Fill in the required information:
  - Server Name: `kiwi-com-flight-search`
  - Server URL: `https://mcp.kiwi.com`
- Click **Add Server** to initiate the connection
- Cline will attempt to connect to the server and display the connection status
- If the connection is successful, click on **Done**
  
</details>

<details>
<summary>Goose</summary>

#### One-click installation:

[![Install in Goose](https://block.github.io/goose/img/extension-install-dark.svg)](https://block.github.io/goose/extension?url&#x3D;https%3A%2F%2Fmcp.kiwi.com&amp;id&#x3D;kiwi-com-flight-search-mcp-server&amp;name&#x3D;Kiwi.com%20Flight%20Search&amp;description&#x3D;This%20is%20the%20Kiwi.com%20flight%20search%20MCP%20server.%20Search%20and%20book%20flights%20directly%20from%20your%20favorite%20AI%20assistant!&amp;type&#x3D;streamable_http)

#### Manual steps:

- Go to **Extensions**
- Click on **Add custom extension**
- Fill the following information:
  - Extension Name: `kiwi-com-flight-search`
  - Type: `HTTP`
  - Description: `This is the Kiwi.com flight search MCP server. Search and book flights directly from your favorite AI assistant!`
  - Endpoint: `https://mcp.kiwi.com`
- Click **Add Extension** to finish the setup
</details>

---

Thank you!


*These installation instructions were generated by the [MCP Install Instructions Generator](https://mcp-install-instructions.alpic.cloud/) by [Alpic.ai](https://alpic.ai)*
