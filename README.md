# CS571_Project_Implementation

## What Drives Ground-Level Ozone in Aotizhongxin, Beijing?

## Overview
This project uses the Beijing Multi-Site Air Quality Dataset (UCI) to analyze which weather factore most influences ground-level ozone concentrations, noted as O3.

## Files in this Repository
- `CS571Project.Rmd` - R Markdown source code with full analysis pipeline
- `CS571Project.html` - Knitted HTML report
- `CS571Project_HTML_Version.pdf` - Viewable knitted HTML report showing inputs, outputs, and comments
- `CS571RunningMarkdown` - Links to view the running R markdown file on browser
- `PRSA_Data_Aotizhongxin_20130301-20170228.csv` - The dataset (Aotizhongxin station)

## Methods Used
In this project, I first do exploratory data analysis of the data set with metrics and summaries. Then, I use regression methods including linear, ridge, and lasso regression. I also use the Best Subset Selection technique. Cross-validation is used to see how well the model worked.

## Results
The Lasso model (main model focused on) identified Temperature (TEMP) and Wind Speed (WSPM) as the strongest positive drivers of ozone, while Pressure (PRES) showed a negative effect. Numerical results are still being analyzed, and will be included in the final report.

## How to Run
1. Open `CS571Project.Rmd` in RStudio.
2. Run All
3. Click "Knit" to reproduce the HTML report.

## References
- [1] G. James, D. Witten, T. Hastie, and R. Tibshirani, “An Introduction to Statistical Learning with Applications in R Second Edition,” 2021. Accessed: July 26, 2026. Chapters #2 - #9: R Lab Codes
- [2] G. James, D. Witten, T. Hastie, and R. Tibshirani, “An Introduction to Statistical Learning with Applications in R Second Edition,” 2021. Accessed: July 26, 2026. [Online]. Available: https://www.casact.org/sites/default/files/2022-12/James-G.-et-al.-2nd-edition-Springer-2021.pdf
- [3] “UCI Machine Learning Repository.” Accessed: July 26, 2026. [Online]. Available: https://archive.ics.uci.edu/dataset/501/beijing+multi+site+air+quality+data
- [4] moonheadsing, “Scatterplot Matrices | R-bloggers,” Jan. 2013. Accessed: July 26, 2026. [Online]. Available: https://www.r-bloggers.com/2013/01/scatterplot-matrices/
- [5] Peter, “The Importance of Dewpoint Measurement in Ozone Generation,” Shaw Moisture Meters, Feb. 27, 2026. https://www.shawmeters.com/the-role-of-dewpoint-measurement-in-ozone-generation/ (accessed July 27, 2026).
- [6] M. Rodríguez-Peña, J. A. Barrios Pérez, J. Lobato, C. Saez, C. E. Barrera-Díaz, and M. A. Rodrigo, “Influence of pressure and cell design on the production of ozone and organic degradation,” Separation and Purification Technology, vol. 297, p. 121529, June 2022, doi: 10.1016/j.seppur.2022.121529.
- [7] L. Burrows, “The Complex Relationship between Heat and Ozone,” Apr. 2016. Accessed: July 26, 2026. [Online]. Available: https://news.harvard.edu/gazette/story/2016/04/the-complex-relationship-between-heat-and-ozone/
- [8] US EPA, “Trends in Ozone Adjusted for Weather Conditions | US EPA,” July 2018. Accessed: July 26, 2026. [Online]. Available: https://www.epa.gov/air-trends/trends-ozone-adjusted-weather-conditions
- [9] https://www.researchgate.net/post/What-does-it-indicating-If-there-is-positive-correlation-but-negative-regression-coefficient
- [10] “Simpson’s Paradox.” Accessed: July 26, 2026. [Online]. Available: https://discovery.cs.illinois.edu/learn/Basics-of-Data-Science-with-Python/Simpsons-Paradox/
- [11] H. Akoglu, “User’s Guide to Correlation Coefficients,” Turkish Journal of Emergency Medicine, vol. 18, no. 3, pp. 91–93, 2018, doi: 10.1016/j.tjem.2018.08.001.
- [12] “Best Subsets Regression in R with leaps (regsubsets),” Datanovia, June 25, 2026. https://www.datanovia.com/learn/machine-learning/model-selection/best-subsets-regression (accessed July 27, 2026).
- [13] D. Lass, “Machine Learning for Beginners, Part 11: Ridge Regression,” Medium, May 2018. https://medium.com/@laurahkahn/machine-learning-for-beginners-part-11-ridge-regression-9c606c764c2a (accessed July 27, 2026).
- [14] Ujang Riswanto, “A Beginner’s Guide to LASSO Regression: When and How to Use It,” Nov. 2024. Accessed: July 26, 2026. [Online]. Available: https://ujangriswanto08.medium.com/a-beginners-guide-to-lasso-regression-when-and-how-to-use-it-dc872e4ee489
- [15] “cv.glmnet function - RDocumentation,” Rdocumentation.org, 2026. https://www.rdocumentation.org/packages/glmnet/versions/5.0/topics/cv.glmnet (accessed July 27, 2026).
