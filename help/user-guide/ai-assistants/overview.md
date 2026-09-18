---
title: AI Assistants
description: Learn about connecting AI assistants to [!DNL GenStudio for Performance Marketing] to get insights, create drafts, and publish approved ads.
role: User
---

# AI assistants overview

[!DNL GenStudio for Performance Marketing] connects to supported AI assistants through the Model Context Protocol (MCP). Once connected, you can query ad performance, assemble creative, and publish approved ads through natural-language conversations.

## Supported AI assistants

You can connect through these supported AI assistant paths:

| AI assistant | Connection path |
|---|---|
| Adobe CX Enterprise Coworker | Native connection managed by your organization |
| Claude | Remote MCP connector |
| ChatGPT on the web | Remote MCP connector in developer mode |
| Codex | Remote MCP connection configured from the command line |
| Writer | Remote MCP custom connector |
| Microsoft Copilot | Remote MCP connection configured with Microsoft guidance |

See [Connect an AI assistant](connect-ai-assistants.md) for setup guidance.

## Capabilities

Once connected, an AI assistant can help with three areas of work:

- **Insights:** Get headline KPIs, find your best- and worst-performing ads, understand why an ad performs a certain way, and receive recommendations grounded in your performance data.
- **Create:** Browse templates, assemble an editable draft from a template or recommendation, and share the draft for review and approval.
- **Activate:** Find an approved experience, resolve its publishing target, and publish it to a connected channel.

Supported channels vary by capability. Insights covers Meta, LinkedIn, and Innovid for most reporting. Custom conversion metrics cover Meta and LinkedIn.

Create covers Meta, LinkedIn, Display, TikTok, and YouTube. Activate covers Meta, LinkedIn, and Google Campaign Manager 360. See the [AI assistant tools reference](tools-reference.md) for each tool's channel support.

## Access and permissions

AI assistant capabilities are generally available to customers enabled for [!DNL GenStudio for Performance Marketing]. You need an active Adobe account with access to the product.

The connection uses your Adobe identity and respects your existing product permissions. You can access only the organizations, paid media accounts, campaigns, and data that your account can already view.

Each connection is scoped to one Adobe Identity Management System (IMS) organization. Reconnect and select another organization when you need to switch.

## Related capabilities

- **[Connect an AI assistant](connect-ai-assistants.md)**: Connect a supported AI assistant to your account.
- **[Use AI assistants](use-ai-assistants.md)**: Explore example prompts for paid media analysis and recommendations.
- **[AI assistant tools reference](tools-reference.md)**: Review the available Insights, Create, Activate, and feedback tools.
