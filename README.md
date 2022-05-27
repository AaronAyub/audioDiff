# audioDiff
A shell script that compares whether a given set of audio streams are completely identical. This differs from normal checksums or the diff command, in that only audio stream content is compared, and not the entire file (e.g., metadata).

To use this, run audioDiff, with at least two files passed as arguments to the script. The arguments can be video containers as well (e.g. mkv), but only the audio content will be used. The files to be compared must readable by ffmpeg.

It will return text only if there is an error, or the files do not match. If both files match, then no output is returned.

### Requirements
- ffmpeg