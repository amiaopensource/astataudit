# astataudit
 Summarizing audio metrics via ffmpeg and bwfmetaedit

From an input of a list of files or a directory, astataudit will identify is the file contains audio and if so, then generate up to four outputs:

- a csv summary of file metadata and summarizations from the astats filter
- a per-file csv output of astats frame-based metadata from astats filter
- an RDF xml containing ffprobe, astats, and bwfmetaedit metadata
- png graphs that visualize metadata from the astats and phasemeter filters

See `astataudit -h` for more info.