# astataudit

## introduction

 Summarizing audio metrics via ffmpeg and bwfmetaedit

From an input of a list of files or a directory, astataudit will identify is the file contains audio and if so, then generate up to four outputs:

- a csv summary of file metadata and summarizations from the astats filter
- a per-file csv output of astats frame-based metadata from astats filter
- an RDF xml containing ffprobe, astats, and bwfmetaedit metadata
- png graphs that visualize metadata from the astats and phasemeter filters

See `astataudit -h` for more info.

## dependencies

astataudit has been tested with:
- bc
- bwfmetaedit
- ffmpeg 4.3.2. Earlier versions may not work or may omit certain metadata values (such as noise floor information which was added in ffmpeg 4.3)
- ffprobe
- xmlstarlet

## install

On a Mac with homebrew: `brew install amiaopensource/amiaos/astataudit` and run like `astataudit -h`

Else:

- download the latest release at https://github.com/amiaopensource/astataudit/releases

- unpackage the download

- using terminal, change to the directory of the unpackaged download, e.g.:

  - `cd /mnt/c/users/ben/Desktop/astataudit-main` or `cd C:\Users\ben\Desktop\astataudit-main`

- run the script from here, such as `./astataudit -h`
