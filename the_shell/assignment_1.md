The Assignment Page is in <https://missing.csail.mit.edu/2020/course-shell/>


Answer:

```powershell
hao@DESKTOP-EUJ3G2G MINGW64 /e/blog/Missing_Semester/the_shell
$ mkdir missing

hao@DESKTOP-EUJ3G2G MINGW64 /e/blog/Missing_Semester/the_shell
$ touch --help
Usage: touch [OPTION]... FILE...
Update the access and modification times of each FILE to the current time.
...

hao@DESKTOP-EUJ3G2G MINGW64 /e/blog/Missing_Semester/the_shell
$ cd missing

hao@DESKTOP-EUJ3G2G MINGW64 /e/blog/Missing_Semester/the_shell/missing
$ touch semester

hao@DESKTOP-EUJ3G2G MINGW64 /e/blog/Missing_Semester/the_shell/missing
$ echo '#!/bin/sh' > semester

hao@DESKTOP-EUJ3G2G MINGW64 /e/blog/Missing_Semester/the_shell/missing
$ echo 'curl --head --silent https://missing.csail.mit.edu' >> semester

hao@DESKTOP-EUJ3G2G MINGW64 /e/blog/Missing_Semester/the_shell/missing
$ ls -l semester
-rwxr-xr-x 1 wuhao 197609 61 11月 22 00:07 semester*
#Why? Because the file lacks execute permissions.

# Adding Execution permissions to the file
hao@DESKTOP-EUJ3G2G MINGW64 /e/blog/Missing_Semester/the_shell/missing
$ chmod +x semester

hao@DESKTOP-EUJ3G2G MINGW64 /e/blog/Missing_Semester/the_shell/missing
$ ./semester > last-modified.txt
```
