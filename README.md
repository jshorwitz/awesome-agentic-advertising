# Awesome Agentic Advertising [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

A curated list of tools, MCP servers, protocols, and resources for AI-powered advertising campaign management.

**Agentic advertising** is the use of autonomous AI agents to plan, create, optimize, and manage advertising campaigns across platforms like Google Ads, Meta Ads, LinkedIn Ads, and more.

## Contents

- [MCP Servers](#mcp-servers)
  - [Cross-Platform](#cross-platform)
  - [Google Ads](#google-ads)
  - [Meta (Facebook/Instagram) Ads](#meta-facebookinstagram-ads)
  - [Amazon Ads](#amazon-ads)
  - [TikTok Ads](#tiktok-ads)
  - [LinkedIn Ads](#linkedin-ads)
  - [General Purpose](#general-purpose)
- [Protocols & Standards](#protocols--standards)
- [AI Creative Generation](#ai-creative-generation)
- [Conversion Tracking](#conversion-tracking)
- [Agent Frameworks](#agent-frameworks)
- [Articles & Resources](#articles--resources)
- [Communities](#communities)

## MCP Servers

### Cross-Platform

- **[Synter Media](https://syntermedia.ai/mcp)** - Cross-platform MCP server supporting Google, Meta, LinkedIn, Reddit, Microsoft, TikTok, X (7 platforms). 100+ tools including campaign creation, AI creative generation, and budget optimization. Open source. [GitHub](https://github.com/Synter-Media-AI/mcp-server)
- **[Adzviser](https://adzviser.com)** - Multi-platform ad data connectivity for AI agents. Supports Google Ads, Meta Ads, and more.

### Google Ads

- **[Google Ads MCP (Official)](https://github.com/nicholasgoulet/google-ads-mcp-server)** - Google's official open-source MCP server for Google Ads API. Read-only: diagnostics and analytics via GAQL queries.
- Community alternatives with read-write support exist on GitHub.

### Meta (Facebook/Instagram) Ads

- **[Pipeboard](https://pipeboard.co)** - Meta Ads MCP server (v1.0.24+). Campaign analysis, budget optimization, creative improvement. Local install or remote MCP option.

### Amazon Ads

- **[Amazon Ads MCP (Official)](https://advertising.amazon.com)** - Amazon's official MCP server (open beta, Feb 2026). Sponsored Products, Brands, and Display. Bundles multi-step workflows into single prompts.

### TikTok Ads

- **[AdsMCP](https://adsmcp.com)** - Specialized TikTok Ads MCP server. Campaign management, performance analytics, and optimization.

### LinkedIn Ads

- Available primarily through middleware platforms like Zapier MCP.
- **Apify LinkedIn Ads Scraper MCP** - Competitive intelligence and ad library data extraction.

### General Purpose

- **[Zapier MCP](https://zapier.com)** - Universal connector supporting Google Ads, Meta Ads, LinkedIn Ads, and thousands of other tools via Zapier automations.

## Protocols & Standards

- **[MCP (Model Context Protocol)](https://modelcontextprotocol.io)** - Open standard by Anthropic (Nov 2024) for connecting AI systems with external tools. The foundation for all ad platform MCP servers.
- **[AdCP (Ad Context Protocol)](https://adcp.dev)** - Open standard for advertising automation over MCP and A2A (Agent2Agent). Version 3.0 beta. Aims to standardize the full buy/sell cycle.
- **[A2A (Agent2Agent)](https://github.com/google/A2A)** - Google's agent-to-agent communication protocol. Used by AdCP for inter-agent ad operations.

## AI Creative Generation

- **[Imagen 4](https://deepmind.google/technologies/imagen/)** - Google's image generation model. Used for ad creative generation.
- **[Veo](https://deepmind.google/technologies/veo/)** - Google's video generation model. Used for video ad creation.
- **[Runway](https://runwayml.com)** - AI video generation for creative production.
- **[Luma](https://lumalabs.ai)** - AI video generation (Dream Machine).
- **[Creatify](https://creatify.ai)** - AI video generation with avatar support for UGC-style ads.
- **[Flux](https://blackforestlabs.ai)** - Open image generation model by Black Forest Labs.

## Conversion Tracking

- **[Google Ads Conversion API](https://developers.google.com/google-ads/api/docs/conversions/overview)** - Server-side conversion tracking for Google Ads.
- **[Meta Conversions API (CAPI)](https://developers.facebook.com/docs/marketing-api/conversions-api/)** - Server-side event tracking for Meta.
- **[Reddit Conversions API](https://business.reddithelp.com/helpcenter/s/article/Reddit-Conversions-API)** - Server-side conversion tracking for Reddit Ads.
- **[LinkedIn Conversions API](https://learn.microsoft.com/en-us/linkedin/marketing/integrations/ads-reporting/conversions-api)** - Server-side conversion tracking for LinkedIn.
- **[TikTok Events API](https://business-api.tiktok.com/portal/docs?id=1741601162187777)** - Server-side event tracking for TikTok.

## Agent Frameworks

- **[Claude Desktop](https://claude.ai/download)** - Anthropic's desktop client with native MCP support.
- **[Cursor](https://cursor.sh)** - AI code editor with MCP integration.
- **[Amp](https://ampcode.com)** - Sourcegraph's AI coding agent with MCP support.
- **[LangGraph](https://langchain-ai.github.io/langgraph/)** - Framework for building agentic applications.
- **[CrewAI](https://crewai.com)** - Framework for orchestrating AI agent teams.

## Articles & Resources

- [What is an Ad Platform MCP Server?](https://syntermedia.ai/blog/best-ad-platform-mcp-servers) - Comparison of all major ad platform MCP servers (Feb 2026)
- [What is Agentic Advertising?](https://syntermedia.ai/blog/what-is-agentic-advertising) - Overview of AI-agent-driven advertising
- [MCP Specification](https://spec.modelcontextprotocol.io) - Official MCP protocol specification

## Communities

- [r/PPC](https://reddit.com/r/PPC) - PPC advertising community
- [r/adops](https://reddit.com/r/adops) - Ad operations community
- [r/MarketingAutomation](https://reddit.com/r/MarketingAutomation) - Marketing automation discussions
- [MCP Discord](https://discord.gg/mcp) - Model Context Protocol community

---

## Contributing

Contributions welcome! Please read the contribution guidelines before submitting a PR.

## License

[![CC0](https://licensebuttons.net/p/zero/1.0/88x31.png)](https://creativecommons.org/publicdomain/zero/1.0/)

Maintained by [Synter Media](https://syntermedia.ai).
