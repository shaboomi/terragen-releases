# TerraGen

**A complete studio for commercial pen-plotter art.** TerraGen turns a photo, code, maths or a map into a signed, editioned ink-on-paper print, all in one desktop app.

This repository holds TerraGen's installers. The source code is kept elsewhere.

## Download

The latest version is **[TerraGen 0.5.0](https://github.com/shaboomi/terragen-releases/releases/tag/v0.5.0)**:

| Platform | Installer |
|---|---|
| Windows 10/11 (x64) | [TerraGen_0.5.0_x64-setup.exe](https://github.com/shaboomi/terragen-releases/releases/download/v0.5.0/TerraGen_0.5.0_x64-setup.exe) |
| macOS (Apple silicon and Intel) | [TerraGen_0.5.0_universal.dmg](https://github.com/shaboomi/terragen-releases/releases/download/v0.5.0/TerraGen_0.5.0_universal.dmg) |
| Linux x64 (AppImage) | [TerraGen_0.5.0_amd64.AppImage](https://github.com/shaboomi/terragen-releases/releases/download/v0.5.0/TerraGen_0.5.0_amd64.AppImage) |
| Linux x64 (.deb) | [TerraGen_0.5.0_amd64.deb](https://github.com/shaboomi/terragen-releases/releases/download/v0.5.0/TerraGen_0.5.0_amd64.deb) |

Every release lists each file's SHA-256 in `SHA256SUMS.txt`. Earlier versions are on the [Releases](https://github.com/shaboomi/terragen-releases/releases) page.

### First launch

The installers are **not yet code-signed**, so your operating system will show a warning the first time you run TerraGen:

- **Windows:** SmartScreen says "Windows protected your PC". Choose **More info → Run anyway**.
- **macOS:** Gatekeeper blocks the app. Right-click TerraGen in Applications, choose **Open**, then choose **Open** again.
- **Linux:** for the AppImage, make it executable (`chmod +x TerraGen_0.5.0_amd64.AppImage`) and run it; or install the .deb with your package manager. These builds are new and untested on real machines.

All TerraGen versions so far are pre-releases.

## What TerraGen does

Today's plotter workflow usually takes three to five separate tools. TerraGen does the whole job in one app:

- **Style carousel and node graph:** pick a style and adjust it with a few sliders. Every style is also a node graph that you can open and rebuild.
- **Generators:** hatching, stippling, TSP art, flow fields, halftone, contours, spirographs, harmonographs, reaction–diffusion, mazes, Voronoi and dozens more.
- **Fields:** drive any parameter from the picture's tone, its edges, depth, noise or a painted mask.
- **Local AI:** click to segment regions, hatch along depth, remove backgrounds. The models run on your computer, and nothing is uploaded.
- **Ink-true preview:** see real pen widths and colours mixing on the paper, with a heatmap that shows where heavy ink could damage the paper.
- **Maps and terrain:** draw streets, coastlines and ridgelines of a place you choose.
- **Painting with a brush:** drive a plotter that holds a real brush and dips it in paint, with planned reloads, washes and drying waits, a painted preview and four paint styles. New in 0.5.0 and not yet run on a real machine.
- **Machine control:** supports FluidNC and GRBL plotters, among others. TerraGen estimates plot times from motion planning, guides you through pen changes, can resume a plot after a failure, and runs calibration plots.
- **Publish:** editions, signatures, title blocks, certificates of authenticity, proof sheets, framed mockups, CSV batch personalisation and costing.

TerraGen never uses the network unless you allow it. Map and terrain data are fetched only after you turn on online maps.

## Free and Pro

Generators, editing, export and plotting are **free**. A **Pro** licence key unlocks the ML styles, the paint styles and paint calibration, the Publish tools, borders, the command line and the MCP server. You enter the key under **Settings → Licence**. Each key carries an "updates until" date and unlocks every version released on or before that date.

## Licence

TerraGen is distributed under the [Functional Source License, Version 1.1, ALv2 Future License](LICENSE.md) (`FSL-1.1-ALv2`). You may use and share it for any purpose except building a competing commercial product or service. Each version becomes available under the Apache License 2.0 two years after its release.

Third-party libraries, fonts and models included in TerraGen keep their own licences. The app lists each of them, with its full licence text, in its **About** dialog.

Copyright 2026 TerraGen.
