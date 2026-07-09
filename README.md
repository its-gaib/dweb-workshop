# DWeb Workshop Resources

Bandwidth will be limited during the workshop. Install the tools and start these downloads early.

## Install

- Docker: https://docs.docker.com/get-started/get-docker/
- Node.js and npm: https://docs.npmjs.com/downloading-and-installing-node-js-and-npm/
- Git, only for `git clone` commands: https://git-scm.com/downloads

## Preload Early

### 1. Pull Pubky Docker Images

Runs the local testnet and Homeserver.

- Repo: https://github.com/pubky/pubky-docker
- Docs: https://pubky.org/explore/technologies/pubky-docker/

```bash
git clone https://github.com/pubky/pubky-docker.git
(cd pubky-docker && cp .env-sample .env && docker compose pull --include-deps homeserver)
```

Do this as early as possible. This is the largest shared download.

### 2. Download App Templates

```bash
npx tiged pubky/pubky-app-templates/vite-starter pubky-hello-world
(cd pubky-hello-world && npm install && npm install @synonymdev/pubky)

npx tiged pubky/pubky-app-templates/basic-pubky-app my-pubky-app
(cd my-pubky-app && npm install)

npx tiged pubky/pubky-app-templates/pubky-signer-app pubky-signer-app
(cd pubky-signer-app && npm install)
```

## Development Guide

When we reach the hands-on part of the presentation, we will use this guide:

https://pubky.org/explore/pubkycore/getting-started/

We will only follow steps 1-3. The rest of the guide is not accurate for this workshop.

## Resources

- https://pubky.org - Main Pubky documentation and concepts.
- https://pubky.app - Social media platform built on Pubky and reference implementation.
- https://pubky.tech - Awesome list of Pubky projects, tools, and examples.

Github and packages:

- https://github.com/pubky/pubky-core/ - Pubky SDK.
- https://www.npmjs.com/package/@synonymdev/pubky - JavaScript SDK package.
- https://crates.io/crates/pubky - Rust SDK crate.
- https://github.com/pubky/ - All Pubky repositories.

Other live Pubky apps for reference:

- https://eventky.app - Event app built on Pubky.
- https://mapky.app - Map app built on Pubky.
- https://payky.app - Payment app built on Pubky.
- https://mypubky.com - Pubky social/profile app.
