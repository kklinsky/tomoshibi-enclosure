# Tomoshibi Enclosure 灯火

3D-printable enclosure for [Tomoshibi](https://github.com/kklinsky/tomoshibi), a simple
voice companion for older adults living with memory loss.

The software, wiring and parts list live in the main
[tomoshibi](https://github.com/kklinsky/tomoshibi) repo. This repo holds only the
printed case.

> **Status:** in design. No printable files yet.

## Hardware revision

This enclosure is designed for **hardware revision `hw-rev-A`**:

| Part | Notes |
|---|---|
| Raspberry Pi 5 + active cooler | Mounted on standoffs inside the body |
| Jabra Speak 410 (USB) | Sits in a recess on top, grille facing up |
| 30 mm arcade button with built-in LED | Front face, directly below the screen |
| 2.0" 320×240 IPS TFT, ST7789 (Adafruit EYESPI) | Front face, angled ~15° up toward a seated person |

The full parts list and wiring are in
[`tomoshibi/hardware/BOM.md`](https://github.com/kklinsky/tomoshibi/blob/main/hardware/BOM.md)
and [`tomoshibi/hardware/wiring.md`](https://github.com/kklinsky/tomoshibi/blob/main/hardware/wiring.md).
If you use different parts, the enclosure will need changes.

## Design goals

- Lantern/lamp shape that reads as a friendly object, not a gadget
- Jabra on top with its grille unobstructed; a printed cover ring hides its mute/call touch keys
- Face (screen) and button on the front together, so it's obvious where to press
- Raised, contrasting bezel around the button so it's easy to find by touch and by eye
- Weighted base and rubber feet so it doesn't slide when the button is pressed
- Vents for the Pi's cooler, kept away from the Jabra's mic and speaker
- Screw-on back/base panel for service access

## Repository layout

```
source/   Fusion 360 source (.f3d) and STEP exports
print/    Print-ready STL/3MF files, one per part
docs/     Print settings, assembly guide, photos
```

## Getting the files

CAD, mesh and photo files are stored with [Git LFS](https://git-lfs.com/). Install it
before cloning:

```bash
git lfs install
git clone https://github.com/kklinsky/tomoshibi-enclosure.git
```

If you only want to print, download the STL/3MF files from the
[Releases](https://github.com/kklinsky/tomoshibi-enclosure/releases) page instead.

## Remixing

STEP files are included so you can edit the design without Fusion 360. If you adapt it
for different parts (another speakerphone, a larger button, a different screen), please
note which parts it fits in your remix's README.

## License

This enclosure design is licensed under
[Creative Commons Attribution-ShareAlike 4.0 International](https://creativecommons.org/licenses/by-sa/4.0/)
(CC BY-SA 4.0). See [LICENSE](LICENSE). You may share and adapt it, including
commercially, as long as you give credit and share your changes under the same license.

The Tomoshibi software is licensed separately; see the
[tomoshibi](https://github.com/kklinsky/tomoshibi) repo.
