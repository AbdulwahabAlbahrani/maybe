
<img width="1440" alt="dashboard_mockup" src="https://github.com/maybe-finance/maybe/assets/35243/a7763d0e-a942-42db-bde7-eb8d28106917">
<sup><i>(Note: The image above is a mockup of what we're working towards. We're rapidly approaching the functionality shown, but not all of the parts are ready just yet.)</i></sup>

# Maybe: The OS for your personal finances

the idea of this repo is to try and add the saudi rial simpol

<b>Get
involved: [Discord](https://link.maybe.co/discord) • [Website](https://maybefinance.com) • [Issues](https://github.com/maybe-finance/maybe/issues)</b>

## Backstory

We spent the better part of 2021/2022 building a personal finance + wealth
management app called, Maybe. Very full-featured, including an "Ask an Advisor"
feature which connected users with an actual CFP/CFA to help them with their
finances (all included in your subscription).

The business end of things didn't work out, and so we shut things down mid-2023.

We spent the better part of $1,000,000 building the app (employees +
contractors, data providers/services, infrastructure, etc.).

We're now reviving the product as a fully open-source project. The goal is to
let you run the app yourself, for free, and use it to manage your own finances
and eventually offer a hosted version of the app for a small monthly fee.

## Maybe Hosting

There are 3 primary ways to use the Maybe app:

1. Managed (easiest) - we're in alpha and release invites in our Discord
2. [Self-host with Docker](docs/hosting/docker.md)

## Contributing

Before contributing, you'll likely find it helpful
to [understand context and general vision/direction](https://github.com/maybe-finance/maybe/wiki).

Once you've done that, please visit
our [contributing guide](https://github.com/maybe-finance/maybe/blob/main/CONTRIBUTING.md)
to get started!

## Local Development Setup

**If you are trying to _self-host_ the Maybe app, stop here. You
should [read this guide to get started](docs/hosting/docker.md).**

The instructions below are for developers to get started with contributing to the app.

### Requirements

- See `.ruby-version` file for required Ruby version
- PostgreSQL >9.3 (ideally, latest stable version)

After cloning the repo, the basic setup commands are:

```sh
cd maybe
cp .env.local.example .env.local
bin/setup
bin/dev

# Optionally, load demo data
rake demo_data:reset
```

And visit http://localhost:3000 to see the app. You can use the following
credentials to log in (generated by DB seed):

- Email: `user@maybe.local`
- Password: `password`

For further instructions, see guides below.

### Multi-currency support

If you'd like multi-currency support, there are a few extra steps to follow.

1. Sign up for an API key at [Synth](https://synthfinance.com). It's a Maybe
   product and the free plan is sufficient for basic multi-currency support.
2. Add your API key to your `.env` file.

### Setup Guides

- [Mac dev setup guide](https://github.com/maybe-finance/maybe/wiki/Mac-Dev-Setup-Guide)
- [Linux dev setup guide](https://github.com/maybe-finance/maybe/wiki/Linux-Dev-Setup-Guide)
- [Windows dev setup guide](https://github.com/maybe-finance/maybe/wiki/Windows-Dev-Setup-Guide)
- Dev containers - visit [this guide](https://code.visualstudio.com/docs/devcontainers/containers) to learn more

## Repo Activity

![Repo Activity](https://repobeats.axiom.co/api/embed/7866c9790deba0baf63ca1688b209130b306ea4e.svg "Repobeats analytics image")

## Copyright & license

Maybe is distributed under
an [AGPLv3 license](https://github.com/maybe-finance/maybe/blob/main/LICENSE). "
Maybe" is a trademark of Maybe Finance, Inc.
