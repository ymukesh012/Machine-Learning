Predicting Student Scores Using Linear Regression

This project demonstrates a simple linear regression to predict student scores based on the number of hours studied.

| Hours (x) | Score (y) |
| --------- | --------- |
| 1         | 52        |
| 2         | 57        |
| 3         | 65        |
| 4         | 70        |
| 5         | 75        |
| 6         | 80        |

------------------------------------------------
Step 1: Calculate the Slope (m)

Formula:

m = (n * Σ(xy) - Σx * Σy) / (n * Σ(x^2) - (Σx)^2)



Compute sums:


n = 6
Σx = 1 + 2 + 3 + 4 + 5 + 6 = 21

Σy = 52 + 57 + 65 + 70 + 75 + 80 = 399

Σx² = 1² + 2² + 3² + 4² + 5² + 6² = 91

Σxy = 152 + 257 + 365 + 470 + 575 + 680 = 1496




Slope calculation:

m = (6*1496 - 21*399) / (6*91 - 21^2)
m = (8976 - 8379) / (546 - 441)
m = 597 / 105 ≈ 5.686

------------------------------------------------------
Step 2: Calculate the Intercept (c)

Formula:
c = (Σy - m*Σx) / n

c = (399 - 5.686*21) / 6
c = (399 - 119.406) / 6
c = 279.594 / 6 ≈ 46.599


--------------------------------------------------------
Linear Regression Equation
y ≈ 5.686*x + 46.599


--------------------------------------------------------
Example Prediction

If a student studies 10 hours:

y = 5.686*10 + 46.599 ≈ 103.46

⚠️ Note: Scores usually cap at 100. A prediction above 100 shows a strong positive trend.

