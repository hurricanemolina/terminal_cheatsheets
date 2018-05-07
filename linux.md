# terminal-linux-cheatsheet
Basic and frequently used Linux commands in a cheatsheet.

## CORE COMMANDS

| Key/Command | Description |
| ----------- | ----------- |
| ssh [remote] | Connect to another host |
| scp [file destination] | Transfer file to another host |
| wget [http file] | Download web files |
| ftp [domain] | Download files |
| rm [file] | Remove a file |
| rm -r [directory] |  Remove a directory |
| mkdir [directory] | Make a directory |
| cp -R [source destination/] | Copy a directory with files
| cd ~ |  Home directory |
| cd /  | Root of drive |
| cd -  | Previous directory |
| ls | Short listing |
| ls -l | Long listing |
| ls -a | Listing incl. hidden files |
| ls -lh| Long listing with Human readable file sizes |
| ls -R | Entire content of folder recursively |
| ls insert_vertical_line wc -l | List number of files in directory |
| top | Displays active processes. Press q to quit |
| du | Disk usage |
| du -h | Disk usage human-readable format |
| du -sh * | List files with human-readable format size |
| ls -lS | List files with sizes, no issue if lots of files |


## VI COMMANDS

| Key/Command | Description |
| ----------- | ----------- |
| vi [filename] | Open file or create file with VI |
| i | Insert text from cursor|
| I | Insert text from top of file |
| :q! | Quit file without saving |
| :wq! | Write and quit with saving, force write|
| :wq | Write and quit with saving, no force write|
| :q | Safer quit, won't quit if changes |
| :x | Write and quit with saving, but won't write if no changes |



