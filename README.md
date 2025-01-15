# Java-Course-Program-2
This program dealt with input parameters and using a string tokenizer to break up words in an input file

# Topics
  BufferedReader Objects, PrintWriter Objects, File methods, String token methods, String functions, character functions, file validation, array methods

# Program Function
## File validation
  Receive an input file and an output file and validate the file. An input file is valid if the file exists in the current directory. An output file is valid if the file does not exist in the current directory. An existing output file can be backed up and overwritten if the user desires. Continue to validate until both files are valid or no file name is entered, in which case the program will quit.

## Traversing files with String Tokenizer
Once validated, the program is to open the input file for reading. The program will read each line of the file, tokenize that line, and then adjust the token so that
  1. The token is a word - meaning it begins with a letter and contains hyphens, digits, or numbers
  2. The token is a number - a sequence of digits

Once finished, all numbers are added to a total sum, and words are kept in a separate array

The output file should contain
  1. the list of words in the order they were encountered
  2. the total number of unique words
  3. the sum of the numbers

# Implementation
## IOFile class
To validate files, the IOFile class was created. This class contains functions that 
  1. check if a file name exists or does not exist
  2. backup a file
  3. return a file extension
  4. return the file name
  5. return a file path
  6. Open a BufferedReader object (used in main method)
  7. Open a PrintWriter object (used in main method)
  8. Set a file name
  9. Prompt user for names for both input and output files
  10. Gets file names entered by the user in the command prompt

## Word class
  To deal with the tokens read in from the file, the word class was created. This class contained functions that
  1. returned the number of words
  2. returned the string of the word
  3. checked if the current instance of a word was equal to a word passed in (both case-sensitive and not case sensitive)
  4. Incremented count by 1
  5. Printed the word and count to the output file
  6. Looked for a specific word in the array

