<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>NML Group Project</title>
</head>
<body>
  <h1>NML Group Project</h1>
  <p>
    This project is about solving different types of equations and finding their roots. We have learned about solving 
    Linear Equations, Non-linear Equations, Ordinary Differential Equations, and the Matrix Inversion Process. The group members are:
  </p>
  <ul>
    <li><strong>Abu Jar Gefaree Sayeem</strong><br>Roll: 2107033</li>
    <li><strong>Mahhia Kamal Mim</strong><br>Roll: 2107081</li>
    <li><strong>Al Nahian Zarif</strong><br>Roll: 2107098</li>
  </ul>

  <h2>Non Linear Equations - Al Nahian Zarif</h2>

  <h3>1. Bisection Method for Finding Polynomial Roots</h3>
  <p>
    The bisection method is a numerical technique used to find the roots of a polynomial within a given interval. 
    This method is particularly useful when the polynomial does not have an analytical solution or when it is 
    difficult to find the roots algebraically. The bisection method works by iteratively narrowing down the interval 
    in which the root lies until a satisfactory approximation is obtained.
  </p>

  <h4>Algorithm</h4>
  <ol>
    <li>Start with an interval [a, b] such that the function changes sign at the endpoints a and b.</li>
    <li>Calculate the midpoint c = (a + b) / 2.</li>
    <li>Evaluate the function at the midpoint c.</li>
    <li>If the function value at c is close enough to zero (i.e., within a specified tolerance), then c is considered as the root and the algorithm terminates.</li>
    <li>Otherwise, determine which half of the interval [a, b] to continue with based on the sign of the function at the midpoint.</li>
    <li>Repeat steps 2-5 with the new interval until the function value at the midpoint is sufficiently close to zero.</li>
  </ol>

  <h4>Implementation</h4>
  <ol>
    <li>Define a function to evaluate the polynomial at a given x using its coefficients.</li>
    <li>Implement the bisection method to find the root of the polynomial within a specified interval.</li>
    <li>Input the coefficients of the polynomial and the interval [a, b].</li>
    <li>Check if the function has different signs at the endpoints of the interval.</li>
    <li>If the condition is satisfied, call the bisection method to find the root and output the result.</li>
  </ol>

  <h4>Example</h4>
  <p>
    Consider a polynomial with coefficients [1, -3, 0, 1, 1, -5, 2] for x^6 to x^0. To find a root of this polynomial 
    within the interval [1, 2] with a tolerance of 0.001, entering the coefficients and interval into the program 
    yields a result with a root of approximately 1.73205.
  </p>

  <h3>2. False Position Method for Finding Polynomial Roots</h3>
  <p>
    The false position method, also known as the regula falsi method, is an iterative technique for finding the 
    roots of a polynomial equation within a specified interval. It is based on the intermediate value theorem, 
    which states that if a continuous function changes sign over an interval, then it must have at least one root within that interval.
  </p>

  <h4>Implementation</h4>
  <ol>
    <li>Input coefficients for the polynomial from the user.</li>
    <li>Input the interval [a, b] where the function changes sign.</li>
    <li>Input the tolerance for the root approximation.</li>
    <li>Check if the function has different signs at the endpoints of the interval.</li>
    <li>Apply the false position method to find the root of the polynomial within the specified interval and tolerance.</li>
  </ol>

  <h4>Example</h4>
  <p>
    Consider a polynomial with coefficients for (x^6) to (x^0): 2x^6 - 4x^5 + 3x^4 - 6x^3 + 8x^2 - 5x + 7. Finding 
    the root of this polynomial within the interval [1, 3] with a tolerance of 0.0001 yields a root of approximately 1.73205.
  </p>

  <h3>3. Secant Method for Finding Polynomial Roots</h3>
  <p>
    The Secant Method is a numerical technique used to find the roots of a polynomial. It is an iterative process 
    that uses two initial guesses to approximate the root of the polynomial within a specified tolerance.
  </p>

  <h4>Implementation in C++</h4>
  <ol>
    <li>Input the coefficients of the polynomial from highest power to lowest power.</li>
    <li>Enter two initial guesses for the root.</li>
    <li>Specify the tolerance for the root approximation.</li>
  </ol>

  <h4>Example</h4>
  <p>
    Suppose we have a polynomial with the following coefficients: 1, -3, 0, 4, -2, 1, -5. Using initial guesses x0 = 1 
    and x1 = 2 with a tolerance of 0.0001, running the program with these inputs yields an approximate root of 1.00003.
  </p>

  <h3>4. Newton-Raphson Method for Finding Polynomial Roots</h3>
  <p>
    The Newton-Raphson method is a powerful numerical technique used to find the roots of a polynomial equation. 
    It is particularly useful for finding the roots of nonlinear equations, including polynomial equations.
  </p>

  <h4>Implementation</h4>
  <ol>
    <li>Define a function to evaluate the polynomial at a given x.</li>
    <li>Implement a function to evaluate the derivative of the polynomial at a given x.</li>
    <li>Implement the Newton-Raphson formula to iteratively find the root within the specified tolerance.</li>
    <li>Input the coefficients, an initial guess for the root, and a tolerance for the approximation.</li>
  </ol>

  <h4>Example</h4>
  <p>
    To find the root of a polynomial with coefficients: 1, -3, 0, 2, 0, 1, -5. Using an initial guess of 1 and a 
    tolerance of 0.0001, the result approximates a root to 1.73205.
  </p>
</body>
</html>
