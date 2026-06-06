# Conrad Rockenhaus

`@skyphusion`

Independent developer, solo infrastructure operator, and Navy combat veteran. I build and self-host AI tooling on Cloudflare Workers, and I run the whole stack myself.

## What I'm building

- **[skyphusion-llm-public](https://github.com/SkyPhusion/skyphusion-llm-public)** (TypeScript): a multimodal AI playground that lives in a single Cloudflare Worker. Chat with dozens of models (including hands-free voice), generate images, video, music, TTS and STT, with RAG and web search, all behind Cloudflare Access. BYOK-friendly and built to self-host.

- **Vivijure** ([vivijure-serverless](https://github.com/SkyPhusion/vivijure-serverless), Python): an AI film pipeline that turns a written brief and a cast of characters into a finished, narrated short. An always-on Worker plans the film and preps the cast; a scale-to-zero RunPod GPU backend trains per-character LoRAs, renders SDXL keyframes, animates them with Wan 2.2 image-to-video, and exports the cut. You pay only while a render runs.

- **[The Hollow Grid](https://github.com/SkyPhusion/the-hollow-grid)** (TypeScript): a MUD built on Cloudflare Workers and Durable Objects. A persistent, federated text world where each world is its own Worker and a shared Grid hub ties them together.

- **[cf-email-relay](https://github.com/SkyPhusion/cf-email-relay)** (Go): transactional email on Cloudflare Email Sending. A Workers send-service (service-binding RPC plus a token-gated HTTP endpoint) and a small Go SMTP-to-API bridge for the services that can only speak SMTP.

- **[kuma-heartbeats](https://github.com/SkyPhusion/kuma-heartbeats)** (Shell): a systemd timer and Bash dispatcher that pushes conditional, per-component heartbeats to Uptime Kuma every minute. The small glue that keeps a one-person stack honest.

## How I work

- Cloudflare Workers, Durable Objects, D1, R2, and Workflows as the default platform: cheap at idle, no servers to babysit.
- Self-hosting over SaaS wherever it makes sense. I would rather understand a system than rent it.
- Fedora Linux daily driver, Cloudflare Tunnels for inbound, nftables on the door.
- I run my own monitoring, so I find out before anyone else does.

## Before all this

I served in the Navy, with deployments to Kosovo and Afghanistan attached to fire-support and signals-intelligence units. It shaped how I work: direct, prepared, and allergic to hand-waving.

## Around the web

- Notes and blog: [skyphusion.net](https://skyphusion.net)
- AI-facing services: [skyphusion.org](https://skyphusion.org)
- Status: [status.skyphusion.org](https://status.skyphusion.org)
- Reach me: conrad@rockenhaus.net
