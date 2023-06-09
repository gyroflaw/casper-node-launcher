## Archieved
Please check https://github.com/casper-network/casper-node-launcher-js

# casper-node-launcher

The npm library for makes easy to run casper node for test purpose.

[![oclif](https://img.shields.io/badge/cli-oclif-brightgreen.svg)](https://oclif.io)
[![Version](https://img.shields.io/npm/v/oclif-hello-world.svg)](https://npmjs.org/package/oclif-hello-world)
[![License](https://img.shields.io/npm/l/oclif-hello-world.svg)](https://github.com/gyroflaw/casper-node-launcher/blob/main/package.json)

[![Open in Gitpod](https://gitpod.io/button/open-in-gitpod.svg)](https://gitpod.io/from-referrer/)

<!-- toc -->

- [casper-node-launcher](#casper-node-launcher)
- [Usage](#usage)
- [Commands](#commands)
<!-- tocstop -->

# Usage

<!-- usage -->

```sh-session
$ npm install -g casper-node-launcher
$ casper-node-launcher COMMAND
running command...
$ casper-node-launcher (--version)
casper-node-launcher/0.0.2 linux-x64 node-v16.15.1
$ casper-node-launcher --help [COMMAND]
USAGE
  $ casper-node-launcher COMMAND
...
```

<!-- usagestop -->

# Commands

<!-- commands -->

- [`casper-node-launcher config [BRANCH] [NETWORKNAME]`](#casper-node-launcher-config-branch-networkname)
- [`casper-node-launcher download [BRANCH]`](#casper-node-launcher-download-branch)
- [`casper-node-launcher help [COMMANDS]`](#casper-node-launcher-help-commands)
- [`casper-node-launcher node [BRANCH] [NETWORKNAME]`](#casper-node-launcher-node-branch-networkname)
- [`casper-node-launcher plugins`](#casper-node-launcher-plugins)
- [`casper-node-launcher plugins:install PLUGIN...`](#casper-node-launcher-pluginsinstall-plugin)
- [`casper-node-launcher plugins:inspect PLUGIN...`](#casper-node-launcher-pluginsinspect-plugin)
- [`casper-node-launcher plugins:install PLUGIN...`](#casper-node-launcher-pluginsinstall-plugin-1)
- [`casper-node-launcher plugins:link PLUGIN`](#casper-node-launcher-pluginslink-plugin)
- [`casper-node-launcher plugins:uninstall PLUGIN...`](#casper-node-launcher-pluginsuninstall-plugin)
- [`casper-node-launcher plugins:uninstall PLUGIN...`](#casper-node-launcher-pluginsuninstall-plugin-1)
- [`casper-node-launcher plugins:uninstall PLUGIN...`](#casper-node-launcher-pluginsuninstall-plugin-2)
- [`casper-node-launcher plugins update`](#casper-node-launcher-plugins-update)

## `casper-node-launcher config [BRANCH] [NETWORKNAME]`

Generate config files

```
USAGE
  $ casper-node-launcher config [BRANCH] [NETWORKNAME]

ARGUMENTS
  BRANCH       (v0.9.0|v0.9.3|v0.9.3.1|v0.9.4|v1.0.0|v1.0.1|v1.1.0|v1.1.1|v1.1.2|v1.2.0|v1.2.1|v1.3.0|v1.3.1|v1.3.2|v1.3
               .3|v1.3.4|v1.4.0|v1.4.1|v1.4.2|v1.4.3|v1.4.4|v1.4.5|v1.4.6|v1.4.8|v1.4.9|v1.4.13|v1.4.14|v1.4.15|v1.4.15-
               alt|dev) [default: v1.4.15-alt] The branch to use
  NETWORKNAME  (casper|casper-test|casper-net-1|casper-example) [default: casper-net-1] The default network name

DESCRIPTION
  Generate config files
```

_See code: [dist/commands/config.ts](https://github.com/gyroflaw/casper-node-launcher/blob/v0.0.2/dist/commands/config.ts)_

## `casper-node-launcher download [BRANCH]`

Download required assets for running casper node.

```
USAGE
  $ casper-node-launcher download [BRANCH]

ARGUMENTS
  BRANCH  (v0.9.0|v0.9.3|v0.9.3.1|v0.9.4|v1.0.0|v1.0.1|v1.1.0|v1.1.1|v1.1.2|v1.2.0|v1.2.1|v1.3.0|v1.3.1|v1.3.2|v1.3.3|v1
          .3.4|v1.4.0|v1.4.1|v1.4.2|v1.4.3|v1.4.4|v1.4.5|v1.4.6|v1.4.8|v1.4.9|v1.4.13|v1.4.14|v1.4.15|v1.4.15-alt|dev)
          [default: v1.4.15-alt] The branch to use

DESCRIPTION
  Download required assets for running casper node.
```

_See code: [dist/commands/download.ts](https://github.com/gyroflaw/casper-node-launcher/blob/v0.0.2/dist/commands/download.ts)_

## `casper-node-launcher help [COMMANDS]`

Display help for casper-node-launcher.

```
USAGE
  $ casper-node-launcher help [COMMANDS] [-n]

ARGUMENTS
  COMMANDS  Command to show help for.

FLAGS
  -n, --nested-commands  Include all nested commands in the output.

DESCRIPTION
  Display help for casper-node-launcher.
```

_See code: [@oclif/plugin-help](https://github.com/oclif/plugin-help/blob/v5.2.9/src/commands/help.ts)_

## `casper-node-launcher node [BRANCH] [NETWORKNAME]`

Starts a single Casper node.

```
USAGE
  $ casper-node-launcher node [BRANCH] [NETWORKNAME] [-d]

ARGUMENTS
  BRANCH       (v0.9.0|v0.9.3|v0.9.3.1|v0.9.4|v1.0.0|v1.0.1|v1.1.0|v1.1.1|v1.1.2|v1.2.0|v1.2.1|v1.3.0|v1.3.1|v1.3.2|v1.3
               .3|v1.3.4|v1.4.0|v1.4.1|v1.4.2|v1.4.3|v1.4.4|v1.4.5|v1.4.6|v1.4.8|v1.4.9|v1.4.13|v1.4.14|v1.4.15|v1.4.15-
               alt|dev) [default: v1.4.15-alt] The branch to use
  NETWORKNAME  (casper|casper-test|casper-net-1|casper-example) [default: casper-net-1] The default network name

FLAGS
  -d, --daemon

DESCRIPTION
  Starts a single Casper node.
```

_See code: [dist/commands/node.ts](https://github.com/gyroflaw/casper-node-launcher/blob/v0.0.2/dist/commands/node.ts)_

## `casper-node-launcher plugins`

List installed plugins.

```
USAGE
  $ casper-node-launcher plugins [--core]

FLAGS
  --core  Show core plugins.

DESCRIPTION
  List installed plugins.

EXAMPLES
  $ casper-node-launcher plugins
```

_See code: [@oclif/plugin-plugins](https://github.com/oclif/plugin-plugins/blob/v2.4.4/src/commands/plugins/index.ts)_

## `casper-node-launcher plugins:install PLUGIN...`

Installs a plugin into the CLI.

```
USAGE
  $ casper-node-launcher plugins:install PLUGIN...

ARGUMENTS
  PLUGIN  Plugin to install.

FLAGS
  -f, --force    Run yarn install with force flag.
  -h, --help     Show CLI help.
  -v, --verbose

DESCRIPTION
  Installs a plugin into the CLI.
  Can be installed from npm or a git url.

  Installation of a user-installed plugin will override a core plugin.

  e.g. If you have a core plugin that has a 'hello' command, installing a user-installed plugin with a 'hello' command
  will override the core plugin implementation. This is useful if a user needs to update core plugin functionality in
  the CLI without the need to patch and update the whole CLI.


ALIASES
  $ casper-node-launcher plugins add

EXAMPLES
  $ casper-node-launcher plugins:install myplugin

  $ casper-node-launcher plugins:install https://github.com/someuser/someplugin

  $ casper-node-launcher plugins:install someuser/someplugin
```

## `casper-node-launcher plugins:inspect PLUGIN...`

Displays installation properties of a plugin.

```
USAGE
  $ casper-node-launcher plugins:inspect PLUGIN...

ARGUMENTS
  PLUGIN  [default: .] Plugin to inspect.

FLAGS
  -h, --help     Show CLI help.
  -v, --verbose

GLOBAL FLAGS
  --json  Format output as json.

DESCRIPTION
  Displays installation properties of a plugin.

EXAMPLES
  $ casper-node-launcher plugins:inspect myplugin
```

## `casper-node-launcher plugins:install PLUGIN...`

Installs a plugin into the CLI.

```
USAGE
  $ casper-node-launcher plugins:install PLUGIN...

ARGUMENTS
  PLUGIN  Plugin to install.

FLAGS
  -f, --force    Run yarn install with force flag.
  -h, --help     Show CLI help.
  -v, --verbose

DESCRIPTION
  Installs a plugin into the CLI.
  Can be installed from npm or a git url.

  Installation of a user-installed plugin will override a core plugin.

  e.g. If you have a core plugin that has a 'hello' command, installing a user-installed plugin with a 'hello' command
  will override the core plugin implementation. This is useful if a user needs to update core plugin functionality in
  the CLI without the need to patch and update the whole CLI.


ALIASES
  $ casper-node-launcher plugins add

EXAMPLES
  $ casper-node-launcher plugins:install myplugin

  $ casper-node-launcher plugins:install https://github.com/someuser/someplugin

  $ casper-node-launcher plugins:install someuser/someplugin
```

## `casper-node-launcher plugins:link PLUGIN`

Links a plugin into the CLI for development.

```
USAGE
  $ casper-node-launcher plugins:link PLUGIN

ARGUMENTS
  PATH  [default: .] path to plugin

FLAGS
  -h, --help     Show CLI help.
  -v, --verbose

DESCRIPTION
  Links a plugin into the CLI for development.
  Installation of a linked plugin will override a user-installed or core plugin.

  e.g. If you have a user-installed or core plugin that has a 'hello' command, installing a linked plugin with a 'hello'
  command will override the user-installed or core plugin implementation. This is useful for development work.


EXAMPLES
  $ casper-node-launcher plugins:link myplugin
```

## `casper-node-launcher plugins:uninstall PLUGIN...`

Removes a plugin from the CLI.

```
USAGE
  $ casper-node-launcher plugins:uninstall PLUGIN...

ARGUMENTS
  PLUGIN  plugin to uninstall

FLAGS
  -h, --help     Show CLI help.
  -v, --verbose

DESCRIPTION
  Removes a plugin from the CLI.

ALIASES
  $ casper-node-launcher plugins unlink
  $ casper-node-launcher plugins remove
```

## `casper-node-launcher plugins:uninstall PLUGIN...`

Removes a plugin from the CLI.

```
USAGE
  $ casper-node-launcher plugins:uninstall PLUGIN...

ARGUMENTS
  PLUGIN  plugin to uninstall

FLAGS
  -h, --help     Show CLI help.
  -v, --verbose

DESCRIPTION
  Removes a plugin from the CLI.

ALIASES
  $ casper-node-launcher plugins unlink
  $ casper-node-launcher plugins remove
```

## `casper-node-launcher plugins:uninstall PLUGIN...`

Removes a plugin from the CLI.

```
USAGE
  $ casper-node-launcher plugins:uninstall PLUGIN...

ARGUMENTS
  PLUGIN  plugin to uninstall

FLAGS
  -h, --help     Show CLI help.
  -v, --verbose

DESCRIPTION
  Removes a plugin from the CLI.

ALIASES
  $ casper-node-launcher plugins unlink
  $ casper-node-launcher plugins remove
```

## `casper-node-launcher plugins update`

Update installed plugins.

```
USAGE
  $ casper-node-launcher plugins update [-h] [-v]

FLAGS
  -h, --help     Show CLI help.
  -v, --verbose

DESCRIPTION
  Update installed plugins.
```

<!-- commandsstop -->
