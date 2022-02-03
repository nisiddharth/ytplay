# ytplay

A simple bash script to play YouTube videos from terminal.

Supports:
- Music only playback
- List of search results to select from
- Play on infinite loop

## Screenshots

|With video|Without video|
|----|----|
|![Screenshot with video](./screenshots/with-video.png)|![Screenshot without video](./screenshots/music-only.png)|

*Lyrics on the right shown using [lyrics-in-terminal](https://github.com/Jugran/lyrics-in-terminal).*

## Requirements

`mpv`, `youtube-dl`, `jq`, `curl`, `awk` and `fzf`.

## Usage

```
ytplay [OPTION] query

OPTIONS:
	-m, --music                Music only mode. No video playback.
	-t, --top                  Play the top search result. No options presented.
	-l, --loop                 Play the media on an infinite loop
	-r, --results COUNT        Specify the number of options to be presented
	-h, --help                 Show this help
```

## Install

Copy [ytplay](ytplay) to your `~/.local/bin` directory, like so:

```bash
curl https://raw.githubusercontent.com/nisiddharth/ytplay/main/ytplay > ~/.local/bin/ytplay && chmod +x ~/.local/bin/ytplay
```