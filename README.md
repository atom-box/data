## What's going on here
This is test data.  It was scraped or downloaded and then broken up into a list of words or a CSV.  For convenience, some tools are below:
1. Shell
<br>Replace punctuation with newline
<br>sed 's/\([.,:;!?]\)/\1|/g' $1  | tr "|" "\1\n" 

2. Shell
<br>Grab just the first column from CSV
<br>sed 's_\([A-z]\{1,11\}\).*_\1_' thousandNouns.csv | sort | uniq

3. Third party tool
<br>There's a word counter/ranker function at this WordCloud generator.   Don't use it for any private data!! <br>https://www.wordclouds.com/ 
