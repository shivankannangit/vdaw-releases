# Vivvy DAW

A Mac app for playing and practising music: your folders of songs and videos in one window, with a
visualizer, a waveform, markers, beats and loops, and play-along support for the Arturia MiniLab 3.

**[⬇ Download the latest version](https://github.com/shivankannangit/vivvy-releases/releases/latest)**
· Requires macOS 13 (Ventura) or later · Runs natively on Apple silicon and Intel Macs

## Features

- **Your music folders in a sidebar,** as in Finder. Move, copy, rename, tag and delete tracks from the
  app. MP3, AAC/M4A, WAV, AIFF, FLAC and MP4 video are supported.
- **Playback** with crossfade, a waveform you can scrub, and a full-screen visualizer with several
  styles. MP4 videos play in the preview panel.
- **Wave panel:** tap beats, show beat lines with a metronome, paint loop regions, save loops, and edit
  the audio.
- **Markers** with notes for any moment in a track.
- **Arturia MiniLab 3:** an on-screen keyboard, keys marked per song (with shift, transpose, start key
  and instrument), and assignable knobs, faders and pads.
- **Save from YouTube:** paste a link to save its audio as an MP3 or the video as an MP4.
- **Your data on all your Macs:** optionally keep your settings, folders and every track's marks,
  markers, beats and loops in iCloud Drive, with a backup copy on each Mac.
- **Light, Dark or System** appearance.

## Installing

1. Download the `.dmg` from the [latest release](https://github.com/shivankannangit/vivvy-releases/releases/latest).
2. Open it and drag **Vivvy DAW** onto **Applications**.
3. Open Vivvy DAW from Applications.

**The first time you open it,** macOS may say it can't verify Vivvy DAW. That's because it isn't signed
with a paid Apple Developer certificate. Open **System Settings ▸ Privacy & Security**, scroll down and
click **Open Anyway** (or Control-click Vivvy DAW in Applications and choose **Open**). You only need to
do this once.

On first launch Vivvy DAW:

- asks where to keep its data: in **iCloud Drive** (shared by your Macs, with a backup on this Mac) or
  **on this Mac only**;
- offers to **finish installing**: it downloads what saving from YouTube needs, with one progress bar.
  You can choose **Later**; the YouTube folder offers it again.

Then add your music folders with **⌘O**. Vivvy DAW also creates a **Vivvy DAW** folder in your Music
folder, where YouTube saves go.

## Updating

Download the newest `.dmg` from the [latest release](https://github.com/shivankannangit/vivvy-releases/releases/latest),
quit Vivvy DAW, then drag the new version onto Applications and choose **Replace**. Your music, settings
and track data are stored outside the app, so they're kept.

Versions are named by release date, e.g. `20261114`. A second release on the same day becomes
`20261114a`, and so on.

## Privacy

- **Your music stays where it is.** Vivvy DAW reads your folders; it never uploads them anywhere.
- **Your data is stored on your Mac,** or in your own iCloud Drive if you choose. Each track's marks,
  markers, beats and loops are also kept in a small `.vvy` file beside the track.
- **Network use:** downloading the YouTube components (from their official GitHub and ffmpeg pages), and
  YouTube itself when you save a video. There's no analytics or tracking.

## Keyboard shortcuts

| Action | Shortcut |
|---|---|
| Play / pause | Space |
| Next / previous track | ⌘→ / ⌘← |
| Back 10 s / play-pause / forward 10 s | J / K / L |
| Add a marker | M |
| Tap a beat | B |
| Full-screen visualizer | F |
| Add a folder | ⌘O |
| Save the track's MiniLab 3 settings | ⌘S |
| Show or hide Explorer / MiniLab 3 / Preview / Markers / Wave panel | ⇧⌘E / ⇧⌘K / ⇧⌘P / ⇧⌘M / ⇧⌘W |
| Show beats / markers on waveforms | ⌥B / ⌥M |

## Uninstalling

Drag **Vivvy DAW** from Applications to the Trash. To also remove its settings and downloaded
components, run this in Terminal:

```sh
rm -rf ~/Library/"Application Support/Vivvy DAW"
defaults delete com.shivankannan.vivvydaw
```

If you used iCloud, also delete the **Vivvy DAW** folder in iCloud Drive. The **Vivvy DAW** folder in your
Music folder holds your YouTube saves and any music you added there: delete it only if you no longer
want those files.

## Other apps

- **[Vmail](https://github.com/shivankannangit/vmail-releases):** several Google accounts' Gmail, Calendar and
  Drive in one window, switched in a click.
- **[Triview](https://github.com/shivankannangit/triview-releases):** preview a web page on desktop, tablet and
  mobile side by side.

---

Vivvy DAW isn't affiliated with or endorsed by Arturia or YouTube. MiniLab is a trademark of Arturia;
YouTube is a trademark of Google LLC.
