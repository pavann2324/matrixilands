# Matrix Islands with Diagonals

This project provides a web-based tool to calculate the number of islands in a binary matrix (0s and 1s). It supports diagonal connectivity, allowing islands to span all 8 directions (up, down, left, right, and diagonals).

## Features

- **Input Flexibility**: Accepts a binary matrix as input, with rows separated by new lines and cells by spaces.
- **Diagonal Connectivity**: Counts islands considering 8 possible directions.
- **Responsive Output**: Displays the number of islands or provides an error message for invalid input.

## Technologies Used

- **HTML5**: Builds the structure of the web page.
- **CSS3**: Adds an elegant and modern user interface with gradient backgrounds and smooth interactions.
- **JavaScript**: Implements the core logic for matrix validation and island counting.

## Usage

1. **Input the Matrix**:
   - Enter a binary matrix of `0`s and `1`s in the text area. Separate rows with new lines and cells with spaces.
   - Example input:
     ```
     1 1 0 0
     0 1 0 0
     0 0 1 0
     1 0 0 1
     ```

2. **Count Islands**:
   - Click the **Count Islands** button.
   - The application will display the number of islands in the matrix.

3. **Examples**:
   - Input:
     ```
     1 1 0
     0 1 0
     0 0 1
     ```
     Output: `2` islands.

   - Input:
     ```
     1 0 1
     0 0 0
     1 1 1
     ```
     Output: `3` islands.

## How It Works

1. **Matrix Validation**:
   - Checks if all rows have the same length.
   - Ensures all cells contain either `0` or `1`.

2. **Island Counting Algorithm**:
   - Uses a Depth-First Search (DFS) approach to traverse connected `1`s in all 8 possible directions.
   - Marks visited cells to avoid redundant calculations.
   - Increments the island count whenever a new unvisited `1` is found.

3. **Error Handling**:
   - Displays an error message for:
     - Non-binary or non-uniform matrices.
     - Empty or invalid input.

## Design Highlights

- **Modern UI**:
  - Frosted glass container with gradient background.
  - Smooth transitions and hover effects.
  - Focused input field with dynamic styling.

- **Clear Output**:
  - Displays results in a styled box with distinct formatting for errors.

