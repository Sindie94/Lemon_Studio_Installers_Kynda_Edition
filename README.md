# Lemon Studio – Kynda Edition: installers

Ready-to-install downloads of **Lemon Studio 2026.11 (Kynda Edition)** and the **Fluxwave plugins**, by Sindiso Moyo (Kynda).

**➜ Download from the [Releases page](../../releases/latest).** This repository holds the installers only; the source
code is at [Sindie94/Lemon_Studio_Fluxwave_Version](https://github.com/Sindie94/Lemon_Studio_Fluxwave_Version).

## What to download

| You want | File |
|---|---|
| Lemon Studio for a Mac with Apple silicon (M1 or later) | `Lemon-Studio-2026.11-macOS-AppleSilicon-UNSIGNED.pkg` |
| Lemon Studio for Windows (64-bit) | `Lemon-Studio-2026.11-Windows-x64-Setup.exe` |
| Fluxwave plugins for another DAW on a Mac (VST3 and CLAP) | `Fluxwave-Plugins-macOS-VST3-CLAP.zip` |
| Fluxwave plugins as Audio Units (Logic Pro, GarageBand) | `Fluxwave-Plugins-macOS-AudioUnits.zip` |
| Fluxwave plugins for Windows (VST3 and CLAP) | `Fluxwave-Plugins-Windows.zip` |
| Fluxwave plugins for Linux (VST3 and CLAP) | `Fluxwave-Plugins-Linux.zip` |

Lemon Studio already has all of these effects and instruments built in. The Fluxwave plugins are the same ones, named
Fluxwave, for use in other DAWs (FL Studio, Ableton Live, Logic Pro, Cubase, Studio One, Reaper, Bitwig and others).
If you install them, Lemon Studio lists them too, under the maker "Fluxwave".

## Installing Lemon Studio

**Mac.** Open the `.pkg` and follow the installer; Lemon Studio goes into Applications. The installer is not signed
by Apple, so macOS may block it the first time: open **System Settings ▸ Privacy & Security** and click **Open
Anyway** for it ([Apple's guide](https://support.apple.com/en-us/102445)). Your projects and settings are kept when
you install a newer version.

**Windows.** Run the `Setup.exe`. It is not code-signed, so Windows may show "Windows protected your PC": click
**More info ▸ Run anyway**. No administrator rights are needed; it installs for your user.

## Installing the Fluxwave plugins

Unzip, then copy the plugins you want (you don't need both VST3 and CLAP):

| | VST3 | CLAP | Audio Units |
|---|---|---|---|
| Mac | `~/Library/Audio/Plug-Ins/VST3/` | `~/Library/Audio/Plug-Ins/CLAP/` | `~/Library/Audio/Plug-Ins/Components/` |
| Windows | `C:\Program Files\Common Files\VST3\` | `C:\Program Files\Common Files\CLAP\` | – |
| Linux | `~/.vst3/` | `~/.clap/` | – |

On a Mac, `~/Library` is hidden: in Finder press **Shift+Cmd+G** and paste the path. If a DAW won't load plugins
downloaded from the internet, run this in Terminal:

```
xattr -dr com.apple.quarantine ~/Library/Audio/Plug-Ins/VST3/Fluxwave* ~/Library/Audio/Plug-Ins/CLAP/Fluxwave* ~/Library/Audio/Plug-Ins/Components/Fluxwave*
```

Then rescan plugins in your DAW. Each zip also has a `READ ME.txt` with the full list of 43 plugins.

## License

Free software under the GNU General Public License v3 or later. Lemon Studio is based on the open-source
[Lemon Studio](https://github.com/ItsAlphaNeon/Lemon-Studio) by ItsAlphaNeon and contributors; this is a modified
community edition, not an official release. The matching source code is in the
[source repository](https://github.com/Sindie94/Lemon_Studio_Fluxwave_Version) and inside each installer.
