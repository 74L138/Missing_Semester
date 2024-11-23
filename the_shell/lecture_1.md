# The Shell
Wu Hao
2024/11/23

## echo

`echo string`: String/Variable output

``` powershell
hao@DESKTOP-EUJ3G2G MINGW64 /e/blog
$ echo "hello"
hello

hao@DESKTOP-EUJ3G2G MINGW64 /e/blog
$ echo it is a test
it is a test
```

## cd and pwd

`pwd`: display the current directory<br> `cd .`: to the current
directory<br> `cd ..`: to its parent directory<br> `cd dir_name`: to
dir_name directory<br> `cd ~`: to the home<br> `cd -`: to the last
visited directory

``` powershell
hao@DESKTOP-EUJ3G2G MINGW64 /e/blog
$ pwd
/e/blog

hao@DESKTOP-EUJ3G2G MINGW64 /
$ cd /e/blog
hao@DESKTOP-EUJ3G2G MINGW64 /e/blog

hao@DESKTOP-EUJ3G2G MINGW64 /e/blog
$ cd -
hao@DESKTOP-EUJ3G2G MINGW64 /

hao@DESKTOP-EUJ3G2G MINGW64 /
$ cd ~
hao@DESKTOP-EUJ3G2G MINGW64 ~
```

## ls

`ls`: display all the content in the current directory `ls -l`: display
the details of content

``` powershell
hao@DESKTOP-EUJ3G2G MINGW64 /e/blog
$ ls -l
total 4
drwxr-xr-x 1 hao 197609 0 11月 20 23:26 _site/
drwxr-xr-x 1 hao 197609 0 11月 21 16:54 Missing_Semester/
drwxr-xr-x 1 hao 197609 0 11月 14 21:31 posts/
drwxr-xr-x 1 hao 197609 0 11月 21 16:49 WEEK_REPORT/
```

1.  d refers to a directory
2.  rwx: read, write, execute
3.  rwx refers to the owner of the file’s permissions
4.  r-x refers to the group of the file’s permissions
5.  r-x refers to anyone else’s permissions

## rmdir and mkdir

`rmdir dir_name` : Delete empty dirs<br> `mkdir dir_name`: Building a
new directory

``` powershell
hao@DESKTOP-EUJ3G2G MINGW64 /e/blog
$ mkdir 1
hao@DESKTOP-EUJ3G2G MINGW64 /e/blog
$ ls
_site/  1/  Missing_Semester/  posts/  WEEK_REPORT/
hao@DESKTOP-EUJ3G2G MINGW64 /e/blog
$ rmdir 1
hao@DESKTOP-EUJ3G2G MINGW64 /e/blog
$ ls
_site/  Missing_Semester/  posts/  WEEK_REPORT/
```

## cat

`cat file_name`and`cat file1 file2`: Displaying file contents<br>
`cat file1 file2 > combined_file`: Redirecting files contents to other
file<br> `cat > newfile`: Reading and saving content from the
terminal<br> `cat >> existing_file`: Appending content to an existing
file<br>

``` powershell
hao@DESKTOP-EUJ3G2G MINGW64 /e/blog
$ cat > main1.py
print("hello")
hao@DESKTOP-EUJ3G2G MINGW64 /e/blog
$ cat > main2.py
print("hao")
hao@DESKTOP-EUJ3G2G MINGW64 /e/blog
$ cat main1.py main2.py
print("hello")
print("hao")
hao@DESKTOP-EUJ3G2G MINGW64 /e/blog
$ cat main1.py main2.py > main.py
hao@DESKTOP-EUJ3G2G MINGW64 /e/blog
$ python main.py
hello
hao
```

## pipe character

`|`: Using the output of one command as input to another command<br>
(Waiting for construction…)

## touch

`touch file_name`: Update the access and modification times of each FILE
to the current time.