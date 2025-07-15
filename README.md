# Musicplayer

A simple *terminal based* music player (MP3, etc.) using [Textual](https://textual.textualize.io/).

## Background and reasoning

I've been countless of times been cursing over how *MacOS Music* player treating star-rating (kept outside of mp3), and for some reason when there is a glitch with e.g. your NAS where you keep your files it suddenly loose the proper file location. And not only that but experience a sluggish experience 😫

So being fed up with this, I thankfully piggyback on bluematt's initial work using a quick and rapid terminal based player that I think will solve my problem - or at least permits more easily address those myself using Python.

If anyone else found at this same spot - please feel free to try or enhance this project.

## Enhancements

The current main enhancements made to this project [bluematt/textual-musicplayer](https://github.com/bluematt/textual-musicplayer)
- Transition to [uv](https://docs.astral.sh/uv/) with advantages such as easier installation and locked dependencies
- Made into a command line tool with subcommands and `--help` 
- Star ⭐ rating based on ["POPULARIMETER"](https://id3.org/id3v2.3.0#Popularimeter) id3 tag as part of song list.
- Also comments and year added to song list
- Caching for speedup of large mp3 catalogs *(as it looks through all id3 tags)*
- Status bar been modified
- More verbose error handling such as display which mp3 files fails for whatever reason 

## Requirements

- textual - for TUI
- pygame - for music playing
- tinytag - for reading audio tags
- rich_pixel - for artwork

## Sample audio

If you have any music (currently MP3 or Ogg Vorbis) to hand, pop something into `./demo_music` to get started.

[Sample music files](https://www.soundhelix.com/audio-examples) used in the development of this app were downloaded
from [SoundHelix](https://www.soundhelix.com/). Copyright for these belongs to the appropriate artist(s).

## Basic usage/installation

```bash
uv tool install https://github.com/engdan77/musicplayer.git
musicplayer
```
