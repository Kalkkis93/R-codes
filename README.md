# Data-analysis-with-C++

A little data analysis project with C++.

Functions:
  readAndCleanFile: reads file and pics up all the decimal numbers
  kmeans: completes k means algorithm to some vector
  knn: completes k nearest neighbors algorithms to some vector
  printData: prints the data
  sort: sorts the vector

File input.txt includes the following lines:
  3.0 6 --7 8 8.x 2 9 4 8 1 0_ 9 7 0 5
  x0 2 z 6 0z 0.789 4 2 8.7 9 9,0

Now the relevant decimal numbers in the first line are
  3.0 6 7 8 2 9 4 8 1 9 7 0 5
and the relevant decimal numbers in the second line are
  2 6 0.789 4 2 8.7 9

The code in main.cpp reads the file, picks up those numbers, completes k means algorithm to the first line with k = 3 and then completes k nearest neighbors algorithm to the second line using the first line as a training set.

Here's what it prints on the command line:

$ g++ main.cpp data_analysis.cpp; ./a.out
Data x:
- Number of values: 12
- Class 0: [ 0 1 2 3 ] (Size: 4)
- Class 1: [ 4 5 6 7 ] (Size: 4)
- Class 2: [ 8 8 9 9 ] (Size: 4)

Data y:
- Number of values: 7
- Class 0: [ 0.789 2 2 ] (Size: 3)
- Class 1: [ 4 6 ] (Size: 2)
- Class 2: [ 8.7 9 ] (Size: 2)
