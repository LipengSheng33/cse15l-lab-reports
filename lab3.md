```
$ find -type d
.
./.git
./.git/hooks
./.git/info
./.git/logs
./.git/logs/refs
./.git/logs/refs/heads
./.git/logs/refs/remotes
./.git/logs/refs/remotes/origin
./.git/logs/refs/remotes/upstream
./.git/objects
./.git/objects/04
./.git/objects/7f
./.git/objects/c4
./.git/objects/info
./.git/objects/pack
./.git/refs
./.git/refs/heads
./.git/refs/remotes
./.git/refs/remotes/origin
./.git/refs/remotes/upstream
./.git/refs/tags
./lib
./technical
./technical/911report
./technical/biomed
./technical/government
./technical/government/About_LSC
./technical/government/Alcohol_Problems
./technical/government/Env_Prot_Agen
./technical/government/Gen_Account_Office
./technical/government/Media
./technical/government/Post_Rate_Comm
./technical/plos
```

The above command is searching for all the directories from ./technical. The find -type command is useful because it can helps us find a specific type of files: The above case only find the directory files.

```
$ find technical/911report -type f
technical/911report/chapter-1.txt
technical/911report/chapter-10.txt
technical/911report/chapter-11.txt
technical/911report/chapter-12.txt
technical/911report/chapter-13.1.txt
technical/911report/chapter-13.2.txt
technical/911report/chapter-13.3.txt
technical/911report/chapter-13.4.txt
technical/911report/chapter-13.5.txt
technical/911report/chapter-2.txt
technical/911report/chapter-3.txt
technical/911report/chapter-5.txt
technical/911report/chapter-6.txt
technical/911report/chapter-7.txt
technical/911report/chapter-8.txt
technical/911report/chapter-9.txt
technical/911report/preface.txt
```

The above command is searching for all the regular files from ./technical/911report. The find -type command is useful because it can helps us find a specific type of files: the above case only find the regular files from ./technical/911report.

```
$ find -size +250k
./.git/objects/pack/pack-ebe3d375863bc7c77f3a085578b78e94ce70f1a0.pack
./lib/junit-4.13.2.jar
./technical/911report/chapter-13.4.txt
./technical/911report/chapter-13.5.txt
./technical/911report/chapter-3.txt
./technical/government/Gen_Account_Office/d01591sp.txt
./technical/government/Gen_Account_Office/Statements_Feb28-1997_volume.txt
```

The above command is searching for all files larger than 250 kilobytes. The find -size command is useful because it can helps us find all the files below or above certain sizes: the above case only find the files larger than 250 kilobytes.

```
$ find -size -1k
.
./.git
./.git/hooks
./.git/info
./.git/logs
./.git/logs/refs
./.git/logs/refs/heads
./.git/logs/refs/remotes
./.git/logs/refs/remotes/origin
./.git/objects
./.git/objects/info
./.git/objects/pack
./.git/refs
./.git/refs/heads
./.git/refs/remotes
./.git/refs/remotes/origin
./.git/refs/tags
./lib
./technical
./technical/911report
./technical/biomed
./technical/government
./technical/government/About_LSC
./technical/government/Alcohol_Problems
./technical/government/Env_Prot_Agen
./technical/government/Gen_Account_Office
./technical/government/Media
./technical/government/Post_Rate_Comm
./technical/plos
```

The above command is searching for all files smaller than 1 kilobytes. The find -size command is useful because it can helps us find all the files below or above certain sizes: the above case only find the files smaller than 1 kilobytes.

```
$ find -maxdepth 0
.
```

The above command is searching for all files within the depth of 0, which means that it is only searching for the starting directory. This is why the out put is only a dot. The find -maxdepth command is useful when we only want to search for files within certain depth.

```
$ find -maxdepth 2
.
./.git
./.git/config
./.git/description
./.git/FETCH_HEAD
./.git/HEAD
./.git/hooks
./.git/index
./.git/info
./.git/logs
./.git/objects
./.git/packed-refs
./.git/refs
./DocSearchServer.java
./lib
./lib/hamcrest-core-1.3.jar
./lib/junit-4.13.2.jar
./README.md
./Server.java
./technical
./technical/911report
./technical/biomed
./technical/government
./technical/plos
./TestDocSearch.java
```

The above command is searching for all files within the depth of 2, which means that it is only searching for the starting directory, the subdirectories of the starting directory and the subdirectories of the subdirectories of the starting directory. The find -maxdepth command is useful when we only want to search for files within certain depth.

```
$ find technical/plos/pmed.0020206.txt -delete

```

The above command is searching for a specific file technical/plos/pmed.0020206.txt and delete it. The find -delete command is useful when we want to find a specific file to delete.

```
$ find technical/government/Gen_Account_Office/Statements_Feb28-1997_volume.txt 
-delete

```

The above command is searching for a specific file technical/government/Gen_Account_Office/Statements_Feb28-1997_volume.txt  and delete it. The find -delete command is useful when we want to find a specific file to delete.
