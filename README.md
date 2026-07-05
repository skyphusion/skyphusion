# Conrad Rockenhaus

[`@skyphusion`](https://github.com/skyphusion) | [Skyphusion Labs](https://github.com/skyphusion-labs) | [github.skyphusion.org](https://github.skyphusion.org) (the Labs page) | [skyphusion.net](https://skyphusion.net) (engineering blog) | [skyphusion.org](https://skyphusion.org) (the lab)

Independent developer, infrastructure operator, and Navy combat veteran. I build and self-host AI tooling, mostly on Cloudflare Workers, and I run the whole stack myself.

## Not for sale, free forever

Everything I build is **open source and not for sale**. Free use forever, made with love, and developed entirely out in the open: public repos, public CI, public issue trackers, public failures next to the successes. No subscription, no account wall, no lock-in, no "open core" bait.

Open source does not mean lower standards. Every project ships with real CI gates, test suites, security review, signed-off contributions, honest documentation, and release processes that verify before they promote. I call the bar my punk ethos with an aviation-grade finish: do it yourself, answer to nobody, and build it like lives depend on the checklist. Most of it is AGPL-3.0: run a modified copy as a network service and you owe your users the source, which keeps free things free.

## What I'm building

All of it lives at **[github.com/skyphusion-labs](https://github.com/skyphusion-labs)**, with write-ups on [skyphusion.net](https://skyphusion.net).

### The Vivijure constellation (AI film studio, nearing full public release)

- **[vivijure](https://github.com/skyphusion-labs/vivijure)**: the Studio itself, a self-hosted AI film studio on Cloudflare Workers. Storyboard, cast, render orchestration, and a module registry that makes every engine below swappable. Runs on the Workers free tier. Meet it at [vivijure.skyphusion.org/welcome](https://vivijure.skyphusion.org/welcome).
- **[slate](https://github.com/skyphusion-labs/slate)**: the Discord front door. A collaborative screenwriter assistant that keeps a structured storyboard brief in channel and ships finished bundles to the Studio.
- **[vivijure-backend](https://github.com/skyphusion-labs/vivijure-backend)**: the datacenter GPU engine on RunPod. LoRA training, SDXL keyframes, Wan image-to-video, and a release gate that renders a real film before it promotes an image.
- **[vivijure-local-12gb](https://github.com/skyphusion-labs/vivijure-local-12gb)** and **[vivijure-local-16gb](https://github.com/skyphusion-labs/vivijure-local-16gb)**: own-GPU doors. Image-to-video on a single consumer card in your homelab (LTX-Video at a proven 12GB floor; CogVideoX-5B-I2V at a proven 16GB floor), reached over a Cloudflare tunnel. No rent.
- **[vivijure-musetalk](https://github.com/skyphusion-labs/vivijure-musetalk)**, **[vivijure-upscale](https://github.com/skyphusion-labs/vivijure-upscale)**, **[vivijure-audio-upscale](https://github.com/skyphusion-labs/vivijure-audio-upscale)**: the finish engines. Lip-sync, Real-ESRGAN video upscale, and speech cleanup, each a single-purpose GPU satellite.

The full map: [the constellation write-up](https://skyphusion.net/blog/vivijure-constellation/).

### Everything else

- **[prism](https://github.com/skyphusion-labs/prism)**: a multimodal AI playground in a single Cloudflare Worker. 35 chat models across five providers, voice chat, RAG, image/video/music generation, durable jobs via Workflows.
- **[postern](https://github.com/skyphusion-labs/postern)**: email for humans and agents. A self-hostable mailbox on Cloudflare: send, receive, store, search, thread, with webmail, IMAP, LDAP-backed doors, and a Go SMTP relay for legacy callers.
- **[common-thread](https://github.com/skyphusion-labs/common-thread)**: a methodology paper plus reference implementation for sockpuppet attribution from public behavioral signals. For journalists, OSINT practitioners, and researchers.
- **[the-hollow-grid](https://github.com/skyphusion-labs/the-hollow-grid)**: a multiplayer MUD on Workers and Durable Objects. Federated worlds, one shared character, ~$0 at idle. Play it: [hollow.skyphusion.org](https://hollow.skyphusion.org).
- **[mud-bots](https://github.com/skyphusion-labs/mud-bots)**: AI inhabitants of The Hollow Grid. Open-source models on Workers AI that log in like players, face the game's real moral choices, and double as live QA.
- **[SidVicious_exe](https://github.com/skyphusion-labs/SidVicious_exe)**: a punk rock Discord roadie. Claude, web search, a knowledge base, and image generation, with zero corporate sycophancy.

## The team

Skyphusion Labs is not just me. The crew each keep their own README:

- **[Mackaye][mackaye]**
- **[Rollins][rollins]**
- **[Strummer][strummer]**
- **[Joan][joan]**
- **[Ernst][ernst]**

[mackaye]: https://github.com/skyphusion-mackaye/skyphusion-mackaye
[rollins]: https://github.com/skyphusion-rollins/skyphusion-rollins
[strummer]: https://github.com/skyphusion-strummer/skyphusion-strummer
[joan]: https://github.com/skyphusion-joan/skyphusion-joan
[ernst]: https://github.com/skyphusion-ernst/skyphusion-ernst

## How I work

- Cloudflare Workers, Durable Objects, D1, R2, Workflows, and Workers AI as the default platform: cheap at idle, no servers to babysit, and the ones I do babysit are mine.
- The fleet: five dedicated CPU servers and one dedicated GPU server, all running Linux, plus several cloud VMs, the whole thing wired into a clean infrastructure-as-code stack.
- Self-hosting over SaaS wherever it makes sense. I would rather understand a system than rent it.
- Fedora Linux daily driver, Cloudflare Tunnels for inbound, nftables on the door.
- I run my own monitoring at [status.skyphusion.org](https://status.skyphusion.org), so I find out before anyone else does.

## Before all this

I served in the Navy, with deployments to Kosovo and Afghanistan attached to fire-support and signals-intelligence units. It shaped how I work: direct, prepared, and allergic to hand-waving.

## Around the web

- Engineering blog: [skyphusion.net](https://skyphusion.net)
- Skyphusion Labs: [skyphusion.org](https://skyphusion.org)
- The code: [github.com/skyphusion-labs](https://github.com/skyphusion-labs)
- Skyphusion Labs GitHub landing page: [github.skyphusion.org](https://github.skyphusion.org)
- Vivijure, the AI film studio: [vivijure.skyphusion.org/welcome](https://vivijure.skyphusion.org/welcome)
- GitHub profile: [github.com/skyphusion](https://github.com/skyphusion)
- Status: [status.skyphusion.org](https://status.skyphusion.org)
- Reach me: conrad@skyphusion.org
