### Download

https://drive.google.com/open?id=0B-gPKiJYuKuITld4dzhuTC1WWWM

http://1drv.ms/1OqPDOe

### New Features

- added setting to prevent the StaxRip window to become the active foreground window if certain applications are currently in the foreground
- added new option to disable audio and subtitle demuxing
- added subtitle formats column to MediaInfo Folder View
- added all missing x265 switches
- added hardware decoding methods to x265 'Other' tab, this will bypass AviSynth though
- added new standalone mkvextract GUI (Apps > Demux)
- added new QSVEncC switches for hardcoded subtitles
- added MP4 support to standalone demux app
- added -avsinfo starting AVSMeter without a source opened
- added support for unicode filenames using VapourSynth, AviSynth don't support it
- added mkv cutting support without encoding
- added MSharpen x64 filter for AviSynth+ x64
- added x264 10-Bit support, binary is not included, StaxRip will ask for the location
- added ffmpeg codecs x264, x265 and ProRes
- added codec help menu to ffmpeg options dialog which shows help for the currently selected codec, it displayes the output queried with 'ffmpeg -h encoder=name'
- added option to define preferred audio languages
- added audio and subtitle demuxing modes 'Show Dialog', 'Preferred', 'All', 'None'
- added x265 changes for v1.9 183

### Fixed Bugs

- custom switches were missing in the Intel Quick Sync encoding GUI for QSVEncC
- fixed crash with ass file by replacing VSFilter with VSFilterMod

### Tweaks

- the batch audio profile uses now always batch execution, the PATH variable knows the location of ffmpeg, eac3to and BeSweet, the temp files directory is set as current directory, if input files is empty all files are excepted 
- the search feature of the apps dialog searches now also the supported filters of plugins
- enabled audio demuxing using MP4Box for mov files
- removed mkvinfo.exe which is 18 MB large and not really needed. It's large due to QT toolkit being used
- mkv audio demuxing happens now all streams together instead of every stream separate, it's much faster now.
- changed filter profiles editor to support both tab and 4 spaces for multiline profiles, tabs are converted to 4 spaces which is the standard in Python and Visual Studio
- log file improvements
- filters list view did not accept drag and drop with source files 
- enabled posibility to remux mov to mp4
- the apps dialog writes the customized versions now to the settings folder so it don't matter if the startup folder has no write access

### Updated Tools

- AviSynth 1847
- ffmpeg 2016-04-25
- L-SMASH-Works 877
- mkvtoolnix 9.1.0
- MP4Box 0.6.2
- mvsfunc 7
- mvtools2 2.7.0.22
- nnedi3 0.9.4.21
- NVEncC 2.06
- QSVEncC 2.47
- StaxRip Toolbox Demux 1.1
- x265 1.9 183