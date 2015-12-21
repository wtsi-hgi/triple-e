# Triple-E

Docker and Docker Machine wrapper script...sailing with a full
complement of nautical puns.

## Usage

    3e [command]

Start or manage a Docker-aware environment. (Note that, within which,
commands that make sense are aliased for convenience.)

### `ahoy [name]`

Start the Docker host, if not already running, and enter into a
Docker-aware environment (subshell). If no name is specified, then it
will:

* Choose the single host, if only one is found;
* Prompt to create a new VirtualBox instance, if no hosts are found;
* Choose a host prioritised by running, VirtualBox and named "default"

Within the subshell, you may exit by issuing the `avast` command
(aliased with `exit`). Note that, if you run multiple subshells
simultaneously (e.g., within tmux), then closing one will invalidate the
others.

This is the default option and can be omitted.

### `avast`

**Within the Subshell** Stop all running containers and shutdown the
active machine.

**Outside the Subshell** Stop all running containers and shutdown every
running machine.

### `yarr`

**Within the Subshell** Display the active machine's IP address and the
list (and status) of its running containers.

**Outside the Subshell** Show the available machines.

### `keelhaul`

Kill all running containers on the active machine.

This option is only applicable within the subshell.

### `scuttle`

Stop and remove all running containers and remove all images on the
active machine.

This option is only applicable within the subshell.

## Zsh Autocompletion

A tab completion function for Zsh can be found as `_3e`. This can be
installed into your `$fpath` or as a plugin to [Oh-My-Zsh](http://ohmyz.sh).

### Oh-My-Zsh Plugin Installation

1. Create a `3e` plugin directory in `~/.oh-my-zsh`
2. Copy/move/symlink `_3e` into this directory
3. Add `3e` to the `plugins` list in your `.zshrc`

## License

Copyright (c) 2014, 2015 Genome Research Limited

This program is free software: you can redistribute it and/or modify it
under the terms of the GNU General Public License as published by the
Free Software Foundation, either version 3 of the License, or any later
version.

This program is distributed in the hope that it will be useful, but
WITHOUT ANY WARRANTY; without even the implied warranty of
MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the [GNU
General Public License](LICENSE) for more details.

You should have received a copy of the GNU General Public License along
with this program. If not, see <http://www.gnu.org/licenses/>.
