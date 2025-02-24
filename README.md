# HASS Google Keep (Sync)

[![Latest Version][ico-version]][link-releases]
[![Software License][ico-license]](LICENSE.md)
[![Build Status][ico-github-actions]][link-github-actions]
[![Buy us a tree][ico-treeware-gifting]][link-treeware-gifting]

A [Google Keep](https://keep.google.com) integration for [Home Assistant](https://home-assistant.io)

## Install

### Via HACS

1. Install the [Home Assistant Community Store (HACS)](https://hacs.xyz/docs/setup/download)
2. Add Oh Dear as a custom repository. See [the HACS FAQs](https://hacs.xyz/docs/faq/custom_repositories) and
   add `https://github.com/owenvoke/hass-gkeep-sync`
3. Select `integration` as the category
4. You should now be able to install Oh Dear via HACS
5. Once installation is complete, restart Home Assistant
6. In the HA UI, go to `Configuration -> Integrations`, click `+` and search for `Google Keep (Sync)`

### Manual

1. Using the tool of choice open the directory (folder) for your HA configuration (where you find `configuration.yaml`)
2. If you do not have a `custom_components` directory there, you need to create it
3. Add the `gkeep_sync` directory and its contents from this repository to the `custom_components` directory in your
   Home
   Assistant configuration directory
4. Restart Home Assistant
5. In the HA UI, go to `Configuration -> Integrations`, click `+` and search for `Google Keep (Sync)`

### Dependencies

This component relies on [gkeepapi](https://github.com/kiwiz/gkeepapi), an unofficial client for the Google Keep API.

## Usage

This can be configured fully via the Integrations interface. Click the following link to add a new Google Keep list.

[![Add Integration](https://my.home-assistant.io/badges/config_flow_start.svg)](https://my.home-assistant.io/redirect/config_flow_start?domain=gkeep_sync)

You'll need to have your email and [app password](https://myaccount.google.com/apppasswords), or a [master token](#master-token).

### Master token

Due to authentication issues with Google credentials alone it may be required to get the master token separately and
provide it during the setup process. This can be done using [this script][link-master-token-script]
or the [glocaltokens][link-glocaltokens] package.

## Security

If you discover any security related issues, please email security@voke.dev instead of using the issue tracker.

## Credits

- [Owen Voke][link-author]
- [All Contributors][link-contributors]

## License

The MIT License (MIT). Please see [License File](LICENSE.md) for more information.

## Treeware

You're free to use this package, but if it makes it to your production environment please consider buying the world a
tree.

It’s now common knowledge that one of the best tools to tackle the climate crisis and keep our temperatures from rising
above 1.5C is to plant trees. If you support this package and contribute to the Treeware forest you’ll be creating
employment for local families and restoring wildlife habitats.

You can buy trees [here][link-treeware-gifting].

Read more about Treeware at [treeware.earth][link-treeware].

[ico-version]: https://img.shields.io/github/v/release/owenvoke/hass-gkeep-sync.svg?style=flat-square&sort=semver
[ico-license]: https://img.shields.io/badge/license-MIT-brightgreen.svg?style=flat-square
[ico-github-actions]: https://img.shields.io/github/actions/workflow/status/owenvoke/hass-gkeep-sync/tests.yml?branch=main&style=flat-square
[ico-treeware-gifting]: https://img.shields.io/badge/Treeware-%F0%9F%8C%B3-lightgreen?style=flat-square

[link-master-token-script]: https://gist.github.com/rithvikvibhu/952f83ea656c6782fbd0f1645059055d
[link-glocaltokens]: https://github.com/leikoilja/glocaltokens#quickstart
[link-releases]: https://github.com/owenvoke/hass-gkeep-sync/releases
[link-github-actions]: https://github.com/owenvoke/hass-gkeep-sync/actions
[link-treeware]: https://treeware.earth
[link-treeware-gifting]: https://ecologi.com/owenvoke?gift-trees
[link-author]: https://github.com/owenvoke
[link-contributors]: ../../contributors
