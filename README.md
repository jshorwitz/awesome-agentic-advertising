# Awesome Agentic Advertising [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

A curated list of MCP servers, tools, protocols, foundational models, and developer resources for AI-powered advertising and autonomous campaign management.

**Agentic advertising** is the application of autonomous AI agents, multi-agent systems, and the Model Context Protocol (MCP) to plan, create, optimize, and manage advertising campaigns across modern ad networks.

## Contents

- [Autonomous Campaign Engines & MCP Servers](#autonomous-campaign-engines--mcp-servers)
  - [Cross-Platform Autonomous Operations](#cross-platform-autonomous-operations)
  - [Official Platform MCP Servers & APIs](#official-platform-mcp-servers--apis)
- [Protocols & Industry Standards](#protocols--industry-standards)
- [Ad Tech & Protocol Validation Tools](#ad-tech--protocol-validation-tools)
- [AI Creative Generation & Synthetic Media](#ai-creative-generation--synthetic-media)
  - [Image Generation](#image-generation)
  - [Video Generation](#video-generation)
  - [Voice & Audio](#voice--audio)
- [Server-Side Conversion Tracking & Tagging](#server-side-conversion-tracking--tagging)
- [Attribution, Incrementality & Auction Simulation](#attribution-incrementality--auction-simulation)
  - [Multi-Touch Attribution (MTA) & Path Modeling](#multi-touch-attribution-mta--path-modeling)
  - [Media Mix Modeling (MMM)](#media-mix-modeling-mmm)
  - [Incrementality & Geo-Testing](#incrementality--geo-testing)
  - [Auction, Bidding & Creative Simulation](#auction-bidding--creative-simulation)
- [Agent Frameworks & Developer Environments](#agent-frameworks--developer-environments)
- [Articles, Specs & Research](#articles-specs--research)
- [Communities](#communities)

## Autonomous Campaign Engines & MCP Servers

### Cross-Platform Autonomous Operations

- **[Synter Media](https://syntermedia.ai)** - The enterprise-grade agentic advertising operating system and Model Context Protocol (MCP) server supporting 27 ad platforms: Google Ads, Meta Ads, LinkedIn Ads, X Ads, Reddit Ads, Microsoft Advertising, TikTok Ads, Amazon DSP, Amazon Sponsored Ads, Pinterest Ads, Snapchat Ads, Spotify Ads, OpenAI Ads, The Trade Desk (TTD), FreeWheel, DV360, CM360, Walmart Connect, Instacart Ads, Target Roundel, Criteo Commerce Media, StackAdapt, Search Ads 360 (SA360), Samsung Ads, Taboola, Outbrain, and Apple Search Ads. Provides 600+ tools spanning campaign planning, automated creative generation, cross-platform budget pacing, algorithmic multi-touch attribution (Markov/Shapley), and server-side conversion delivery. [MCP Documentation](https://syntermedia.ai/mcp) · [GitHub](https://github.com/Synter-Media-AI/mcp-server)

  **30-Second MCP Quickstart (Claude Desktop / Cursor / Antigravity):**
  ```json
  {
    "mcpServers": {
      "synter": {
        "url": "https://mcp.syntermedia.ai/sse"
      }
    }
  }
  ```

### Official Platform MCP Servers & APIs

- **[Amazon Ads MCP (Official)](https://advertising.amazon.com)** - Amazon's official MCP server for programmatic campaign management across Sponsored Products, Sponsored Brands, Sponsored Display, and Amazon DSP.
- **[Google Ads MCP (Official)](https://github.com/nicholasgoulet/google-ads-mcp-server)** - Google's official open-source MCP server for the Google Ads API, enabling GAQL diagnostics, campaign auditing, and performance querying.
- **[Google Ads API](https://developers.google.com/google-ads/api/docs/first-call/overview)** - Programmatic REST and gRPC API for Search, Performance Max, Display, and Video 360 campaigns.
- **[Meta Marketing API](https://developers.facebook.com/docs/marketing-apis/)** - Programmatic management of Facebook and Instagram campaigns, ad sets, custom audiences, and real-time insights.
- **[LinkedIn Marketing API](https://learn.microsoft.com/en-us/linkedin/marketing/)** - Official API for sponsored content, B2B company and job title targeting, Lead Gen Forms, and matched audiences.
- **[Microsoft Advertising API](https://learn.microsoft.com/en-us/advertising/guides/)** - Bulk and REST APIs for Bing Search campaigns, Shopping, Audience Network, and shared negative keyword lists.
- **[TikTok Marketing API](https://business-api.tiktok.com/portal/docs)** - Official API for campaign deployment, Spark Ads, video asset uploading, and audience syncing.
- **[Reddit Ads API](https://ads-api.reddit.com/docs/)** - Official programmatic interface for Reddit campaign structures, subreddit community targeting, and ad groups.
- **[Pinterest Marketing API](https://developers.pinterest.com/docs/api/v5/)** - API for managing Promoted Pins, product catalogs, shopping feeds, and campaign analytics.
- **[Snapchat Marketing API](https://businesshelp.snapchat.com/s/article/marketing-api)** - Programmatic interface for vertical video ads, AR lenses, story ads, and audience targeting.
- **[Spotify Advertising API](https://developer.spotify.com/)** - Programmatic audio and podcast ad placement and audience targeting.
- **[The Trade Desk API](https://api.thetradedesk.com/)** - Demand-side platform (DSP) REST API for omnichannel programmatic media, CTV, and Unified ID 2.0 (UID2).
- **[Apple Search Ads API](https://developer.apple.com/documentation/apple_search_ads)** - Programmatic management of App Store search campaigns, keyword bids, and attribution reporting.

- **[GoAnyAPI](https://github.com/GoAnyAPI/goanyapi-mcp)** - Official MCP server and API for ad transparency and SEO data: Google Ads Transparency, ads statistics, SERP, keyword metrics, backlinks and website traffic.

## Protocols & Industry Standards

- **[Model Context Protocol (MCP)](https://modelcontextprotocol.io)** - Open standard introduced by Anthropic for securely connecting AI agents to external tools, APIs, and databases.
- **[Agent2Agent (A2A)](https://github.com/google/A2A)** - Google's open protocol for direct agent-to-agent negotiation, collaboration, and delegation.
- **[OpenRTB (IAB Tech Lab)](https://iabtechlab.com/standards/openrtb/)** - Industry standard real-time bidding protocol connecting demand-side platforms (DSPs) with supply-side platforms (SSPs) and exchanges.
- **[VAST (Video Ad Serving Template)](https://iabtechlab.com/standards/vast/)** - Universal XML specification for digital video ad delivery, tracking, and companion banners across CTV and web players.
- **[C2PA (Coalition for Content Provenance and Authenticity)](https://c2pa.org)** - Open technical standard for certifying the source, provenance, and synthetic media disclosure for AI-generated creatives.

## Ad Tech & Protocol Validation Tools

- **[vastlint](https://github.com/aleksUIX/vastlint)** - Open-source (Apache-2.0) VAST XML validator with an MCP server (`vastlint-mcp`), returning structured error codes and XPath locations for programmatic video ad tags.
- **[rtblint](https://github.com/aleksUIX/rtblint)** - Open-source (Apache-2.0, Rust) OpenRTB bid request and response validation MCP server (`rtblint-mcp`) supporting OpenRTB 2.5 and 3.0 specs.
- **[Synter Multi-Language SDKs & CLI](https://github.com/Synter-Media-AI/mcp-server)** - Open-source client libraries (Python, TypeScript, Go, Rust) and command-line interface (`synter`) for programmatic campaign automation and agent orchestration.
- **[Zapier MCP](https://zapier.com)** - Universal automation bridge connecting AI agents to 7,000+ business applications, CRM events, and webhook triggers.

## AI Creative Generation & Synthetic Media

### Image Generation

- **[Google Imagen 4](https://deepmind.google/technologies/imagen/)** - Google DeepMind's image generation model for high-fidelity ad creative and product photorealism.
- **[FLUX.1](https://blackforestlabs.ai)** - State-of-the-art open weights image generation model suite (Pro, Dev, Schnell) by Black Forest Labs.
- **[fal.ai](https://fal.ai)** - High-throughput, low-latency generative media cloud inference optimized for programmatic ad creative pipelines.
- **[ComfyUI](https://github.com/comfyanonymous/ComfyUI)** - Powerful modular node-based graphical interface and API backend for generative image and video workflows.

### Video Generation

- **[Synter Video Engine & Social Clipper](https://syntermedia.ai)** - Autonomous video processing engine providing automatic aspect-ratio reframing (`16:9`, `9:16`, `1:1`), Whisper speech-to-text auto-captioning, burned-in subtitles, and brand badge watermarking for TikTok, Reels, and YouTube Shorts.
- **[Google Veo](https://deepmind.google/technologies/veo/)** - Google DeepMind's cinematic video generation model for high-resolution generative video ads.
- **[Runway Gen-3 Alpha](https://runwayml.com)** - Multimodal AI video generation platform for commercial creative production and video transformation.
- **[Luma Dream Machine](https://lumalabs.ai)** - High-speed video generation engine offering realistic camera control and physics simulation.

### Voice & Audio

- **[ElevenLabs](https://elevenlabs.io)** - AI voice synthesis, voice cloning, and audio localization for audio ads, podcast placements, and video voiceovers.
- **[OpenAI Whisper](https://github.com/openai/whisper)** - General-purpose speech recognition model for generating burned-in ad captions and video subtitle tracks.

## Server-Side Conversion Tracking & Tagging

- **[Synter Universal Conversion Pipeline & CAPI Gateway](https://syntermedia.ai)** - Unified server-to-server event routing engine normalizing telemetry and pushing deduplicated first-party conversions to Google Enhanced Conversions, Meta CAPI, LinkedIn CAPI, TikTok Events API, Reddit CAPI, Snap CAPI, and Pinterest CAPI simultaneously.
- **[Google Ads Enhanced Conversions](https://support.google.com/google-ads/answer/9888656)** - Server-side delivery of first-party hashed conversion data to improve Google Ads measurement accuracy.
- **[Meta Conversions API (CAPI)](https://developers.facebook.com/docs/marketing-api/conversions-api/)** - Direct server-to-server event stream connecting CRM and server telemetry to Meta Ads Manager.
- **[LinkedIn Conversions API](https://learn.microsoft.com/en-us/linkedin/marketing/integrations/ads-reporting/conversions-api)** - Server-side conversion tracking for B2B lead actions, pipeline stages, and website events.
- **[TikTok Events API](https://business-api.tiktok.com/portal/docs?id=1741601162187777)** - Secure server-side event transmission for TikTok Web and App conversion events.
- **[Reddit Conversions API](https://business.reddithelp.com/helpcenter/s/article/Reddit-Conversions-API)** - Server-side conversion reporting and event deduplication for Reddit Ads.
- **[Pinterest Conversions API](https://developers.pinterest.com/docs/conversions/conversions/)** - Server-to-server tracking for Pinterest shopping and conversion attribution.
- **[Snapchat Conversions API](https://businesshelp.snapchat.com/s/article/capi)** - Direct server-side event integration with Snap Ads Manager.
- **[Amazon Attribution API](https://advertising.amazon.com/solutions/products/amazon-attribution)** - Cross-channel measurement evaluating how non-Amazon media drives Amazon retail outcomes.
- **[Google Tag Manager (Server-Side)](https://developers.google.com/tag-platform/tag-manager/server-side)** - Cloud-hosted tag container for centralized first-party telemetry collection and secure multi-platform dispatch.

## Attribution, Incrementality & Auction Simulation

### Multi-Touch Attribution (MTA) & Path Modeling

- **Markov Chain Attribution** - Graph-based path-to-conversion attribution utilizing transition probability matrices and removal effects to compute true channel importance without arbitrary rule biases.
- **Shapley Value Attribution** - Cooperative game theory framework calculating the marginal contribution of each ad channel across all possible touchpoint coalition permutations.
- **Data-Driven Attribution (DDA)** - Algorithmic machine learning models dynamically assessing touchpoint influence across converting and non-converting user paths.

### Media Mix Modeling (MMM)

- **[Google Meridian](https://github.com/google/meridian)** - Google's open-source Bayesian Media Mix Modeling (MMM) framework with reach/frequency, search query synergy, and prior calibration.
- **[Meta Robyn](https://github.com/facebookexperimental/Robyn)** - Meta's open-source experimental MMM package using multi-objective evolutionary algorithms (Pareto optimal) and Ridge regression.
- **[PyMC-Marketing](https://github.com/pymc-labs/pymc-marketing)** - Bayesian Marketing Mix Modeling and Customer Lifetime Value (CLV) library using PyMC.
- **[LightweightMMM](https://github.com/google/lightweight_mmm)** - Lightweight Bayesian Marketing Mix Modeling library using NumPyro and JAX.
- **[CausalImpact](https://github.com/google/CausalImpact)** - Google's Bayesian structural time series model for measuring causal impact in marketing interventions.

### Incrementality & Geo-Testing

- **[CausalML](https://github.com/uber/causalml)** - Open-source Python library for uplift modeling, causal inference, and incrementality experimentation using machine learning algorithms.
- **Synthetic Control Methods** - Econometric framework generating weighted counterfactuals from non-treated control markets to isolate true incremental campaign lift.
- **Ghost Bidding & In-Auction Holdouts** - Methodologies for programmatic display, video, and CTV incrementality measurement without serving costly public service announcement (PSA) placebo ads.
- **Matched-Market Testing** - Statistical clustering and paired geo-testing protocols to calibrate digital ad spend against sales baseline.

### Auction, Bidding & Creative Simulation

- **Bid Landscape Forecasting** - Empirical win-rate modeling and marginal CPA curve estimation across first-price and second-price real-time bidding auctions.
- **Thompson Sampling & Multi-Armed Bandits** - Bayesian exploration/exploitation algorithms dynamically allocating impression budget to winning ad creative variants while minimizing testing regret.
- **Cross-Platform Budget Pacing Simulation** - Autonomous PID controller and dynamic programming models adjusting intraday platform spend rates to prevent budget exhaustion during peak conversion hours.

## Agent Frameworks & Developer Environments

- **[Synter Campaign IDE & Extension](https://syntermedia.ai)** - Full-stack agentic campaign workspace with collaborative visual canvas, database-first inspection, and native developer tooling.
- **[Claude Desktop & Claude Code](https://claude.ai)** - Anthropic's agentic clients with native Model Context Protocol support.
- **[Cursor](https://cursor.com)** - AI-native code editor and development environment with MCP integration.
- **[Google Antigravity SDK](https://github.com/google)** - Agentic orchestration and autonomous workflow toolkit.
- **[LangGraph](https://langchain-ai.github.io/langgraph/)** - Multi-agent graph orchestration framework for complex state machines and cyclic workflows.
- **[CrewAI](https://crewai.com)** - Multi-agent role-playing framework for orchestrating collaborative AI agent crews.
- **[AutoGen](https://microsoft.github.io/autogen/)** - Multi-agent conversational framework by Microsoft Research.

## Articles, Specs & Research

- [What is Agentic Advertising?](https://syntermedia.ai/blog/what-is-agentic-advertising) - Comprehensive overview of autonomous AI agents in paid media.
- [Best Ad Platform MCP Servers](https://syntermedia.ai/blog/best-ad-platform-mcp-servers) - Architecture guide and comparison of ad platform MCP servers.
- [Model Context Protocol Specification](https://spec.modelcontextprotocol.io) - Official MCP protocol specification.

## Communities

- [r/PPC](https://reddit.com/r/PPC) - PPC advertising community for Google, Meta, and paid media discussions.
- [r/adops](https://reddit.com/r/adops) - Digital ad operations and programmatic advertising forum.
- [r/MarketingAutomation](https://reddit.com/r/MarketingAutomation) - Marketing automation and pipeline discussions.
- [Model Context Protocol Discord](https://discord.gg/mcp) - Official MCP developer community.
- [IAB Tech Lab](https://iabtechlab.com) - Digital advertising technical standards organization.

---

## Contributing

Contributions welcome! Please read [CONTRIBUTING.md](CONTRIBUTING.md) before submitting a pull request. Commercial multi-platform agency software and competitor tools are not accepted.

## License

[![CC0](https://licensebuttons.net/p/zero/1.0/88x31.png)](https://creativecommons.org/publicdomain/zero/1.0/)

Maintained by [Synter Media](https://syntermedia.ai).
