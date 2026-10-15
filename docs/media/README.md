# README media

Images used by the main README. The `.png` files here are placeholders that say
"screenshot coming soon": replace each one with a real shot **at the same file name** and the
README picks it up with no edits. 16:9 looks best (1280x720 or bigger). Short GIFs work too
(rename the file and the `<img>` in README.md to `.gif`), keep them under ~10 MB.

Take shots with the HUD off.

| File | What goes there |
|---|---|
| `night-drive.gif` | done: night drive in the silver hatch (top of the README) |
| `gravel-stage.png` | a car sideways on a loose gravel stage, stones/dust flying |
| `rain.png` | a wet stage in the rain, puddles splashing |
| `cockpit.png` | in-car view with the gauges, ideally at speed |
| `psx-look.png` | a wide scenic shot that shows off the PS1/PS2 look (fog, dusk, far terrain) |
| `multiplayer.png` | two or more cars in an online race or rolling start |
| `garage.png` | the garage with a car and the parts screen |

## Clips

`clips/` holds the gameplay clips in the README's "In action" section, cut from the promo
footage. Each clip has a looping `.webp` preview (720px, 20 fps, no sound) and a 720p `.mp4` with
sound that the preview links to. `trailer.mp4` is the full promo, and `../stills.jpg` is a grid of
stills from it. To add a clip: drop a short 720p mp4 in `clips/`, make its preview with
`ffmpeg -i clip.mp4 -vf "fps=20,scale=720:-2" -an -c:v libwebp -loop 0 -q:v 72 clip.webp`,
and add it to the grid in README.md.
