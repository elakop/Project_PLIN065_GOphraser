# Project_PLIN065
Project for the Tools for theories course at Masaryk University, Brno

This is paraser for XML text files. In this case it is needed to extract "clear" text from Czech corpus csTenTen17.vert.
The paraser reads a structured text file with XML tags (<doc>, <p>, <s> etc.), extracts only the text content (words) from it and produces "clean" text output, where each sentence is on a separate line.

Requirements:
  GO - https://go.dev/dl
  csTenTen.vert file - Data source commit

How to use the code:
  1. Install GO programming language
  2. Initialize Go module in the command line: go mod init nameoftheproject
      -> go.mod will be created with: module nameoftheproject
                                       go 1.24.2
  3. Save the code from GitHub as a main.go
  4. In the terminal line run: go run main.go -i csTenTen17.vert -o output.txt (name your output as you wish)
      ->`-i` = input file (required)
      -> `-o` = output file (required)
      -> `-n` = number of documents to process (optional): go run main.go -i csTenTen17.vert -o test.txt -n 100

The file (nameoftheproject) is going to have:
  go.mod
  main.go
  csTenTen17.vert (the corpus)
  output.txt (generated from the program)
