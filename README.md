# Triple-E

Docker and Boot2Docker wrapper scripts...sailing with a full complement
of nautical puns.

## Usage

    3e [command]

    ahoy     Start Docker host (if not already running)
    avast    Stop Docker host
    yarr     Display the Docker host status and list running containers
    scuttle  Stop and remove all running containers and remove all images (i.e., start afresh)

## Zsh Autocompletion

A tab completion function for Zsh can be found as `_3e`. This can be
installed into your `$fpath` or as a plugin to [Oh-My-Zsh](http://ohmyz.sh).

### Oh-My-Zsh Plugin Installation

1. Create a `3e` plugin directory in `~/.oh-my-zsh`
2. Copy/move/symlink `_3e` into this directory
3. Add `3e` to the `plugins` list in your `.zshrc`

## License

Copyright (C) 2014 Genome Research Limited

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
