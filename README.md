<p class="site-header-links">
  <a href="https://github.com/skyphusion">@skyphusion</a><span class="sep"> / </span>
  <a href="https://github.com/skyphusion-labs">Skyphusion Labs</a><span class="sep"> / </span>
  <a href="https://github.skyphusion.org">github.skyphusion.org</a> <span class="label">(Labs page)</span><span class="sep"> / </span>
  <a href="https://github.skyphusion.net">github.skyphusion.net</a> <span class="label">(this page)</span><span class="sep"> / </span>
  <a href="https://skyphusion.net">skyphusion.net</a> <span class="label">(blog)</span><span class="sep"> / </span>
  <a href="https://skyphusion.org">skyphusion.org</a> <span class="label">(lab)</span><span class="sep"> / </span>
  <a href="https://vivijure.com">vivijure.com</a><span class="sep"> / </span>
  <a href="https://demo.vivijure.com">Vivijure demo</a><span class="sep"> / </span>
  <a href="https://x.com/skyphusion">X</a><span class="sep"> / </span>
  <a href="https://www.linkedin.com/in/skyphusion/">LinkedIn</a>
</p>

Independent developer, infrastructure operator, and Navy combat veteran. I build and self-host AI tooling, mostly on Cloudflare Workers, and I run the whole stack myself.

## Not for sale, free forever

Everything I build is **open source and not for sale**. Free use forever, made with love, and developed entirely out in the open: public repos, public CI, public issue trackers, public failures next to the successes. No subscription, no account wall, no lock-in, no "open core" bait.

Open source does not mean lower standards. Every project ships with real CI gates, test suites, security review, signed-off contributions, honest documentation, and release processes that verify before they promote. I call the bar my punk ethos with an aviation-grade finish: do it yourself, answer to nobody, and build it like lives depend on the checklist. Most of it is AGPL-3.0: run a modified copy as a network service and you owe your users the source, which keeps free things free.

## What I'm building

