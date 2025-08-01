# Gruvvy

A cool and musical system theme

## Installation

1. Clone this repository to `~/.local/share/sounds/Gruvvy`.
2. Set up your sound effects in your System Sounds, giving them the names of the files in `~/.local/share/sounds/Gruvvy/stereo/`
3. Enjoy!

## Contributing / Custom SFX

Making new SFX is very easy! Simply create a `wav` file in `src/` with the appropriate name from the [sound naming spec](https://0pointer.de/public/sound-naming-spec.html), and then run (Requires FFMPEG)

```sh
for file in *.wav; do   ffmpeg -i "$file" -af volume=1 -c:a libvorbis -b:a 128k -ar 44100 "${file%.wav}.oga"; done
```

*Note that contributing new sfx to this repository is at my discretion, due to the nature of this theme.*

## Contact

Contact me at https://winnerwind.in in case of any errors, or if you want to comment on something
