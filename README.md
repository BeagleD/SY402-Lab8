# SY402-Lab8 - this is an example of a read me file for the Lab. This program creates a hash.py script that will recursively walk through all files on a webserver file system. 
Hint: In-built libraries and functions, such as os.listdir, os.stat, and os.walk can be quite helpful. You will want to define certain files and/or directories as unhashable so that they will be ignored, /dev is a perfect example, as you do not want to hash this directory. Note: Below is a non-exhaustive list of directories you will probably want to ignore (if your program gets stuck on a directory you will want to consider ignore those as well):
/dev
/proc
/run
/sys
/tmp
/var/lib
/var/run
A Part 1 solution will be able to walk through the entire file system, printing out the filenames (with their paths), and taking no action other than skipping the unhashable files or directories.

Hint: In-built libraries and functions, such as os.listdir, os.stat, and os.walk can be quite helpful.
Integrate SHA2 (SHA256) so that each file is hashed as it moves through the file system. You are not expected to write SHA2 from scratch, use a python library such as hashlib.
Store the file and hash information so that it will be available for future runs. At a minimum store the following data:
filename with full path
hash
date/time file was observed
The final step, your program should run and update the hash information, upon completion it should print out summary information that includes all new files found, any missing files, and any file that was modified.
Extra Credit Detect that a file was moved, add to your summary section an output that documents where the file is now, and where it was, and the time of the last scan that saw it in the older location.
