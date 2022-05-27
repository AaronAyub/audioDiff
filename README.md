# audioDiff
A shell script that compares whether a given set of audio streams are completely identical. This differs from normal checksums or the diff command, in that only audio stream content is compared, and not the entire file (e.g., metadata).

### Usage
To use this, run audioDiff, with at least two files passed as arguments to the script. The arguments can be video containers as well (e.g. mkv), but only the audio content will be used. The files to be compared must readable by ffmpeg.

If there are no errors, the script will return whether or not the file contents match.

Optionally, you can pass "-p" as the first parameter, which will print the hashes for all of the provided files.

### Requirements
- ffmpeg

### License
This script is available under the [MIT license](https://github.com/AaronAyub/audioDiff/blob/main/LICENSE).
