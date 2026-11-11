# Java

## I/O
- input from file: `import java.io.File` `import java.util.Scanner`
```
  String inputFileName = "~.txt";
  File inputFile = new File(inputFileName); // legal to contruct a non-existent file
  Scanner in = new Scanner(inputFile);
```
or

` Scanner in = new Scanner(new File(inputFileName));`

- output to file: `import java.io.PrinterWriter`
```
  String outputFileName = "~.txt";
  PrintWriter out = new PrintWriter(outputFileName);
```
- close File (necessary)
  `in.close()` `out.close()`

## Command Line Arguments
- read from terminal: `String[] args`
- prompt - encrypts inputFile to outputFile: `java ProgramName input.txt output.txt`
- prompt - decrypt inputFile to outputFile: `java ProgramName -d input.txt output.txt`

## Exception
- `FileNotFoundException e`
- `NoSuchElementException e`: invalid datatype
- `IOException e`


## Reading
- read characters seperate by smth
  
  `in.useDelimiter("")`

- read words (stop at space)
  `String word = in.next();`

- read lines (stop at \n without \n) => \n would have a buffer

  `String line = in.nextLine();`

- read from string
  `Scanner lineScanner = new Scanner(line);`

## Coverter
- String to Int
  `int numInt = Integer.parseInt(numString);`
- String to Double
  `double numDouble = Double.parseDouble(numString);`

## Classify Character
- Character.isDigit()
- Character.isLetter()
- Character.isUpperCase()
- Character.isLowerCase()
- Character.isWhitespace()
