# Steam Play - FTEQW

If you'd like a convenient way to FTEQW in order to run games such as:

- Quake (and QuakeWorld, it'll know to differentiate)
- Quake Mission Pack 1: Scourge of Armagon
- Quake Mission Pack 2: Dissolution of Eternity
- Quake II
- Quake II Mission Pack 1: The Reckoning
- Quake II Mission Pack 2: Ground Zero
- Quake III Arena
- Quake III: Team Arena
- HeXen II

Then this is the right tool for you.

It'll play with the new re-release content by default now; if you
want it to ALWAYS start with the original, authentic content
set PLAY_RERELEASE to 0 inside fteqw_wrapper.

You will not be able to play the new expansions however if you do that!

# Dependencies
None, it expects your /bin/sh to handle arrays and things though.

If you have fteqw installed on your system (command -v fteqw) it'll use
the system binary. If you don't, it'll grab the latest 64-bit SDL2 binary
from https://www.fteqw.org that's statically linked against any third party
dependencies. It should be as easy as clicking play!

# Installation
In order to install it, you just clone
the repository into your $HOME/.steam/steam/compatibilitytools.d/ directory.

If the directory 'compatibilitytools.d' does not exist, make sure to create it.

# Special Thanks
This script will download and install game-logic from the Yamagi Quake II
project, as it has a redone save-game system that's ASLR friendly.
You are free to provide your own libraries for Quake II and its expansions!
This script will not override them.

# License

Copyright (c) 2021 Marco "eukara" Hladik

Permission to use, copy, modify, and distribute this software for any
purpose with or without fee is hereby granted, provided that the above
copyright notice and this permission notice appear in all copies.

THE SOFTWARE IS PROVIDED "AS IS" AND THE AUTHOR DISCLAIMS ALL WARRANTIES
WITH REGARD TO THIS SOFTWARE INCLUDING ALL IMPLIED WARRANTIES OF
MERCHANTABILITY AND FITNESS. IN NO EVENT SHALL THE AUTHOR BE LIABLE FOR
ANY SPECIAL, DIRECT, INDIRECT, OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES
WHATSOEVER RESULTING FROM LOSS OF MIND, USE, DATA OR PROFITS, WHETHER
IN AN ACTION OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS ACTION, ARISING
OUT OF OR IN CONNECTION WITH THE USE OR PERFORMANCE OF THIS SOFTWARE. 
