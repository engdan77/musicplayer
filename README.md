# Musicplayer

A simple music player (MP3, etc.) using [Textual](https://textual.textualize.io/).

## Enhancements

The current main enhancements made originally in this project [bluematt/textual-musicplayer](https://github.com/bluematt/textual-musicplayer)
-  Star ⭐ rating based on ["POPULARIMETER"](https://id3.org/id3v2.3.0#Popularimeter) tag in song list.
- Comments added to song list

## Requirements

- textual - for TUI
- pygame - for music playing
- tinytag - for reading audio tags
- rich_pixel - for artwork

## Sample audio

If you have any music (currently MP3 or Ogg Vorbis) to hand, pop something into `./demo_music` to get started.

[Sample music files](https://www.soundhelix.com/audio-examples) used in the development of this app were downloaded
from [SoundHelix](https://www.soundhelix.com/). Copyright for these belongs to the appropriate artist(s).

## Basic installation

```bash
uv tool install https://github.com/engdan77/musicplayer.git
musicplayer
```
