# 🚀 Deploy and hosting reviews · Best of Vibe Coding

Self-hosted platforms that deploy and run your apps from Git or Docker on your own servers. Back to the [leaderboard](../README.md#-deploy-and-hosting).

<sub>🌐 Also on the web: [Deploy and hosting on archestack.com](https://archestack.com/best-of-vibe-coding/deploy/), each project on its own page.</sub>

<a name="dokploy"></a>
### 🥇 [dokploy](https://github.com/dokploy/dokploy) <sub>score [87](../README.md#-how-we-rank "Score 87/100. Adoption: widely used (93) · Freshness: active (100) · Maintenance: healthy (84) · Easy to run: very easy (83) · Agent-ready: partly (55) (each out of 100, weighted). Click for how we rank.") · ⭐ 38k · custom license · Oct 2026</sub>

**Self-hosted PaaS for deploying apps and databases across Docker Swarm nodes.**

Dokploy is a self-hostable platform-as-a-service that deploys applications, Docker Compose stacks and databases (MySQL, PostgreSQL, MongoDB, MariaDB, libsql, Redis) to your own servers. It uses Traefik for routing, Docker Swarm for multi-node scaling, and offers one-click open-source templates, database backups to external storage, and a CLI and API. It has no AI-specific features, so it fits as deployment infrastructure for apps built elsewhere.

- **+** Installs on a VPS with a single curl script
- **+** Native Docker Compose and Docker Swarm multi-node support
- **+** Built-in database backups, monitoring and deploy notifications
- **+** Exports logs and metrics to Grafana, Datadog, Splunk, CloudWatch and others
- **−** License is reported as NOASSERTION; terms need checking before commercial use
- **−** README gives no minimum RAM or CPU requirements
- **−** No AI features; general-purpose deployment tool only
- **−** Hosted Dokploy Cloud is offered alongside; feature split with self-hosted not stated

<sub>no GPU · Docker · Needs Docker, Docker Swarm, Traefik · [Repo](https://github.com/dokploy/dokploy) · [▶️ Demo ↗](https://app.dokploy.com) · [📖 Docs ↗](https://docs.dokploy.com) · [🌐 Site ↗](https://dokploy.com) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/dokploy/)</sub>

<a name="dokku"></a>
### 🥈 [dokku](https://github.com/dokku/dokku) <sub>score [69](../README.md#-how-we-rank "Score 69/100. Adoption: known (41) · Freshness: active (100) · Maintenance: healthy (92) · Easy to run: easy (67) · Agent-ready: none (0) (each out of 100, weighted). Click for how we rank.") · ⭐ 32k · MIT · Oct 2026</sub>

**Self-hosted mini-Heroku PaaS that deploys apps with git push.**

Dokku is a small Platform-as-a-Service that runs on a single Ubuntu or Debian VM and builds and runs applications in Docker containers. Applications are deployed over SSH, and the server is managed through the `dokku` command line, including domains and SSH keys. The README describes it as a Docker-powered mini-Heroku and does not mention any AI features.

- **+** Installs on a single VM with one bootstrap script
- **+** Supports Ubuntu 22.04/24.04/26.04 and Debian 11+ on amd64 and arm64
- **+** MIT license, with an active release history and Ubuntu and Arch packages
- **+** Written in Go, with documentation and a Slack support channel
- **−** Not an AI project; the README has no AI or model features
- **−** Targets one server; the README describes no multi-node setup
- **−** Only Ubuntu and Debian are listed as supported operating systems
- **−** Deployment and management are CLI and SSH based; the README mentions no web UI

<sub>Docker · Needs Docker, SSH keypair · [Repo](https://github.com/dokku/dokku) · [📖 Docs ↗](https://dokku.com/docs/getting-started/installation/) · [🌐 Site ↗](https://dokku.com) · [📊 Score breakdown ↗](https://archestack.com/best-of-vibe-coding/projects/dokku/)</sub>

<sub>Written from each project README and checked facts; see [how this works](../README.md#-how-this-works). Wrong? [Tell us](https://github.com/archestack/best-of-vibe-coding/issues/new/choose).</sub>
