# LINUX COMMAND LINE

## HOW TO

**\$** = Normal user\
**\#** = Super user (root)

> `<command> <options....>` :- Brief description\
> `<shows the output of the command>`

# 

> `date` :- Displays the current date and time in ISO format\
> `Monday 16 February 2026 11:19:57 PM IST`

# 

> `uptime` :- Shows system uptime along with load average\
> `23:21:47 up 2 min, 2 users, load average: 0.23, 0.27, 0.11`

# 

> `df` :- Displays available and used disk space for mounted filesystems
>
>     Filesystem          1K-blocks    Used Available Use% Mounted on
>     /dev/mapper/rl-root   6430720 2852944   3577776  45% /
>     devtmpfs               829324       0    829324   0% /dev
>     tmpfs                  856900       0    856900   0% /dev/shm
>     tmpfs                  342760    6440    336320   2% /run
>     tmpfs                    1024       0      1024   0% /run/>credentials/systemd-journald.service
>     /dev/nvme0n1p2         983040  503160    479880  52% /boot
>     tmpfs                    1024       0      1024   0% /run/>credentials/getty@tty1.service
>     tmpfs                  171380       4    171376   1% /run/user/1000

# 

> `pwd` :- Shows the present working directory\
> `/home/<username>/testing`

# 

> `cd <dir/>` :- Changes the current directory
>
> **Interesting** -- Try `cd -` (previous directory) \| `cd ~` (home
> directory) \| `cd ~<username>`

# 

> `ls` :- Lists directory contents
>
>     bin               docker_practice     testing
>     syntax            docker_status.txt   setup-firewall.sh
>     dockerfile.txt    mypipe
>
> Also
>
> `ls <file|dir>....` :- List multiple `<dirs>` or `<files>`
>
> **Common options**
>
> -   *`-l`* = Long listing format\
> -   *`-i`* = Shows inode numbers (useful for checking links)\
> -   *`-a`* = Shows all files (including hidden)\
> -   *`-d`* = Shows directory itself (best used with *`-ld`*)\
> -   *`-A`* = Shows hidden files except `.` and `..`
>
> **Interesting** -- Try `ll` (if available) for long listing

# 

> `file <file|dir>` :- Determines the file type\
> `mypipe: fifo (named pipe)`

# 

> `less <file_name>` :- Views file content page by page (very useful)
>
> **Common options**
>
> -   *`-f`* = Follow mode (useful for debugging logs)
>
> **Inside `less`**
>
> -   *`/`* = Search forward\
> -   `?` = Search backward\
> -   `f` \| `<space>` = Forward one screen\
> -   `b` = Backward one screen\
> -   *`n`* = Next match\
> -   *`p`* = Previous match\
> -   *`g`* = Go to beginning of file\
> -   *`G`* = Go to end of file\
> -   *`h`* = Show help\
> -   *`q`* = Quit

# 

> `type <command>` :- Shows how a command is interpreted (alias,
> builtin, or executable file)

# 

> `reset` :- Clears and fully resets the terminal

# 

> `cp <source> <destination>` :- Copies files or directories\
> Most used options: `-r` (recursive), `-i` (confirm before overwrite),
> `-v` (verbose)

# 

> `mv <source> <destination>` :- Moves or renames files\
> Most used options: `-i`, `-v`

# 

> `mkdir <dir>` :- Creates a directory\
> Most used options: `-p` (create parent directories if needed)

# 

> `rm <file|dir>` :- Removes files or directories\
> Most used options: `-r` (recursive), `-f` (force), `-i` (confirm
> before delete)

# 

> `ln <target> <link>` :- Creates links between files\
> Most used options: `-s` (create symbolic link)

# 

> `which <command>` :- Displays the path of an executable

# 

> `help <builtin>` :- Displays help for shell built-in commands

# 

> `man <command>` :- Opens the manual page

# 

> `apropos <keyword>` :- Searches manual pages by keyword

# 

> `info <command>` :- Opens detailed GNU documentation

# 

> `whatis <command>` :- Shows a one-line description from the manual

# 

> `alias name='command'` :- Creates a shortcut for a command

# 

> `unalias name` :- Removes an alias

# 

> `cat <file>` :- Displays file contents\
> Most used options: `-n` (number lines)

# 

> `>` :- Redirects output to a file (overwrite)

# 

> `>>` :- Redirects output to a file (append)

# 

> `sort <file>` :- Sorts lines in a file\
> Most used options: `-n` (numeric sort), `-r` (reverse order)

# 

> `uniq <file>` :- Removes duplicate lines (file should be sorted
> first)\
> Most used options: `-c` (count occurrences)

# 

> `grep <pattern> <file>` :- Searches text using a pattern\
> Most used options: `-i` (ignore case), `-r` (recursive), `-n` (show
> line numbers)

# 

> `wc <file>` :- Counts lines, words, and characters\
> Most used options: `-l` (lines), `-w` (words), `-c` (characters)

# 

> `head <file>` :- Shows the first 10 lines of a file\
> Most used options: `-n <number>`

# 

> `tail <file>` :- Shows the last 10 lines of a file\
> Most used options: `-n <number>`, `-f` (follow live updates)

# 

> `tee <file>` :- Sends output to both screen and file\
> Most used options: `-a` (append)

# 

> `|` (pipe) :- Sends the output of one command as input to another

# 

> `echo <text>` :- Prints text to the terminal\
> Most used options: `-e` (enable escape characters)
