## bemuse

Takes a MuseScore 3 score, exports it into various formats (including a 2D visualization similar to Synthesia) and uploads the resulting files to Sheethost and YouTube.

### Getting Started

```
# Run this only on Ubuntu. On Windows, install MuseScore 3 as usual and
# add C:\Program Files\MuseScore 3\bin\ to the PATH environment variable.
sudo add-apt-repository ppa:mscore-ubuntu/mscore3-stable
sudo apt install musescore3

# on Ubuntu and Windows (run in wsl.exe)
sudo apt install imagemagick ffmpeg jq
sudo python2 -mpip install --upgrade google-api-python-client oauth2client progressbar2
git clone https://github.com/ekuiter/youtube-upload.git
cd youtube-upload
sudo python2 setup.py install
cd ..
rm -rf youtube-upload
git clone https://github.com/ekuiter/bemuse.git
cd bemuse

# on Ubuntu
./bemuse <score>

# on Windows
# Keep in mind that this will not generally work with absolute paths. The best strategy
# may be to include this directory in your `PATH` and only supply relative paths.
bemuse <score>
```

For a real-world usage example, have a look at my [sheet music for Fran Bow](https://github.com/ekuiter/fran-bow-sheet-music).