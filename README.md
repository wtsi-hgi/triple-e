# Triple-E

Docker and Docker Machine wrapper scripts...sailing with a full
complement of nautical puns.

## Usage

    3e [command]

    ahoy      Start Docker host (if not already running)
    avast     Stop active Docker host
    yarr      Display the Docker host status and list running containers
    keelhaul  Kill all running containers on the active host
    scuttle   Stop and remove all running containers and remove all images (i.e., start afresh)

**Note** A shell script cannot affect the environment of its host (i.e.,
the calling shell). As such, when a Docker machine is brought up, the
necessary environment variables must be set manually by calling:

    eval "$(docker-machine env [name])"

An ugly-but-workable solution, if you're using Docker mainly on your
client machine (i.e., `default` is the Docker Machine you're primarily
working with), is creating an alias in your shell rc:

    alias eee='3e ahoy && eval "$(docker-machine env default)" &>/dev/null'

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
