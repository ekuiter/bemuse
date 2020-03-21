## bemuse

Takes a MuseScore 3 score and exports it into various formats (MIDI, PDF, MP3, JPG, and MP4).

### Getting Started

#### Ubuntu

```
sudo add-apt-repository ppa:mscore-ubuntu/mscore3-stable
sudo apt install imagemagick ffmpeg musescore3
git clone https://github.com/ekuiter/bemuse.git
cd bemuse
./bemuse [-w <width in px>] [-h <height in px>] [-o <audio offset in s>] <path to mscz score>
```

#### Windows/WSL

First, install MuseScore 3 as usual and add `C:\Program Files\MuseScore 3\bin\` to the `PATH` environment variable.
In cmd.exe, run:

```
wsl sudo apt install imagemagick ffmpeg
git clone https://github.com/ekuiter/bemuse.git
cd bemuse
wsl ./bemuse [-w <width in px>] [-h <height in px>] [-o <audio offset in s>] <path to mscz score>
```

Keep in mind that this will not generally work with absolute paths.
The best strategy may be to include this directory in your `PATH` and only supply relative paths.