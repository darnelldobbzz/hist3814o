This was my second attempt at REGEX, my first attempt was a no go as I didn't delete every I should I have so there was still unnecessary data remaining along with the index. 

    1  curl http://archive.org/stream/diplomaticcorre33statgoog/diplomaticcorre33statgoog_djvu.txt > texas.txt
    2  nano texas.txt
    3  grep '\bto\b' texas.txt
    4  sed -r -i.bak 's/(.+\bto\b.+)/~\1/g' texas.txt
    5  ls
    6  nano texas.txt
    7  grep '~' texas.txt > index.txt
    8  ls
    9  nano index.txt
   10  sed -r -i.bak 's/(,)( [0-9]{4})(.+)/\2/g' index.txt
   11  nano index.txt
   12  sed -r -i.bak 's/~//g' index.txt
   13  nano index.txt
   14  sed -r -i.bak 's/(\b to \b)/,/g' index.txt
   15  nano index.txt
   16  cp index.txt cleaned-correspondence.csv
   17  ls
   18  dhbox work-today.md
   19  dhbox-work-today.md
   20  history
   21  history > dhbox-work-today.md
