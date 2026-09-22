---
title: Connect an AI Assistant
description: Learn how to connect a supported AI assistant to [!DNL GenStudio for Performance Marketing] and verify access to available tools.
role: User
---

# Connect an AI assistant

Connect a supported AI assistant to [!DNL GenStudio for Performance Marketing] before you query performance data, assemble drafts, or publish approved ads. Connection options vary by AI assistant and organization.

## Prerequisites

Before you connect, confirm that you have:

- An active Adobe account with access to [!DNL GenStudio for Performance Marketing].
- A supported plan that allows remote MCP connections when you use Claude, ChatGPT, or Microsoft Copilot. Refer to the AI assistant documentation for specific instructions on manually configuring MCP connections.

## Connect Adobe CX Enterprise Coworker

[!DNL GenStudio for Performance Marketing] tools are managed as a native connection in Adobe CX Enterprise Coworker. Your organization controls availability, so you do not enter the direct MCP server URL.

Start a new conversation and [verify the connection](#verify-the-connection). If the tools do not appear, contact your organization's administrator or Adobe representative.

## Connect Claude

Claude requires a Pro, Max, Team, or Enterprise plan. The same remote connector works in Claude on the web and in the desktop application.

1. In Claude, select **[!UICONTROL Customize]** in the left sidebar.
1. Select **[!UICONTROL Connectors]**, then select the add icon.
1. Select **[!UICONTROL Add custom connector]**.
1. Enter `https://genstudio-services.adobe.io/mcp` as the MCP server URL.
1. Sign in with your Adobe ID.
1. Select the IMS organization that has access to [!DNL GenStudio for Performance Marketing].

>[!NOTE]
>
>On a Team or Enterprise plan, an organization owner might need to add the connector first. If the connector is already available, select **[!UICONTROL Connect]** instead.

## Connect ChatGPT

ChatGPT requires a Plus, Pro, Business, Enterprise, or Education account. Custom MCP connections are available on the web through developer mode.

1. Sign in to [ChatGPT](https://chatgpt.com) in a web browser.
1. Open **[!UICONTROL Settings]**, then enable **[!UICONTROL Developer mode]**.
1. In **[!UICONTROL Settings]**, open the area for apps or connectors.
1. Add a custom MCP connection named `GenStudio`.
1. Enter `https://genstudio-services.adobe.io/mcp` as the MCP server URL.
1. Keep **[!UICONTROL OAuth]** as the authentication method.
1. Sign in with your Adobe ID.
1. Select the IMS organization that has access to [!DNL GenStudio for Performance Marketing].

>[!NOTE]
>
>ChatGPT can change the location of developer and connector settings. If these labels differ in your account, follow the current OpenAI instructions for adding a remote MCP connector.

## Connect Codex

Codex requires the Codex command-line interface and an authenticated Codex account.

1. Open `~/.codex/config.toml` for all projects or `.codex/config.toml` for one project.
1. Add this configuration:

   ```toml
   [mcp_servers.genstudio]
   url = "https://genstudio-services.adobe.io/mcp"
   auth = "oauth"
   ```

1. Run `codex mcp login genstudio`.
1. Sign in with your Adobe ID in the browser window that opens.
1. Select the IMS organization that has access to [!DNL GenStudio for Performance Marketing].

## Connect Writer

Writer requires access to AI Studio.

1. In Writer, open **[!UICONTROL AI Studio]**.
1. Select **[!UICONTROL Connectors & Tools]**.
1. Select **[!UICONTROL Create custom connector]**.
1. Select **[!UICONTROL MCP Server]** as the connector type.
1. Enter a name and description for the connector.
1. Enter `https://genstudio-services.adobe.io/mcp` as the MCP server URL.
1. Set the connector's team access.
1. Select **[!UICONTROL OAuth 2.0 (user-level)]** as the authentication method.
1. Sign in with your Adobe ID.
1. Select **[!UICONTROL Save]**.

[!DNL GenStudio for Performance Marketing] tools appear in the AI Studio tool library. Each Writer user signs in with an individual Adobe ID.

## Connect Microsoft Copilot

Microsoft controls the setup flow for custom MCP connections in Copilot. Follow the current [Microsoft Copilot documentation](https://learn.microsoft.com/en-us/copilot/) to add a remote MCP server, then use `https://genstudio-services.adobe.io/mcp` as the server URL.

When prompted, sign in with your Adobe ID and select the IMS organization that has access to [!DNL GenStudio for Performance Marketing].

## Verify the connection

After setup, confirm that the tools are available.

1. Start a new conversation in your AI assistant.
1. Ask the assistant which [!DNL GenStudio for Performance Marketing] tools it can access.
1. Confirm that the response lists tools across Insights, Create, and Activate.
1. Ask for a performance summary for a connected paid media channel.

The assistant returns available performance data or explains why no data matches the request.

>[!TIP]
>
>If authentication fails, reconnect and confirm that you selected the correct IMS organization. If no tools appear, confirm that your account has access to [!DNL GenStudio for Performance Marketing].

## Related capabilities

- [AI assistants overview](overview.md)
- [Use AI assistants](use-ai-assistants.md)
- [AI assistant tools reference](tools-reference.md)
