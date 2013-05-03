muxkv
==========

muxkv is a command line wrapper for mkvextract, ffmpeg and sublerCLI.

It will pass the video track through and convert the audio from ac3 to aac. 

Installation:
-------------

This script relies on SublerCLI, mkvtoolnix(mkvextract) and ffmpeg
on your system.

SublerCLI is available from https://code.google.com/p/subler/downloads/detail?name=SublerCLI-0.19.zip&can=2&q=

mkvtoolnix is easiest to install through homebrew with the command "brew
install mkvtoolnix" though is also available from http://www.downloadbestsoft.com/MKVToolNix.html

ffmpef is also available through homebrew with "brew install ffmpeg" though can
be found at http://www.evermeet.cx/ffmpeg/

Once these programs have been installed this script can be downloaded through
git with "git clone https://github.com/TheProphetOfRa/muxkv.git" and then
added to your system path like the above.

Usage:
------

Open a terminal in the directory containing the file you wish to remux and
enter the command: "muxkv 'source-file.mkv' 'destination-file'"

The script will create and delete several files as it runs and output some text
to your console.

Once the file script has completed it will display "Done." and there will be
a file marked <destination-file>.mp4 in the folder.

During the "Merging the resulting audio and video." stage it may display "Error
decoding sei message". This message will not impact upon the playability of the
final file and is something to do with the frame packing of the h.264 video
file.
