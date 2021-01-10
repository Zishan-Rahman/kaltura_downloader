# Videos Downloader for websites using Moodle along with Kaltura as a video host

> :warning: This project is very WIP, the link to the video page or the video itself might not be recognised.
> This project is a fork of a fork of the original repository so our programs may not work together in the future.
> I'm probably not even gonna work on this anymore so feel free to try out the other forks! 🙃
> Since this is a fork of a fork, most of the text that uses the first person refers to [POPLOPUK](https://github.com/POPLOPUK/) and not me.

This is a project intended to automatically download all videos in a course and store them locally. My aim has been merging [memst's](https://github.com/memst/keats_downloader) and [dylantjb's](https://github.com/dylantjb/keats_downloader) code into one single script easy to use script that any user can run without having to understand the code along with my edits.
Benefits include:

- Being able to playback videos at speeds the Kaltura player doesn't allow you
- Being able to use subtitles as a semi-accurate transcript
- Being able to watch high-resolution video streams with no buffering
- Offline download for those with bad internet connections.

## Todo (this section is for [Zishan](https://github.com/Zishan-Rahman/kaltura_downloader))

- Basically wait until [POPLOPUK](https://github.com/POPLOPUK/kaltura_downloader) does everything he wants to do (I plan to either merge his changes into my fork or vice versa)
- Get this darn thing working on my computer! All I did so far was comment out 2 lines, and soon I uncommented those lines again because the program just stopped working (for some reason)! 🙃
- Maybe delete this repository?
  
## Confirmed working on

- Keats

## Requirements

1. To install the python modules used by the project run the following in the directory.

```pip3 install -r requirements.txt```

2. Download the chrome selenium driver [here](https://sites.google.com/a/chromium.org/chromedriver/downloads). Extract and place it in the main directory such that the directory looks like this. 

### **Make sure the selenium driver you get is the same version as the chrome browser you are using!!**

```
./selenium/chromedriver.exe
./selenium/chromedriver/
```

3. Download FFMpeg [here](https://github.com/BtbN/FFmpeg-Builds/releases). Copy the contents of the bin folder so that there are 3 files in the main directory.

```
./ffmpeg.exe
./ffplay.exe
./ffprobe.exe
```

## Basic usage

1. Edit  `courses.txt` file with the URLs to all the courses modules you want to download separated by a new line. Its contents should look something like this(+example for Keats):

```
https://[Moodle Website]/course/view.php?id=AAAAA
https://[Moodle Website]/course/view.php?id=BBBBB
https://keats.kcl.ac.uk/course/view.php?id=CCCCC
https://keats.kcl.ac.uk/course/view.php?id=DDDDD
```

2. Execute main.py and it should walk you through the steps.
