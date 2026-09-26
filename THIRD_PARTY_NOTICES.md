# Third-party notices

This repository contains third-party software and media. This inventory is
based on the files and records present in the source workspace; entries marked
unknown need provenance review before relying on them for redistribution.

## Software and fonts

- `app` uses Three.js (`three`, declared as `^0.169.0`, resolved version in
  `app/package-lock.json`) under the MIT License. Its copyright and license
  terms are in the installed package's `node_modules/three/LICENSE`.
- The app is built with Vite (`^8.3.0`, resolved version in
  `app/package-lock.json`) under the MIT License. Build tooling and transitive
  dependencies are recorded in the npm lockfile; their licenses are declared
  in that lockfile and in each package's distribution.
- `app/public/fonts/caveat.ttf` is Caveat by The Caveat Project Authors,
  licensed under the SIL Open Font License 1.1. The license text is included
  beside the font at `app/public/fonts/OFL-Caveat.txt`.

## Audio

- `design-lab/research/sound-credits.md` records these sound files as from
  Kenney's RPG Audio pack under CC0: `metalLatch.ogg`, `doorOpen_2.ogg`,
  `doorClose_1.ogg`, `creak1.ogg`, `bookPlace1.ogg`, and `bookFlip2.ogg`.
  Source: <https://kenney.nl/assets/rpg-audio>. The credit ledger says all
  files in `design-lab/sounds/` came from this pack, but it only identifies the
  six files above. That broader claim has not been independently verified.
- `cloth1.ogg`, `metalClick.ogg`, `page-turn.m4a`, and `room-tone.m4a` are also
  present in `design-lab/sounds/` and/or `app/public/sounds/`; their exact
  creator, source, and applicable license are not recorded in this workspace.
  Verify provenance before redistribution.
- `app/public/sounds/windows-xp-error.wav` is an archived Windows XP system
  sound, sourced from the direct file at
  <https://lelegofrog.github.io/lelegodlex/win/xp/Windows%20XP%20Error.wav>.
  The archive labels it “Windows XP Error.wav”; the downloaded file is RIFF
  PCM, 16-bit mono at 22,050 Hz, 44,136 bytes, SHA-256
  `4b51ec1b1b14889bc2c2cdad8c80dafc974d78b9292c3ccb344e44e93383cac4`.
  Microsoft or its licensors own applicable rights in the original sound; the
  archive provides no redistribution license. No Microsoft rights are claimed
  here; verify permission before public redistribution.

## Images and reference material

- `app/public/desktop-meadow.jpg` is an original generated landscape asset
  documented in `docs/desktop-meadow.md`; it was prompted as an original
  landscape inspired by the Windows XP era, not as a reproduction of a known
  image. `app/public/tex/desk-clean.png` is a generated edit documented in
  `docs/v10-desk-fixes.md`. These are project assets, not Microsoft artwork.
- The original room and object illustrations are maintained in
  `design-lab/assets/` and `app/public/tex/`. They were created for this
  project using supplied visual references; the repository does not establish
  ownership or license for the reference files themselves. Microsoft names,
  Windows XP interface imagery, icons, and sounds remain Microsoft or other
  rightsholders' material where applicable. This project does not claim those
  rights. Verify that each distributed asset is an original recreation or
  separately cleared before publishing it.
- `app/public/icons/photo-album.png` is the Windows XP photo-album icon
  supplied as a reference for the desktop experience. It is not claimed as an
  original work by this project; its rightsholder and permission to distribute
  it have not been verified.
- Files in `design-lab/reference/` are source/reference material and are not
  copied by the current publication script. Their individual sources and
  permissions are not catalogued here.

## External services and media

- The app loads the YouTube IFrame Player API on demand and embeds selected
  videos from `youtube-nocookie.com`. Video content is hosted by its respective
  publishers and is not licensed by this repository. Visitors' playback
  requests are subject to YouTube's terms and privacy practices.
- Note submissions are sent to FormSubmit using the public endpoint configured
  in `app/public/notes-config.json`. The repository does not control that
  service's processing or retention.

## Three.js license text (distributed runtime)

```text
The MIT License

Copyright © 2010-2024 three.js authors

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in
all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
THE SOFTWARE.
```
