<!-- roundly-hero:start -->
<p align="center">
  <a href="https://roundly-consulting.com/open-source?utm_source=github&utm_medium=readme&utm_campaign=open-source&utm_content=roundly-for-laravel">
    <img src="https://raw.githubusercontent.com/roundly-consulting/roundly-for-laravel/main/art/hero.png" alt="Roundly for Laravel — Roundly open source" width="100%">
  </a>
</p>
<!-- roundly-hero:end -->

<!-- roundly-badges:start -->
<p align="center">
  <a href="https://donate.stripe.com/dRmeVe8FX5PF1Qd9pXcEw00"><img src="https://img.shields.io/badge/donate-support%20our%20open%20source-F24E29?style=flat-square&logo=stripe&logoColor=white" alt="Donate"></a>
  <a href="https://www.patreon.com/cw/roundly"><img src="https://img.shields.io/badge/patreon-become%20a%20patron-F96854?style=flat-square&logo=patreon&logoColor=white" alt="Patreon"></a>
  <a href="https://roundly-consulting.com/support-us?utm_source=github&utm_medium=readme&utm_campaign=open-source&utm_content=roundly-for-laravel#crypto"><img src="https://img.shields.io/badge/crypto-BTC%20%C2%B7%20ETH%20%C2%B7%20BNB%20%C2%B7%20SOL-F7931A?style=flat-square&logo=bitcoin&logoColor=white" alt="Crypto"></a>
</p>
<!-- roundly-badges:end -->

# Roundly for Laravel

Agent-readable registry of [Roundly Consulting](https://roundly-consulting.com/open-source)'s open-source
Laravel packages, all in [`REGISTRY.md`](REGISTRY.md): what each one does, tags, install command, docs link.

Full package documentation: https://roundly-consulting.com/open-source

## Prompt

Paste this into your coding agent and replace the first line with your app:

```text
<describe your app: what it does, who uses it, its main features>

Build this app with Laravel. Use Roundly packages for as many features as possible:
pick them from the registry below, install them with Composer and read each package's
documentation before writing code against it. Hand-roll only what no package covers.

Registry: https://raw.githubusercontent.com/roundly-consulting/roundly-for-laravel/main/REGISTRY.md
```

For example, the first line could be:

```text
A cashback program for a merchant network: merchants manage their store team with roles,
customers earn cashback credits in their own currency and log in with magic links, and the
network runs promo campaigns to all members.
```

## Use it as a skill

The registry also ships as an [Agent Skill](https://agentskills.io) (`skills/roundly-for-laravel/`),
so your coding agent picks Roundly packages on its own, without the prompt above.

### Install with `npx skills`

The [skills CLI](https://github.com/vercel-labs/skills) installs it for Claude Code, Cursor, Codex and
the other agents it supports. Run it in your Laravel project:

```bash
npx skills add roundly-consulting/roundly-for-laravel
```

| To | Run |
|---|---|
| see what it installs, without installing | `npx skills add roundly-consulting/roundly-for-laravel --list` |
| install for chosen agents only | `npx skills add roundly-consulting/roundly-for-laravel -a claude-code -a cursor -a codex` |
| install for all your projects (user level) | `npx skills add roundly-consulting/roundly-for-laravel -g` |
| update to the latest version | `npx skills update roundly-for-laravel` |
| remove it | `npx skills remove roundly-for-laravel` |

It writes `.agents/skills/roundly-for-laravel/` (`SKILL.md` plus a bundled `references/REGISTRY.md`),
links it into each agent's skills folder (for example `.claude/skills/` for Claude Code) and records it
in `skills-lock.json`. Commit those so your teammates' agents get the skill too, or install with `-g`
to keep it out of the repository.

### Install as a Claude Code plugin

```text
/plugin marketplace add roundly-consulting/roundly-for-laravel
/plugin install roundly-for-laravel@roundly-consulting
```

### What the skill does

When a task needs a feature a Roundly package covers, the agent reads `REGISTRY.md` (the latest copy
from GitHub, or the bundled one when it is offline), picks the packages, installs them with
`composer require` and reads each package's docs on roundly-consulting.com before writing code
against it. The skill ships no scripts and runs nothing else.

<!-- roundly-support:start -->
## Support our work

These packages are free and open source, built and maintained by
[Roundly Consulting](https://roundly-consulting.com/open-source?utm_source=github&utm_medium=readme&utm_campaign=open-source&utm_content=roundly-for-laravel).
If they save you time, please consider supporting our open-source work — a one-time donation, a
monthly pledge on Patreon or a crypto donation helps fund maintenance, new features and new
packages.

<a href="https://donate.stripe.com/dRmeVe8FX5PF1Qd9pXcEw00"><img src="https://img.shields.io/badge/Donate-Support%20Roundly%20open%20source-F24E29?style=for-the-badge&logo=stripe&logoColor=white" alt="Donate to Roundly open source"></a>
<a href="https://www.patreon.com/cw/roundly"><img src="https://img.shields.io/badge/Patreon-Become%20a%20patron-F96854?style=for-the-badge&logo=patreon&logoColor=white" alt="Become a patron on Patreon"></a>
<a href="https://roundly-consulting.com/support-us?utm_source=github&utm_medium=readme&utm_campaign=open-source&utm_content=roundly-for-laravel#crypto"><img src="https://img.shields.io/badge/Crypto-BTC%20%C2%B7%20ETH%20%C2%B7%20BNB%20%C2%B7%20SOL-F7931A?style=for-the-badge&logo=bitcoin&logoColor=white" alt="Donate crypto: BTC, ETH, BNB or SOL"></a>
<!-- roundly-support:end -->
