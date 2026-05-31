# SynTechOps

> Production-grade DevOps, server security, and full-stack engineering.
> Wyoming-registered LLC. Globally trusted.

The official marketing site for **SynTechOps LLC** — a single-file, statically-served HTML landing page showcasing real production work in DevOps, Linux server administration, security hardening, full-stack web development, and observability.

## What's Inside

- **`index.html`** — The entire site. One file. No build step. No node_modules.
- Tailwind CSS via CDN, Lucide icons via CDN, Google Fonts.
- Dark-mode design with glass morphism, gradient orbs, and smooth animations.

## Sections

- **Hero** — Top Rated badge, key metrics (49+ days uptime, 2,377 threats blocked, 100% UAT pass rate)
- **Services** — DevOps & Cloud, Linux Admin, Security & Cloudflare, Full-Stack, WordPress & PHP, Monitoring
- **About** — Engineering principles: spec-first delivery, security-hardened, fixed-fee, test-backed
- **Process** — Scope & Spec → Build & Test → UAT & Hardening → Deploy & Monitor
- **Production Stack** — Real tools we run: AWS, Hetzner, Docker, Terraform, Cloudflare, Nginx, Caddy, Grafana, Prometheus, PostgreSQL, MongoDB, Next.js, and more
- **Portfolio** — Real shipped projects: Regentic (SaaS infra), Baxter (data pipeline), Portland Flower Market (PHP rebuild), Rukhsati (full marketplace + Android TWA), plus 5 more
- **Testimonials** — Client feedback
- **Contact** — Form + email/phone/HQ

## Deployment

Deployed to Hetzner ARM (Ubuntu 22.04) behind Caddy:

```
syntechops.com, www.syntechops.com {
    root * /var/www/syntechops
    file_server
    encode gzip zstd
}
```

Caddy handles automatic Let's Encrypt SSL on first request. Cloudflare sits in front for DNS, DDoS, and WAF.

## Local Preview

Just open `index.html` in any modern browser. No build step required.

## License

© 2026 SynTechOps LLC. All rights reserved.
