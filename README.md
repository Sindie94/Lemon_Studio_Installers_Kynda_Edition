# Lemon Studio – Kynda Edition: installers

Ready-to-install downloads of **Lemon Studio 2026.11 (Kynda Edition)**, a free music production app (DAW) by
Sindiso Moyo (Kynda). All the instruments and effects are built in.

This repository holds the installers only; the source code is at
[Sindie94/Lemon_Studio_Kynda_Edition](https://github.com/Sindie94/Lemon_Studio_Kynda_Edition).

## Download

| Your computer | Download |
|---|---|
| Mac with Apple silicon (M1 or later), macOS 11 or newer | [Lemon-Studio-2026.11-macOS-AppleSilicon-UNSIGNED.pkg](https://github.com/Sindie94/Lemon_Studio_Installers_Kynda_Edition/raw/main/2026.11/Lemon-Studio-2026.11-macOS-AppleSilicon-UNSIGNED.pkg) (30 MB) |
| Windows 10 or 11, 64-bit | [Lemon-Studio-2026.11-Windows-x64-Setup.exe](https://github.com/Sindie94/Lemon_Studio_Installers_Kynda_Edition/raw/main/2026.11/Lemon-Studio-2026.11-Windows-x64-Setup.exe) (22 MB) |
| Linux, 64-bit (Ubuntu 22.04, Debian 12, Fedora 36 or newer) | [Lemon-Studio-2026.11-Linux-x86_64.tar.gz](https://github.com/Sindie94/Lemon_Studio_Installers_Kynda_Edition/raw/main/2026.11/Lemon-Studio-2026.11-Linux-x86_64.tar.gz) (13 MB) |

Checksums are in [2026.11/SHA256SUMS.txt](2026.11/SHA256SUMS.txt).

## Installing

**Mac.** Open the `.pkg` and follow the installer; Lemon Studio goes into Applications. The installer is not signed
by Apple, so macOS may block it the first time: open **System Settings ▸ Privacy & Security** and click **Open
Anyway** for it ([Apple's guide](https://support.apple.com/en-us/102445)).

**Windows.** Run the `Setup.exe`. It is not code-signed, so Windows may show "Windows protected your PC": click
**More info ▸ Run anyway**. No administrator rights are needed; it installs for your user.

**Linux.** Unpack the archive, then in a terminal in its folder run `./install.sh`. Lemon Studio appears in your
app menu (installed in `~/.local`; `sudo ./install.sh --system` installs it for every user). Audio goes through ALSA,
so PipeWire and PulseAudio work too.

Your projects and settings are kept when you install a newer version.

## New in 2026.11

- Direct offline processing on a clip or just the highlighted part: tape stop and tape start (like Pro Tools Vari-Fi
  and Logic speed fades), fades, gain, normalize, reverse, pitch shift, spectral de-noise and any effect plugin
- Remove silence, highlighting across tracks, auto fades, and Pro Tools / Cubase editing keys
- Recording while playing (punch in at the playhead)
- A help manual with pictures: [Lemon Studio Help.pdf](https://github.com/Sindie94/Lemon_Studio_Kynda_Edition/raw/main/docs/Lemon%20Studio%20Help.pdf)

## Thank you

This Kynda Edition would not exist without others sharing their work:

- **ItsAlphaNeon and the Lemon Studio team**, who created [Lemon Studio](https://github.com/ItsAlphaNeon/Lemon-Studio)
  and share it as free software. Everything here is built on their work.
- **Michael Lane**, who shared the files of his customized edition of Lemon Studio, which this edition continues.

## License

Free software under the GNU General Public License v3 or later. Lemon Studio is based on the open-source
[Lemon Studio](https://github.com/ItsAlphaNeon/Lemon-Studio) by ItsAlphaNeon and contributors; this is a modified
community edition, not an official release. The matching source code is in the
[source repository](https://github.com/Sindie94/Lemon_Studio_Kynda_Edition).
