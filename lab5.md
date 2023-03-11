# Lab Report 5


## find -name
The command find -name will search for a file with a specific name, which is useful because it can find a file within the given directory matching with the name given in the command line. This was found on this [website](https://www.geeksforgeeks.org/find-command-in-linux-with-examples/).
```
# Example One: Input
find written_2 -name ch1.txt

```
```
# Example One: Output 
written_2/non-fiction/OUP/Berk/ch1.txt
written_2/non-fiction/OUP/Abernathy/ch1.txt
written_2/non-fiction/OUP/Rybczynski/ch1.txt
written_2/non-fiction/OUP/Kauffman/ch1.txt
written_2/non-fiction/OUP/Fletcher/ch1.txt
```
```
# Example Two: Input
find written_2 -name HistoryIndia.txt

```
```
# Example Two: Output
written_2/travel_guides/berlitz1/HistoryIndia.txt
```


## find -iname
The command find -iname will search for a file by an approximate name. This is useful because you can search for a file using a partial and case-insensitive search. This command was found at this [website](https://www.redhat.com/sysadmin/linux-find-command).
```
# Example One: Input
find written_2 -iname "*ch8*txt"
```
```
# Example One: Output
written_2/non-fiction/OUP/Abernathy/ch8.txt
written_2/non-fiction/OUP/Kauffman/ch8.txt
```
```
# Example Two: Input
find written_2 -iname "*POLAND*txt"
```
```
# Example Two: Output
written_2/travel_guides/berlitz2/Poland-WhatToDo.txt
written_2/travel_guides/berlitz2/Poland-History.txt
```

## find -type f
The command find -type f will search for files within the specified directory. Thus, this is useful because you can search for a file without specifing the name within a directory. This command was found at this [website](https://www.redhat.com/sysadmin/linux-find-command).
```
# Example One: Input
find written_2/non-fiction/OUP/Berk -type f
```
```
# Example One: Output
written_2/non-fiction/OUP/Berk/ch2.txt
written_2/non-fiction/OUP/Berk/ch1.txt
written_2/non-fiction/OUP/Berk/CH4.txt
written_2/non-fiction/OUP/Berk/ch7.txt
```
```
# Example Two: Input
find written_2/non-fiction/OUP/Rybczynski/ -type f        
```
```
# Example Two: Output
written_2/non-fiction/OUP/Rybczynski/ch2.txt
written_2/non-fiction/OUP/Rybczynski/ch3.txt
written_2/non-fiction/OUP/Rybczynski/ch1.txt
```

## find type -d
The command grep -d lists the directories in the given path. Therefore, this is useful because it will display only the directories and not the files within them. This command was found at this [website](https://www.redhat.com/sysadmin/linux-find-command).
```
# Example One: Input
find written_2 -type d
```
```
# Example One: Output
written_2
written_2/non-fiction
written_2/non-fiction/OUP
written_2/non-fiction/OUP/Berk
written_2/non-fiction/OUP/Abernathy
written_2/non-fiction/OUP/Rybczynski
written_2/non-fiction/OUP/Kauffman
written_2/non-fiction/OUP/Fletcher
written_2/non-fiction/OUP/Castro
written_2/travel_guides
written_2/travel_guides/berlitz1
written_2/travel_guides/berlitz2
```
```
# Example Two: Input
find written_2/travel_guides -type d
```
```
# Example Two: Output
written_2/travel_guides
written_2/travel_guides/berlitz1
written_2/travel_guides/berlitz2
```

