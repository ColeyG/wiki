# Gameboy Advance Development

## Process Documentation

- Read guide at [reinterpretcast.com](https://www.reinterpretcast.com/writing-a-game-boy-advance-game)
- Replicated the [devkitARM toolchain](https://devkitpro.org/wiki/Getting_Started)
  - Installed [pacman on Ubuntu](https://superuser.com/questions/1422797/pacman-in-ubuntu-18-04) a package manager for the binaries
  - `wget https://github.com/devkitPro/pacman/releases/download/devkitpro-pacman-1.0.1/devkitpro-pacman.deb`
  - `sudo dpkg -i devkitpro-pacman.deb`
  - `sudo dkp-pacman -S gba-dev`
- Wrote a compile script
