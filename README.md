# sed (Stream EDitor, a Unix utility) notes and recipes

***Sed editor***  

\*\*\* **Just append text to file**  

`sed -i '$a append_text' filename.txt  `
- *$ and a - must have options!!!*
- *$ - This address matches the last line of the last file of input, or the last line of each file when the -i or -s options are specified. (end of line)*
- *a - insert the text after matched pattern*

\*\*\* **Delete line**  

`sed -i '/search_text/c\' filename.txt  `
- *c - delete line*
 
 
*** **Find template and add new line after line with template**  

`sed -i '/search_text/a \\' filename.txt `
 
- *string - string to be found*
- *-i - edit file in place*
- *a - insert the text after matched pattern*
- *\\ or \n - newline*
 
 
*** **Find and replace text** 
 
`sed -i 's/found_text/replace_text/' filename.txt `


*** **Some more options** 
- *\t - tab character*
- *^ - Matches the null string at beginning of the pattern space, i.e., what appears after the ^ must appear at the beginning of the pattern space*
- - *$ - This address matches the last line of the last file of input, or the last line of each file when the -i or -s options are specified. (end of line)*
