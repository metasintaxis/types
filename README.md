oclif-hello-world
=================

oclif example Hello World CLI

[![oclif](https://img.shields.io/badge/cli-oclif-brightgreen.svg)](https://oclif.io)
[![CircleCI](https://circleci.com/gh/oclif/hello-world/tree/main.svg?style=shield)](https://circleci.com/gh/oclif/hello-world/tree/main)
[![GitHub license](https://img.shields.io/github/license/oclif/hello-world)](https://github.com/oclif/hello-world/blob/main/LICENSE)

<!-- toc -->
* [Usage](#usage)
* [Commands](#commands)
<!-- tocstop -->
# Usage
<!-- usage -->
```sh-session
$ npm install -g @metasintaxis/types
$ @metasintaxis/types COMMAND
running command...
$ @metasintaxis/types (--version)
@metasintaxis/types/0.0.0 darwin-arm64 node-v20.10.0
$ @metasintaxis/types --help [COMMAND]
USAGE
  $ @metasintaxis/types COMMAND
...
```
<!-- usagestop -->
# Commands
<!-- commands -->
* [`@metasintaxis/types hello PERSON`](#metasintaxistypes-hello-person)
* [`@metasintaxis/types hello world`](#metasintaxistypes-hello-world)
* [`@metasintaxis/types help [COMMANDS]`](#metasintaxistypes-help-commands)
* [`@metasintaxis/types plugins`](#metasintaxistypes-plugins)
* [`@metasintaxis/types plugins:install PLUGIN...`](#metasintaxistypes-pluginsinstall-plugin)
* [`@metasintaxis/types plugins:inspect PLUGIN...`](#metasintaxistypes-pluginsinspect-plugin)
* [`@metasintaxis/types plugins:install PLUGIN...`](#metasintaxistypes-pluginsinstall-plugin-1)
* [`@metasintaxis/types plugins:link PLUGIN`](#metasintaxistypes-pluginslink-plugin)
* [`@metasintaxis/types plugins:uninstall PLUGIN...`](#metasintaxistypes-pluginsuninstall-plugin)
* [`@metasintaxis/types plugins reset`](#metasintaxistypes-plugins-reset)
* [`@metasintaxis/types plugins:uninstall PLUGIN...`](#metasintaxistypes-pluginsuninstall-plugin-1)
* [`@metasintaxis/types plugins:uninstall PLUGIN...`](#metasintaxistypes-pluginsuninstall-plugin-2)
* [`@metasintaxis/types plugins update`](#metasintaxistypes-plugins-update)

## `@metasintaxis/types hello PERSON`

Say hello

```
USAGE
  $ @metasintaxis/types hello PERSON -f <value>

ARGUMENTS
  PERSON  Person to say hello to

FLAGS
  -f, --from=<value>  (required) Who is saying hello

DESCRIPTION
  Say hello

EXAMPLES
  $ oex hello friend --from oclif
  hello friend from oclif! (./src/commands/hello/index.ts)
```

_See code: [src/commands/hello/index.ts](https://github.com/metasintaxis/types/blob/v0.0.0/src/commands/hello/index.ts)_

## `@metasintaxis/types hello world`

Say hello world

```
USAGE
  $ @metasintaxis/types hello world

DESCRIPTION
  Say hello world

EXAMPLES
  $ @metasintaxis/types hello world
  hello world! (./src/commands/hello/world.ts)
```

_See code: [src/commands/hello/world.ts](https://github.com/metasintaxis/types/blob/v0.0.0/src/commands/hello/world.ts)_

## `@metasintaxis/types help [COMMANDS]`

Display help for @metasintaxis/types.

```
USAGE
  $ @metasintaxis/types help [COMMANDS] [-n]

ARGUMENTS
  COMMANDS  Command to show help for.

FLAGS
  -n, --nested-commands  Include all nested commands in the output.

DESCRIPTION
  Display help for @metasintaxis/types.
```

_See code: [@oclif/plugin-help](https://github.com/oclif/plugin-help/blob/v6.0.12/src/commands/help.ts)_

## `@metasintaxis/types plugins`

List installed plugins.

```
USAGE
  $ @metasintaxis/types plugins [--json] [--core]

FLAGS
  --core  Show core plugins.

GLOBAL FLAGS
  --json  Format output as json.

DESCRIPTION
  List installed plugins.

EXAMPLES
  $ @metasintaxis/types plugins
```

_See code: [@oclif/plugin-plugins](https://github.com/oclif/plugin-plugins/blob/v4.2.1/src/commands/plugins/index.ts)_

## `@metasintaxis/types plugins:install PLUGIN...`

Installs a plugin into the CLI.

```
USAGE
  $ @metasintaxis/types plugins add plugins:install PLUGIN...

ARGUMENTS
  PLUGIN  Plugin to install.

FLAGS
  -f, --force    Run yarn install with force flag.
  -h, --help     Show CLI help.
  -s, --silent   Silences yarn output.
  -v, --verbose  Show verbose yarn output.

GLOBAL FLAGS
  --json  Format output as json.

DESCRIPTION
  Installs a plugin into the CLI.
  Can be installed from npm or a git url.

  Installation of a user-installed plugin will override a core plugin.

  e.g. If you have a core plugin that has a 'hello' command, installing a user-installed plugin with a 'hello' command
  will override the core plugin implementation. This is useful if a user needs to update core plugin functionality in
  the CLI without the need to patch and update the whole CLI.


ALIASES
  $ @metasintaxis/types plugins add

EXAMPLES
  $ @metasintaxis/types plugins add myplugin 

  $ @metasintaxis/types plugins add https://github.com/someuser/someplugin

  $ @metasintaxis/types plugins add someuser/someplugin
```

## `@metasintaxis/types plugins:inspect PLUGIN...`

Displays installation properties of a plugin.

```
USAGE
  $ @metasintaxis/types plugins inspect PLUGIN...

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
  $ @metasintaxis/types plugins inspect myplugin
```

_See code: [@oclif/plugin-plugins](https://github.com/oclif/plugin-plugins/blob/v4.2.1/src/commands/plugins/inspect.ts)_

## `@metasintaxis/types plugins:install PLUGIN...`

Installs a plugin into the CLI.

```
USAGE
  $ @metasintaxis/types plugins install PLUGIN...

ARGUMENTS
  PLUGIN  Plugin to install.

FLAGS
  -f, --force    Run yarn install with force flag.
  -h, --help     Show CLI help.
  -s, --silent   Silences yarn output.
  -v, --verbose  Show verbose yarn output.

GLOBAL FLAGS
  --json  Format output as json.

DESCRIPTION
  Installs a plugin into the CLI.
  Can be installed from npm or a git url.

  Installation of a user-installed plugin will override a core plugin.

  e.g. If you have a core plugin that has a 'hello' command, installing a user-installed plugin with a 'hello' command
  will override the core plugin implementation. This is useful if a user needs to update core plugin functionality in
  the CLI without the need to patch and update the whole CLI.


ALIASES
  $ @metasintaxis/types plugins add

EXAMPLES
  $ @metasintaxis/types plugins install myplugin 

  $ @metasintaxis/types plugins install https://github.com/someuser/someplugin

  $ @metasintaxis/types plugins install someuser/someplugin
```

_See code: [@oclif/plugin-plugins](https://github.com/oclif/plugin-plugins/blob/v4.2.1/src/commands/plugins/install.ts)_

## `@metasintaxis/types plugins:link PLUGIN`

Links a plugin into the CLI for development.

```
USAGE
  $ @metasintaxis/types plugins link PLUGIN

ARGUMENTS
  PATH  [default: .] path to plugin

FLAGS
  -h, --help          Show CLI help.
  -v, --verbose
      --[no-]install  Install dependencies after linking the plugin.

DESCRIPTION
  Links a plugin into the CLI for development.
  Installation of a linked plugin will override a user-installed or core plugin.

  e.g. If you have a user-installed or core plugin that has a 'hello' command, installing a linked plugin with a 'hello'
  command will override the user-installed or core plugin implementation. This is useful for development work.


EXAMPLES
  $ @metasintaxis/types plugins link myplugin
```

_See code: [@oclif/plugin-plugins](https://github.com/oclif/plugin-plugins/blob/v4.2.1/src/commands/plugins/link.ts)_

## `@metasintaxis/types plugins:uninstall PLUGIN...`

Removes a plugin from the CLI.

```
USAGE
  $ @metasintaxis/types plugins remove plugins:uninstall PLUGIN...

ARGUMENTS
  PLUGIN  plugin to uninstall

FLAGS
  -h, --help     Show CLI help.
  -v, --verbose

DESCRIPTION
  Removes a plugin from the CLI.

ALIASES
  $ @metasintaxis/types plugins unlink
  $ @metasintaxis/types plugins remove

EXAMPLES
  $ @metasintaxis/types plugins remove myplugin
```

## `@metasintaxis/types plugins reset`

Remove all user-installed and linked plugins.

```
USAGE
  $ @metasintaxis/types plugins reset [--hard] [--reinstall]

FLAGS
  --hard       Delete node_modules and package manager related files in addition to uninstalling plugins.
  --reinstall  Reinstall all plugins after uninstalling.
```

_See code: [@oclif/plugin-plugins](https://github.com/oclif/plugin-plugins/blob/v4.2.1/src/commands/plugins/reset.ts)_

## `@metasintaxis/types plugins:uninstall PLUGIN...`

Removes a plugin from the CLI.

```
USAGE
  $ @metasintaxis/types plugins uninstall PLUGIN...

ARGUMENTS
  PLUGIN  plugin to uninstall

FLAGS
  -h, --help     Show CLI help.
  -v, --verbose

DESCRIPTION
  Removes a plugin from the CLI.

ALIASES
  $ @metasintaxis/types plugins unlink
  $ @metasintaxis/types plugins remove

EXAMPLES
  $ @metasintaxis/types plugins uninstall myplugin
```

_See code: [@oclif/plugin-plugins](https://github.com/oclif/plugin-plugins/blob/v4.2.1/src/commands/plugins/uninstall.ts)_

## `@metasintaxis/types plugins:uninstall PLUGIN...`

Removes a plugin from the CLI.

```
USAGE
  $ @metasintaxis/types plugins unlink plugins:uninstall PLUGIN...

ARGUMENTS
  PLUGIN  plugin to uninstall

FLAGS
  -h, --help     Show CLI help.
  -v, --verbose

DESCRIPTION
  Removes a plugin from the CLI.

ALIASES
  $ @metasintaxis/types plugins unlink
  $ @metasintaxis/types plugins remove

EXAMPLES
  $ @metasintaxis/types plugins unlink myplugin
```

## `@metasintaxis/types plugins update`

Update installed plugins.

```
USAGE
  $ @metasintaxis/types plugins update [-h] [-v]

FLAGS
  -h, --help     Show CLI help.
  -v, --verbose

DESCRIPTION
  Update installed plugins.
```

_See code: [@oclif/plugin-plugins](https://github.com/oclif/plugin-plugins/blob/v4.2.1/src/commands/plugins/update.ts)_
<!-- commandsstop -->
