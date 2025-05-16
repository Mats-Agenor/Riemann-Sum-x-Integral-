#Riemann Sum x Integral 

---------------------

This Mathematica notebook was developed as part of a Calculus activity for the Physics course at UNESP in Bauru. The main objective is to compare two methods of calculating the area under a curve:

1. **Exact Integral**: The symbolic computation of the definite integral using Mathematica's powerful symbolic math capabilities
2. **Riemann Sum**: A numerical approximation using the right-endpoint method with a large number of divisions

The implementation demonstrates how numerical methods (Riemann sums) approximate analytical solutions (exact integrals), which is a fundamental concept in calculus with important applications in physics.

## Implementation Details

The code performs the following operations:

1. Defines a mathematical function to analyze (default: `Sin[x] + Cos[x^2]`)
2. Sets an integration interval (default: `[0, 2π]`)
3. Calculates:
   - The Riemann sum approximation using 1 million subdivisions (configurable)
   - The exact integral value using symbolic computation
4. Compares the results by showing:
   - Both numerical values
   - Absolute difference
   - Relative percentage difference
5. Generates presentation-quality visualizations:
   - Left plot: Shows the Riemann sum approximation (displaying 100 subdivisions for visual clarity)
   - Right plot: Shows the exact integral as the area under the curve

## Performance Note

The original implementation uses 1 million divisions (`n = 1,000,000`) for high-precision approximation. However, on modest hardware (e.g., an i3 10th gen processor with 12GB RAM), this configuration may cause Mathematica to crash or become unresponsive. 

**Recommended adjustment**: Reduce the number of divisions to 10,000 (`n = 10,000`) for stable performance while still maintaining reasonable accuracy for educational purposes.

---------------------------------

## Final Considerations

This notebook represents one of my final implementations in the Wolfram Language. While Mathematica excels at symbolic computation and provides an excellent environment for mathematical exploration, I've found that for large-scale numerical computations like this Riemann sum calculation, Python often offers better performance and memory efficiency. This performance consideration, among others, has led me to transition my computational work primarily to Python-based solutions.

The notebook remains valuable for educational purposes, clearly demonstrating the relationship between numerical approximations and exact solutions in calculus, and providing visual intuition about the Riemann sum method and its convergence to the integral as the number of divisions increases.
