# SongOrganizer

### Author: Gonzalo Contreras Aso.
---

I have several folders filled with unorganized songs, each one named title.mp3. SongOrganizer is a script I created to organize this madness, placing each one in a specific folder, depending the artist's name. 

A secondary, though also important purpose, is tinkering with Git and GitHub. At least putting into practice the basics, as this project is not as complicated as to needing branching and merging.

An important detail of the script is that it does not move files, it just copies them, so as to not compromise their integrity if there was any issue in the processs. It is therefore up to the user to delete the files from the original location afterwards.

## Version 2.0

A LICENSE file has been added. It is the standard GPLv3, which I feel is the best one for this project.

Man pages have also been added to the project (SongOrganizer.1 file). As of now, they need to be installed by hand, for which it is recommended executing (while located within the project's directory)
```bash
$ install -g 0 -o 0 -m 0644 SongOrganizer.1 /usr/local/man/man1/
$ gzip /usr/local/man/man1/SongOrganizer.1 
```

The code has also been slightly modified, with the differentiation between types of files being rewritten as a function and adding some minor aesthetical details (colors).

## Version 1.5

Having tried it in one of my folders, I noticed another flaw. The script used id3info command, which requires the song to be an .mp3 file. Upon reaching a .flac one, an error occured. I had to implement another conditional structure to check whether we are dealing with either of those types of files, and continue accordingly. 

Besides, a minor change was implemented: now we are displayed on-screen a message saying each file is being moved from $1 (origin) to $2 (destination), and a completion message afterwards.


## Version v1.0 

After testing v0.0, I realised it was too flawed. This version correctly fixes the issues of the previous version, and introduces the possibility (in fact the requirement) of specifying the origin and destination of the files as first and second arguments of the script, respectively.


## Version v0.0

This is the original script. It hasn't been tested yet.

## Version Beta 
Marshmallon the fuking amo asepteme el commit
