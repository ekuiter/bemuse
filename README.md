## bemuse

Takes a MuseScore 3 score, exports it into various formats (MIDI, PDF, MP3, JPG, and MP4) and optionally uploads it to Sheethost.

### Getting Started

#### Ubuntu

```
sudo add-apt-repository ppa:mscore-ubuntu/mscore3-stable
sudo apt install imagemagick ffmpeg jq musescore3
git clone https://github.com/ekuiter/bemuse.git
cd bemuse
./bemuse <score> # for options, see ./bemuse
```

#### Windows/WSL

First, install MuseScore 3 as usual and add `C:\Program Files\MuseScore 3\bin\` to the `PATH` environment variable.
In cmd.exe, run:

```
wsl sudo apt install imagemagick ffmpeg jq
git clone https://github.com/ekuiter/bemuse.git
cd bemuse
wsl bemuse <score> # for options, see wsl bemuse
```

Keep in mind that this will not generally work with absolute paths.
The best strategy may be to include this directory in your `PATH` and only supply relative paths.