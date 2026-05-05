# Matrix Neighbor Finder

Simple Java console application that works with a 2D matrix.
The program allows the user to input matrix values, search for a specific number, and display its position along with its neighboring elements.

## Features

* Create a matrix with custom dimensions
* Input values manually
* Search for a specific number in the matrix
* Highlight occurrences of the searched number
* Display position (row and column)
* Show neighboring values:

  * Up
  * Down
  * Left
  * Right
* Handles edge cases (no neighbor available)

## Technologies

* Java
* Basic input/output (Scanner)
* Multidimensional arrays

## How It Works

1. The user defines the matrix size (rows and columns)
2. The matrix is filled manually
3. The user enters a number to search
4. The program:

   * Prints the matrix highlighting the number
   * Displays all positions where the number appears
   * Shows neighboring values for each occurrence

## How to Run

1. Clone the repository

```
git clone https://github.com/your-username/matrix-neighbor-finder.git
```

2. Navigate to the folder

```
cd matrix-neighbor-finder
```

3. Compile

```
javac application/Program.java
```

4. Run

```
java application.Program
```

## Example

Input:

```
3 3
1 2 3
4 5 6
7 8 5
```

Search:

```
5
```

Output:

* Positions where 5 appears
* Neighbor values for each position

## Improvements (Future Work)

* Add graphical interface
* Allow random matrix generation
* Improve input validation
* Support larger datasets with better performance

## Author

Richard Bryan
