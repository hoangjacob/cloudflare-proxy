# Cloudflare Worker: Simple Reverse Proxy

This Cloudflare Worker acts as a lightweight reverse proxy that forwards requests from one hostname to another.  
It’s useful for custom domains, bypassing CORS restrictions, or transparently mirroring another site through your Cloudflare Worker.

---

## Features

- **Hostname rewriting:** Automatically redirects incoming requests to target origins.
- **Transparent proxying:** Preserves request methods, headers, and bodies.

---

## How It Works

When a user visits your Worker URL (e.g. `https://cubari.jacob-hoang2010.workers.dev`),  
the script intercepts the request, rewrites the hostname, and fetches the corresponding content from the target domain (e.g. `https://cubari.moe`).
