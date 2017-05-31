# MFCRecorder

This is script to automate the recording of public webcam shows from myfreecams. 


## Requirements

I have only tested this on debian(7+8) and Mac OS X (10.10.4), but it should run on other OSs

Requires python3.5 or newer. You can grab python3.5.2 from https://www.python.org/downloads/release/python-352/
and mfcauto.py (https://github.com/ZombieAlex/mfcauto.py)

to install required modules, run:
```
python3.5 -m pip install livesteramer
python3.5 -m pip install --upgrade git+https://github.com/ZombieAlex/mfcauto.py@master
```

## Setup

edit lines 6 and 8 to set the path for the directory to save the videos to, and to set the location of the "wanted.txt" file.

Add models UID (user ID) to the "wanted.txt" file (only one model per line). This uses the UID instead of the name becaue the models can change their name at anytime, but their UID always stays the same. There is a number of ways to get the models UID, but the easiest would probably be to get it from the URL for their profile image. The profile image URL is formatted as (or similar to):
```
https://img.mfcimg.com/photos2/###/{uid}/avatar.90x90.jpg
```
"{uid}" is the models UID which is the number you will want to add to the "wanted.txt" file. the "###" is the first 3 digits of the models UID. For example, if the models UID is "123456789" the URL for their profile picture will be:
```
https://img.mfcimg.com/photos2/123/123456789/avatar.90x90.jpg
```

I plan to add easier methods to add the models UID, but for now, this will do the job. 
