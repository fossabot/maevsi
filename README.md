[![build status](https://github.com/maevsi/maevsi/workflows/Docker%20CI/badge.svg)](https://github.com/maevsi/maevsi/actions?query=workflow%3ADocker%20CI "build status")
[![renovate](https://badges.renovateapi.com/github/maevsi/maevsi)](https://renovatebot.com/ "renovate")

# mævsi - **ALPHA**

A manager for events supported by invitees: [maev.si](https://maev.si/).

<!-- ![Welcome](images/welcome.jpg "mævsi") -->

## Table of Contents
1. **[Development](#development)**
1. **[Technology](#technology)**

## Development

This project is deployed within the [maevsi_stack](https://github.com/maevsi/maevsi_stack/) in accordance to the [DargStack template](https://github.com/dargmuesli/dargstack_template/) to make deployment a breeze.


### Sqitch

The database management tool *Sqitch* needs special configuration.

- run `mkdir -p /var/run/postgresql/` to create the database's socket mount point, which Sqitch uses to connect to the database
- run `cd sqitch` from this project's root directory
- run `cp SQITCH_TARGET.env.template SQITCH_TARGET.env` and fill in the correct target
- run `./sqitch` with appropriate parameters

  (optionally, add an `alias sqitch="./sqitch"` to your shell, so that you can run `sqitch` like a binary without the preceding location indicator)


## Technology

[![Gridsome](https://gridsome.org/logos/logo-normal.svg)](https://gridsome.org/)
[![PostGraphile](https://www.graphile.org/static/postgres_postgraphile_graphql-4b238552d875fe06196ba3bda74c6d2b.png)](https://www.graphile.org/)
[![Sqitch](https://sqitch.org/img/sqitch-logo.svg)](https://sqitch.org/)
[![FOSSA Status](https://app.fossa.io/api/projects/git%2Bgithub.com%2Fmaevsi%2Fmaevsi.svg?type=shield)](https://app.fossa.io/projects/git%2Bgithub.com%2Fmaevsi%2Fmaevsi?ref=badge_shield)


## License
[![FOSSA Status](https://app.fossa.io/api/projects/git%2Bgithub.com%2Fmaevsi%2Fmaevsi.svg?type=large)](https://app.fossa.io/projects/git%2Bgithub.com%2Fmaevsi%2Fmaevsi?ref=badge_large)