All of it lives at **[github.com/skyphusion-labs](https://github.com/skyphusion-labs)**, with write-ups on [skyphusion.net](https://skyphusion.net).

### The Vivijure constellation (AI film studio, v1.0.0)

An AI film studio you own is also an AI film studio you can run **cheaply**, if you are deliberate about where each kind of work runs. Diffusion belongs on a GPU (your own card, RunPod serverless by the second, or a cloud i2v API). Assembly, mux, captions, portrait prep, beat analysis, and loudness work belong on CPU. Product site: [vivijure.com](https://vivijure.com).

- **[vivijure](https://github.com/skyphusion-labs/vivijure)**: constellation map and front door. Control panel on [vivijure-cf](https://github.com/skyphusion-labs/vivijure-cf) (Cloudflare) or [vivijure-local](https://github.com/skyphusion-labs/vivijure-local) (home PC / any cloud server), unified by [vivijure-core](https://github.com/skyphusion-labs/vivijure-core). Demo: [demo.vivijure.com](https://demo.vivijure.com).
- **[vivijure-cf/containers](https://github.com/skyphusion-labs/vivijure-cf/tree/main/containers)**: the always-on **CPU media stack**. Five slim Docker services (video assembly, portrait prep, beat sync, audio mastering, multi-track mix) so finishing work stays off the GPU bill.
- **[slate](https://github.com/skyphusion-labs/slate)**: the Discord front door. Collaborative screenwriter that ships finished bundles to either studio host.
- **[vivijure-backend](https://github.com/skyphusion-labs/vivijure-backend)**: the datacenter GPU engine on RunPod. LoRA training, SDXL keyframes, Wan image-to-video, release gate that renders a real film before it promotes.
- **[vivijure-local-12gb](https://github.com/skyphusion-labs/vivijure-local-12gb)** and **[vivijure-local-16gb](https://github.com/skyphusion-labs/vivijure-local-16gb)**: own-GPU doors (LTX 12GB floor; CogVideoX 16GB fidelity).
- **[vivijure-musetalk](https://github.com/skyphusion-labs/vivijure-musetalk)**, **[vivijure-upscale](https://github.com/skyphusion-labs/vivijure-upscale)**, **[vivijure-audio-upscale](https://github.com/skyphusion-labs/vivijure-audio-upscale)**: finish engines (lip-sync, video upscale, speech cleanup).

Write-ups: [runs anywhere](https://skyphusion.net/blog/vivijure-run-anywhere/), [constellation](https://skyphusion.net/blog/vivijure-constellation/).

### Everything else

- **[prism](https://github.com/skyphusion-labs/prism)**: multimodal AI playground. Public signup at [play.skyphusion.org](https://play.skyphusion.org) with per-user AI Gateway BYOK. [Write-up](https://skyphusion.net/blog/prism-public/).
- **[postern](https://github.com/skyphusion-labs/postern)** (**v1.4.1**): email for humans and agents. Webmail, IMAP, MCP, identity-bound credentials. Demo: [demo.posternonline.com](https://demo.posternonline.com). [Write-up](https://skyphusion.net/blog/postern-identity-bound/).
- **[security-audit](https://github.com/skyphusion-labs/security-audit)**: adversarial LLM PR/repo audits via Workers AI. MIT. [Write-up](https://skyphusion.net/blog/security-audit/).
- **[search-mcp](https://github.com/skyphusion-labs/search-mcp)**: Cloudflare AI Search MCP + ask widget + corpus sync.
- **[the-hollow-grid](https://github.com/skyphusion-labs/the-hollow-grid)**: federated MUD on Workers and Durable Objects. Play: [hollow.skyphusion.org](https://hollow.skyphusion.org).
- **[mud-bots](https://github.com/skyphusion-labs/mud-bots)**: AI inhabitants of The Hollow Grid.
- **[SidVicious_exe](https://github.com/skyphusion-labs/SidVicious_exe)**: punk rock Discord roadie.
- **[common-thread](https://github.com/skyphusion-labs/common-thread)**: sockpuppet attribution methodology + Workers reference (research line).

## The team

Skyphusion Labs is not just me. The crew each keep their own README:

- **[Conrad Rockenhaus](https://github.com/skyphusion)**
- **[Mackaye][mackaye]**
- **[Rollins][rollins]**
- **[Strummer][strummer]**
- **[Joan][joan]**
- **[Ernst][ernst]**

[mackaye]: https://github.com/skyphusion-mackaye
[rollins]: https://github.com/skyphusion-rollins
[strummer]: https://github.com/skyphusion-strummer
[joan]: https://github.com/skyphusion-joan
[ernst]: https://github.com/skyphusion-ernst

## How I work

- Cloudflare Workers, Durable Objects, D1, R2, Workflows, and Workers AI as the default platform: cheap at idle, no servers to babysit, and the ones I do babysit are mine.
- The fleet: five dedicated CPU servers and one dedicated GPU server, all running Linux, plus several cloud VMs, the whole thing wired into a clean infrastructure-as-code stack.
- Self-hosting over SaaS wherever it makes sense. I would rather understand a system than rent it.
- MacOS daily driver, Cloudflare Tunnels for inbound, nftables on the door.

## Before all this

I served in the Navy, with deployments to Kosovo and Afghanistan attached to fire-support and signals-intelligence units. It shaped how I work: direct, prepared, and allergic to hand-waving.

## Around the web

- Engineering blog: [skyphusion.net](https://skyphusion.net)
- Skyphusion Labs: [skyphusion.org](https://skyphusion.org)
- The code: [github.com/skyphusion-labs](https://github.com/skyphusion-labs)
- Skyphusion Labs GitHub landing page: [github.skyphusion.org](https://github.skyphusion.org)
- My GitHub landing page: [github.skyphusion.net](https://github.skyphusion.net)
- Vivijure, the AI film studio: [vivijure.com](https://vivijure.com) ([live demo](https://demo.vivijure.com))
- GitHub profile: [github.com/skyphusion](https://github.com/skyphusion)
- X: [x.com/skyphusion](https://x.com/skyphusion)
- LinkedIn: [linkedin.com/in/skyphusion](https://www.linkedin.com/in/skyphusion/)
- Reach me: [conrad@skyphusion.org](mailto:conrad@skyphusion.org)
