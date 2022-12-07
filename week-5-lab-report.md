```
[cs15lfa22mh@ieng6-203]:docsearch:29$ grep  "journal" find-results.txt
technical/plos/journal.pbio.0020001.txt
technical/plos/journal.pbio.0020010.txt
technical/plos/journal.pbio.0020012.txt
technical/plos/journal.pbio.0020013.txt
technical/plos/journal.pbio.0020019.txt
technical/plos/journal.pbio.0020028.txt
technical/plos/journal.pbio.0020035.txt
technical/plos/journal.pbio.0020040.txt
technical/plos/journal.pbio.0020042.txt
technical/plos/journal.pbio.0020043.txt
technical/plos/journal.pbio.0020046.txt
technical/plos/journal.pbio.0020047.txt
technical/plos/journal.pbio.0020052.txt
technical/plos/journal.pbio.0020053.txt
technical/plos/journal.pbio.0020054.txt
technical/plos/journal.pbio.0020063.txt
technical/plos/journal.pbio.0020064.txt
technical/plos/journal.pbio.0020067.txt
technical/plos/journal.pbio.0020068.txt
technical/plos/journal.pbio.0020071.txt
technical/plos/journal.pbio.0020073.txt
technical/plos/journal.pbio.0020100.txt
technical/plos/journal.pbio.0020101.txt
technical/plos/journal.pbio.0020105.txt
technical/plos/journal.pbio.0020112.txt
technical/plos/journal.pbio.0020113.txt
technical/plos/journal.pbio.0020116.txt
technical/plos/journal.pbio.0020121.txt
technical/plos/journal.pbio.0020125.txt
technical/plos/journal.pbio.0020127.txt
technical/plos/journal.pbio.0020133.txt
technical/plos/journal.pbio.0020140.txt
technical/plos/journal.pbio.0020145.txt
technical/plos/journal.pbio.0020146.txt
technical/plos/journal.pbio.0020147.txt
technical/plos/journal.pbio.0020148.txt
technical/plos/journal.pbio.0020150.txt
technical/plos/journal.pbio.0020156.txt
technical/plos/journal.pbio.0020161.txt
technical/plos/journal.pbio.0020164.txt
technical/plos/journal.pbio.0020169.txt
technical/plos/journal.pbio.0020172.txt
technical/plos/journal.pbio.0020183.txt
technical/plos/journal.pbio.0020187.txt
technical/plos/journal.pbio.0020190.txt
technical/plos/journal.pbio.0020206.txt
technical/plos/journal.pbio.0020213.txt
technical/plos/journal.pbio.0020214.txt
technical/plos/journal.pbio.0020215.txt
technical/plos/journal.pbio.0020216.txt
technical/plos/journal.pbio.0020223.txt
technical/plos/journal.pbio.0020224.txt
technical/plos/journal.pbio.0020228.txt
technical/plos/journal.pbio.0020232.txt
technical/plos/journal.pbio.0020241.txt
technical/plos/journal.pbio.0020262.txt
technical/plos/journal.pbio.0020263.txt
technical/plos/journal.pbio.0020267.txt
technical/plos/journal.pbio.0020272.txt
technical/plos/journal.pbio.0020276.txt
technical/plos/journal.pbio.0020297.txt
technical/plos/journal.pbio.0020302.txt
technical/plos/journal.pbio.0020306.txt
technical/plos/journal.pbio.0020307.txt
technical/plos/journal.pbio.0020310.txt
technical/plos/journal.pbio.0020311.txt
technical/plos/journal.pbio.0020337.txt
technical/plos/journal.pbio.0020346.txt
technical/plos/journal.pbio.0020347.txt
technical/plos/journal.pbio.0020348.txt
technical/plos/journal.pbio.0020350.txt
technical/plos/journal.pbio.0020353.txt
technical/plos/journal.pbio.0020354.txt
technical/plos/journal.pbio.0020394.txt
technical/plos/journal.pbio.0020400.txt
technical/plos/journal.pbio.0020401.txt
technical/plos/journal.pbio.0020404.txt
technical/plos/journal.pbio.0020406.txt
technical/plos/journal.pbio.0020419.txt
technical/plos/journal.pbio.0020420.txt
technical/plos/journal.pbio.0020430.txt
technical/plos/journal.pbio.0020431.txt
technical/plos/journal.pbio.0020439.txt
technical/plos/journal.pbio.0020440.txt
technical/plos/journal.pbio.0030021.txt
technical/plos/journal.pbio.0030024.txt
technical/plos/journal.pbio.0030032.txt
technical/plos/journal.pbio.0030050.txt
technical/plos/journal.pbio.0030051.txt
technical/plos/journal.pbio.0030056.txt
technical/plos/journal.pbio.0030062.txt
technical/plos/journal.pbio.0030065.txt
technical/plos/journal.pbio.0030076.txt
technical/plos/journal.pbio.0030094.txt
technical/plos/journal.pbio.0030097.txt
technical/plos/journal.pbio.0030102.txt
technical/plos/journal.pbio.0030105.txt
technical/plos/journal.pbio.0030127.txt
technical/plos/journal.pbio.0030129.txt
technical/plos/journal.pbio.0030131.txt
technical/plos/journal.pbio.0030136.txt
technical/plos/journal.pbio.0030137.txt
```
Here is our initial run of the grep command, listing out all the files that contain "journal," in this case finding the path
```
[cs15lfa22mh@ieng6-203]:docsearch:30$ grep -c  "journal" find-results.txt
102
```
-c allows us to count how many files were just listed, in this case 102 files had "journal" in the path.
```
[cs15lfa22mh@ieng6-203]:docsearch:32$ grep -i  "JOURNAL" find-results.txt
technical/plos/journal.pbio.0020001.txt
technical/plos/journal.pbio.0020010.txt
technical/plos/journal.pbio.0020012.txt
technical/plos/journal.pbio.0020013.txt
technical/plos/journal.pbio.0020019.txt
technical/plos/journal.pbio.0020028.txt
technical/plos/journal.pbio.0020035.txt
technical/plos/journal.pbio.0020040.txt
technical/plos/journal.pbio.0020042.txt
technical/plos/journal.pbio.0020043.txt
technical/plos/journal.pbio.0020046.txt
technical/plos/journal.pbio.0020047.txt
technical/plos/journal.pbio.0020052.txt
technical/plos/journal.pbio.0020053.txt
technical/plos/journal.pbio.0020054.txt
technical/plos/journal.pbio.0020063.txt
technical/plos/journal.pbio.0020064.txt
technical/plos/journal.pbio.0020067.txt
technical/plos/journal.pbio.0020068.txt
technical/plos/journal.pbio.0020071.txt
technical/plos/journal.pbio.0020073.txt
technical/plos/journal.pbio.0020100.txt
technical/plos/journal.pbio.0020101.txt
technical/plos/journal.pbio.0020105.txt
technical/plos/journal.pbio.0020112.txt
technical/plos/journal.pbio.0020113.txt
technical/plos/journal.pbio.0020116.txt
technical/plos/journal.pbio.0020121.txt
technical/plos/journal.pbio.0020125.txt
technical/plos/journal.pbio.0020127.txt
technical/plos/journal.pbio.0020133.txt
technical/plos/journal.pbio.0020140.txt
technical/plos/journal.pbio.0020145.txt
technical/plos/journal.pbio.0020146.txt
technical/plos/journal.pbio.0020147.txt
technical/plos/journal.pbio.0020148.txt
technical/plos/journal.pbio.0020150.txt
technical/plos/journal.pbio.0020156.txt
technical/plos/journal.pbio.0020161.txt
technical/plos/journal.pbio.0020164.txt
technical/plos/journal.pbio.0020169.txt
technical/plos/journal.pbio.0020172.txt
technical/plos/journal.pbio.0020183.txt
technical/plos/journal.pbio.0020187.txt
technical/plos/journal.pbio.0020190.txt
technical/plos/journal.pbio.0020206.txt
technical/plos/journal.pbio.0020213.txt
technical/plos/journal.pbio.0020214.txt
technical/plos/journal.pbio.0020215.txt
technical/plos/journal.pbio.0020216.txt
technical/plos/journal.pbio.0020223.txt
technical/plos/journal.pbio.0020224.txt
technical/plos/journal.pbio.0020228.txt
technical/plos/journal.pbio.0020232.txt
technical/plos/journal.pbio.0020241.txt
technical/plos/journal.pbio.0020262.txt
technical/plos/journal.pbio.0020263.txt
technical/plos/journal.pbio.0020267.txt
technical/plos/journal.pbio.0020272.txt
technical/plos/journal.pbio.0020276.txt
technical/plos/journal.pbio.0020297.txt
technical/plos/journal.pbio.0020302.txt
technical/plos/journal.pbio.0020306.txt
technical/plos/journal.pbio.0020307.txt
technical/plos/journal.pbio.0020310.txt
technical/plos/journal.pbio.0020311.txt
technical/plos/journal.pbio.0020337.txt
technical/plos/journal.pbio.0020346.txt
technical/plos/journal.pbio.0020347.txt
technical/plos/journal.pbio.0020348.txt
technical/plos/journal.pbio.0020350.txt
technical/plos/journal.pbio.0020353.txt
technical/plos/journal.pbio.0020354.txt
technical/plos/journal.pbio.0020394.txt
technical/plos/journal.pbio.0020400.txt
technical/plos/journal.pbio.0020401.txt
technical/plos/journal.pbio.0020404.txt
technical/plos/journal.pbio.0020406.txt
technical/plos/journal.pbio.0020419.txt
technical/plos/journal.pbio.0020420.txt
technical/plos/journal.pbio.0020430.txt
technical/plos/journal.pbio.0020431.txt
technical/plos/journal.pbio.0020439.txt
technical/plos/journal.pbio.0020440.txt
technical/plos/journal.pbio.0030021.txt
technical/plos/journal.pbio.0030024.txt
technical/plos/journal.pbio.0030032.txt
technical/plos/journal.pbio.0030050.txt
technical/plos/journal.pbio.0030051.txt
technical/plos/journal.pbio.0030056.txt
technical/plos/journal.pbio.0030062.txt
technical/plos/journal.pbio.0030065.txt
technical/plos/journal.pbio.0030076.txt
technical/plos/journal.pbio.0030094.txt
technical/plos/journal.pbio.0030097.txt
technical/plos/journal.pbio.0030102.txt
technical/plos/journal.pbio.0030105.txt
technical/plos/journal.pbio.0030127.txt
technical/plos/journal.pbio.0030129.txt
technical/plos/journal.pbio.0030131.txt
technical/plos/journal.pbio.0030136.txt
technical/plos/journal.pbio.0030137.txt
```
-i shows us the a case insensitive version of our search, helping allow for any mistakes in capitalization and still yielding results with the word "journal" in any form.
```
[cs15lfa22mh@ieng6-203]:docsearch:33$ grep -vc  "JOURNAL" find-results.txt
1402
```
-v shows us the inverse of our search, filtering out the word "JOURNAL" instead. Since, none of the words contain the case insensitive version, "JOURNAL," it shows the count of all files.
```
[cs15lfa22mh@ieng6-203]:docsearch:35$ grep -c ".txt" find-results.txt
1391
```
Once again, -c is used here to show the count of how many txt files there are.
```
[cs15lfa22mh@ieng6-203]:docsearch:36$ grep -vc ".txt" find-results.txt
11
```
-v is used to show how many non ".txt" files there are.
```
[cs15lfa22mh@ieng6-203]:docsearch:37$ grep -ivc ".Txt" find-results.txt
11
```
Combining all 3 of the commands allows us to perform similarly to the last command but also accounting for errors in capitalization, in this case the first "T" being capitalized in ".txt"
```
[cs15lfa22mh@ieng6-203]:docsearch:40$ grep -c "plos" find-results.txt
253
```
This -c lets us count how many files have the plos path.
```
[cs15lfa22mh@ieng6-203]:docsearch:41$ grep -vc "plos" find-results.txt
1149
```
Combining -c with -v allows us to count the number of files that are in paths not containing /plos
```
[cs15lfa22mh@ieng6-203]:docsearch:42$ grep -ivc "pLoS" find-results.txt
1149
```
Lastly, adding the -i to the command allows us to account for any case sensitivity.