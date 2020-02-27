# SongOrganizer

I have several folders filled with unorganized songs, each one named title.mp3. SongOrganizer is a script I created to organize this madness, placing each one in a specific folder, depending the artist's name. 

## Version 1.5

Having tried it in one of my folders, I noticed another flaw. The script used id3info command, which requires the song to be an .mp3 file. Upon reaching a .flac one, an error occured. I had to implement another conditional structure to check whether we are dealing with either of those types of files, and continue accordingly. 

Besides, a minor change was implemented: now we are displayed on-screen a message saying each file is being moved from $1 (origin) to $2 (destination), and a completion message afterwards.


## Version v1.0 

After testing v0.0, I realised it was too flawed. This version correctly fixes the issues of the previous version, and introduces the possibility (in fact the requirement) of specifying the origin and destination of the files as first and second arguments of the script, respectively.


## Version v0.0

This is the original script. It hasn't been tested yet.

