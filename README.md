# ICS-Quadratic-solver--Grading-system---muya-mainza

## Quadratic Solver & Grading System 

This project implements a single-file web page (`index.html`) that combines two distinct functionalities: a **Quadratic Solver** and a **Grading System**.

1.  **Quadratic Solver**: Allows users to input coefficients `a`, `b`, and `c` for a quadratic equation $$ ax^2 + bx + c = 0 $$. It calculates and displays the discriminant and the nature of the roots (two distinct real roots, one real repeated root, or two complex conjugate roots), along with their numerical values. Includes input validation for coefficients.
2.  **Grading System**: Enables users to input a numerical score (0-100). It then determines and displays the corresponding letter grade based on a predefined scale. Includes input validation to ensure the score is within the valid range.

The entire application, including HTML structure, CSS styling, and JavaScript logic, is contained within a single `index.html` file, making it easy to deploy and run.

## How to Run

This project is a self-contained HTML file. To run it:

1.  **Save the code**: Copy the entire HTML code provided previously and save it as `index.html` (or any other `.html` file name) on your computer.
2.  **Open in a browser**: Navigate to the saved `index.html` file using your file explorer and double-click it. It will open automatically in your default web browser.
3.  **Interact**: Use the input fields and buttons provided on the page to test the Quadratic Solver and Grading System functionalities.

## Test Cases

Here are some test cases to verify the functionality and validation of both components:

### 1) Quadratic Solver

**Input Validation:**

*   **`a = 0`**:
    *   Input: `a=0`, `b=1`, `c=1`
    *   Expected Output: Error message: "Coefficient 'a' cannot be zero for a quadratic equation."
*   **Empty Input**:
    *   Input: `a=""`, `b=1`, `c=1`
    *   Expected Output: Error message: "Please enter a valid number for a." (Similar for b and c)
*   **Non-numeric Input**: (The `type="number"` input field typically prevents non-numeric input, but if manually bypassed or changed, the `isNaN` check would catch it.)
    *   Input: `a="abc"`, `b=1`, `c=1`
    *   Expected Output: Error message: "Please enter a valid number for a."

**Calculation Scenarios:**

*   **Two Distinct Real Roots (D > 0)**:
    *   **Test Case 1**: $$ x^2 - 3x + 2 = 0 $$
        *   Input: `a=1`, `b=-3`, `c=2`
        *   Expected Output:
            *   Discriminant (D): 1
            *   Nature of Roots: Two distinct real roots
            *   Root 1: 2.0000
            *   Root 2: 1.0000
    *   **Test Case 2**: $$ 2x^2 + 5x - 3 = 0 $$
        *   Input: `a=2`, `b=5`, `c=-3`
        *   Expected Output:
            *   Discriminant (D): 49
            *   Nature of Roots: Two distinct real roots
            *   Root 1: 0.5000
            *   Root 2: -3.0000
*   **One Real Repeated Root (D = 0)**:
    *   **Test Case 1**: $$ x^2 - 4x + 4 = 0 $$
        *   Input: `a=1`, `b=-4`, `c=4`
        *   Expected Output:
            *   Discriminant (D): 0
            *   Nature of Roots: One real repeated root
            *   Root: 2.0000
    *   **Test Case 2**: $$ 4x^2 + 4x + 1 = 0 $$
        *   Input: `a=4`, `b=4`, `c=1`
        *   Expected Output:
            *   Discriminant (D): 0
            *   Nature of Roots: One real repeated root
            *   Root: -0.5000
*   **Two Complex Conjugate Roots (D < 0)**:
    *   **Test Case 1**: $$ x^2 + x + 1 = 0 $$
        *   Input: `a=1`, `b=1`, `c=1`
        *   Expected Output:
            *   Discriminant (D): -3
            *   Nature of Roots: Two complex conjugate roots
            *   Root 1: -0.5000 + 0.8660i
            *   Root 2: -0.5
         
            *   for any contribution to the project requests are welcome 

   
