# shell-data-processing

## To return a page text and output it to a file:
* The curl command which I used used to get data from the URL and store in a data.txt file is ```curl "http://shakespeare.mit.edu/cymbeline/cymbeline.1.1.html" -O "data.txt"```

## To process text data
*  The command used to transform each space '' into a return charater is ``` tr ' ' '\12' < data.txt``` 
*  The command used to sort the text in data file is ```tr ' ' '\12' < data.txt | sort ```
*  The command used to pipe the sorted output to count is  ```tr ' ' '\12' < data.txt | sort | uniq -c```
*  The command used to pipe the resulted output to sort with -nr flag is  ```tr ' ' '\12' < data.txt | sort | uniq -c | sort -nr```.
*  The command used to store the final output to result.txt file ```tr ' ' '\12' < data.txt | sort | uniq -c | sort -nr > result.txt``` 

## Bash 
* When up arrow is hit, bash shell will cycle through the history of commands used.
* -n flag means compare according to string numerical value
* -r flag means reverse the result of comparisions.
* a flag with a single letter is preceded by only single dash where as if the flag is more than one letter, it is preceded by two dashes. 
