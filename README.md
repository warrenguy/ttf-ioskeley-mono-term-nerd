# ttf-ioskeley-mono-term-nerd

Arch package for the [Ioskeley Mono](https://github.com/ahatem/IoskeleyMono) terminal build with single-width Nerd Font icons.

`makepkg` downloads `IoskeleyMono-Term-NerdFont.zip` from the upstream release and installs the Normal and SemiCondensed faces. The glyphs are one cell wide, so terminals treat the family as monospace and arrows stay inside their cells. The package installs beside `ttf-ioskeley-mono`.

It conflicts with the outdated AUR packages `ttf-ioskeley-mono-nerd` and `ttf-ioskeley-mono-nerd-unhinted`.

## Install

```bash
makepkg -si
```
