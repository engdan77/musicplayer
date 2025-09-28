# Musicplayer

A simple *terminal based* music player (MP3, etc.) using [Textual](https://textual.textualize.io/).

![MusicPlayer_2025-09-28T20_32_11_158220](https://raw.githubusercontent.com/engdan77/project_images/master/pics/MusicPlayer_2025-09-28T20_32_11_158220.svg)

## Background and reasoning

I've been countless of times been cursing over how *MacOS Music* player treating star-rating (kept outside of mp3), and for some reason when there is a glitch with e.g. your NAS where you keep your files it suddenly loose the proper file location. And not only that but experience a sluggish experience 😫

So being fed up with this, I thankfully piggyback on bluematt's initial work using a quick and rapid terminal based player that I think will solve my problem - or at least permits more easily address those myself using Python.

If anyone else found at this same spot - please feel free to try or enhance this project.

## Enhancements

The current main enhancements made to this project [bluematt/textual-musicplayer](https://github.com/bluematt/textual-musicplayer)

:white_check_mark: Transition to [uv](https://docs.astral.sh/uv/) with advantages such as easier installation and locked dependencies

:white_check_mark: Made into a command line tool with subcommands and `--help` 

:white_check_mark: ​Replace id3-tag package from tinytag to eyeD3

:white_check_mark: Star ⭐ rating based on ["POPULARIMETER"](https://id3.org/id3v2.3.0#Popularimeter) id3 tag as part of song list.

:white_check_mark: Also comments and year added to song list

:white_check_mark: Caching for speedup of large mp3 catalogs *(as it looks through all id3 tags)*

:white_check_mark: Statusbar has been updated

:white_check_mark: Verbose error handling such as display which mp3 files fails for whatever reason 

:white_check_mark: More advanced search including comparison operators e.g. "> <1988 foo" to filter all songs rated more than 4 stars, older than 1988 and containing "foo" in artist, title or comment.

:white_check_mark: Updated to Textual >=6.1.0

:white_check_mark: Supports updating comment ID3-tag of tack (press "c")

:white_check_mark: Update star rating (press 0-5)

:white_check_mark: Copy current filtered MP3 tracks to a new path (press "y")


## Requirements

- textual - for TUI
- pygame - for music playing
- eyed3 - for reading audio tags
- rich_pixel - for artwork

## Basic usage/installation

```bash
uv tool install https://github.com/engdan77/musicplayer.git
musicplayer
```
