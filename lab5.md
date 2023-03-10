# Lab Report 5

All of the commands below were found on this [website](https://phoenixnap.com/kb/less-command-in-linux).

## find -name
The command find -name will search for a file with a specific name, which is useful because it can find a file within the given directory matching with the name given in the command line. This was found on this [website](https://www.geeksforgeeks.org/find-command-in-linux-with-examples/).
```
# Example One: Input
find written_2/ -name ch1.txt

```
```
# Example One: Output 
written_2//non-fiction/OUP/Berk/ch1.txt
written_2//non-fiction/OUP/Abernathy/ch1.txt
written_2//non-fiction/OUP/Rybczynski/ch1.txt
written_2//non-fiction/OUP/Kauffman/ch1.txt
written_2//non-fiction/OUP/Fletcher/ch1.txt
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
The command find -iname will search for a file by an approximate name. This is useful because you can search for a file using a partial and case-insensitive search. This command was found at this [website](https://www.redhat.com/sysadmin/linux-find-command)
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
The command grep -i ignores case sensitivity, thus this command is useful because it will search for a string regardless of the capitalization. 
```
# Example One: Input
find written_2/non-fiction/OUP/Berk/ -type f
```
```
# Example One: Output
written_2/non-fiction/OUP/Berk//ch2.txt
written_2/non-fiction/OUP/Berk//ch1.txt
written_2/non-fiction/OUP/Berk//CH4.txt
written_2/non-fiction/OUP/Berk//ch7.txt
```
```
# Example Two: Input
find written_2/non-fiction/OUP/Rybczynski/ -type f        
```
```
# Example Two: Output
written_2/non-fiction/OUP/Rybczynski//ch2.txt
written_2/non-fiction/OUP/Rybczynski//ch3.txt
written_2/non-fiction/OUP/Rybczynski//ch1.txt
```

## grep -n
The command grep -n shows the number of the lines where the string is matched. This is useful because you can locate the specific line of where the string occurs within the file. 
```
# Example One: Input
grep -n "Boston Common" written_2/*/*/*.txt
```
```
# Example One: Output
written_2/travel_guides/berlitz2/Boston-WhereToGo.txt:7:Boston Common, Beacon Hill,and The Esplanade
written_2/travel_guides/berlitz2/Boston-WhereToGo.txt:8:Boston Common
written_2/travel_guides/berlitz2/Boston-WhereToGo.txt:84:In the middle of the 19th-century, Boston ended at Boston Common and Back Bay was just a polluted tidal flat. In 30 years, however, an immense landfill project transformed it into the city’s most fashionable residential and commercial district to which the well-to-do moved from Beacon Hill and the South End.
written_2/travel_guides/berlitz2/Boston-WhereToGo.txt:113:Franklin Park lies close by to the west. The Zoo (open winter Monday–Friday, 10am–4 pm; 10–5pm, Saturday, Sunday, and holidays; 10am–5pm and 10am–6pm respectively in winter), a 75-acre (30-hectare) area with 150 different species, is part of the park. The showpieces are the new lion exhibit, snow leopard and cheetah exhibits, and an African tropical rain forest, which is complete with gorillas and warthogs. Franklin Park was the jewel in the Emerald Necklace, the last in a 7-mile (11-km) network of parks designed by Frederick Law Olmsted that run all the way from Boston Common.
```
```
# Example Two: Input
grep -n "Antilles chain" written_2/*/*/*.txt
```
```
# Example Two: Output
written_2/travel_guides/berlitz1/HistoryFWI.txt:15:        America began migrating up the Antilles chain, reaching Martinique and
written_2/travel_guides/berlitz1/WhereToFWI.txt:13:        Lesser Antilles chain. Its major neighbors are volcano-devastated
written_2/travel_guides/berlitz1/WhereToFWI.txt:736:        along the confusing Antilles chain, some experts suggest that he
```

