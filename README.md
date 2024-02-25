<h1 align="left">Resolution of the agriculture-related problem using PuLP</h1>

<h3 align="left">Report</h3>

<div align="left">
  <a href="https://drive.google.com/file/d/1a_MZ5JpEXpfT38x5LYSsyEMdSIE6U4Ns/view?usp=sharing">
    <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/googlecloud/googlecloud-original.svg" height="40" alt="googlecloud logo"  />
  </a>
</div>

<h2 align="left">Problem Statement</h2>

<p align="left">An agriculteur wants to allocate 150 hectares of irrigable land between the cultivation of tomatoes and peppers. He has 480 hours of labor and 440 m<sup>3</sup> of water available. Cultivating one hectare of tomatoes requires 1 hour of labor, 4 m<sup>3</sup> of water, and yields a net profit of 1000 dirhams. Cultivating one hectare of peppers requires 4 hours of labor, 2 m<sup>3</sup> of water, and yields a net profit of 2000 dirhams.<br><br>The irrigation office wants to protect the price of tomatoes and does not allow the agriculteur to cultivate more than 90 hectares of tomatoes. What is the best allocation of his resources ?</p>

## Solution Approach

To find the best allocation of resources, we can formulate this problem as a linear programming problem.

### Decision Variables
Let:
- \( x \) be the number of hectares of tomatoes to be cultivated.
- \( y \) be the number of hectares of peppers to be cultivated.

### Objective Function
We aim to maximize the net profit:
\[ \text{Maximize} \: Z = 1000x + 2000y \]

### Constraints
1. Land constraint: Total hectares allocated should not exceed 150 hectares.
\[ x + y \leq 150 \]

2. Labor constraint: Total hours of labor should not exceed 480 hours.
\[ x + 4y \leq 480 \]

3. Water constraint: Total water usage should not exceed 440 m^3.
\[ 4x + 2y \leq 440 \]

4. Tomato cultivation limit: The agriculteur cannot cultivate more than 90 hectares of tomatoes.
\[ x \leq 90 \]

### Solution
We can use linear programming solvers like the Simplex method or interior-point methods to solve this optimization problem and find the optimal values of \( x \) and \( y \).
