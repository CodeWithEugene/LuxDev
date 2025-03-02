# The govt of kenya has introduced a new policy on free education aimed at improving the overall well-being of a child. The govt aims to move a child expectancy from 5yrs to 10yrs. Its std deviation 2.5.Use hypothesis testing to check whether the policy will improve the child expectancy.Take n = 50
To test whether the new policy will improve child expectancy, we can set up the following hypothesis test:

- Null Hypothesis (H0): The policy does not improve child expectancy (mean = 5 years).
- Alternative Hypothesis (H1): The policy improves child expectancy (mean > 5 years).

Given:
- Population standard deviation (σ) = 2.5 years
- Sample size (n) = 50
- Significance level (α) = 0.05

We use a one-sample z-test for the mean. The test statistic is calculated as:

$$ z = \frac{\bar{x} - \mu}{\sigma / \sqrt{n}} $$

Where:
- \( \bar{x} \) is the sample mean  
- \( \mu \) is the population mean (5 years)  
- \( \sigma \) is the population standard deviation  
- \( n \) is the sample size  

If the calculated z-value is greater than the critical value from the z-table, we reject the null hypothesis.

# Read about Resampling methods and Montecarlo Simulation
Resampling methods involve repeatedly drawing samples from a data set and assessing the variation in a statistic of interest. Common resampling methods include:

- **Bootstrapping**: This method involves repeatedly sampling with replacement from the original data set to create many simulated samples. It is used to estimate the sampling distribution of a statistic and to calculate confidence intervals.
- **Permutation Tests**: This method involves repeatedly shuffling the data labels and calculating the test statistic for each permutation. It is used to test hypotheses and assess the significance of observed effects.

Monte Carlo Simulation involves using random sampling to obtain numerical results. It is often used to model the probability of different outcomes in a process that cannot easily be predicted due to the intervention of random variables. Key aspects of Monte Carlo Simulation include:

- **Random Sampling**: Generating random samples from a probability distribution to simulate the behavior of a system or process.
- **Numerical Results**: Using the generated samples to compute estimates of statistical measures, such as means, variances, and probabilities.
- **Applications**: Monte Carlo Simulation is widely used in fields such as finance, engineering, and physics to model complex systems and assess the impact of uncertainty.

Both resampling methods and Monte Carlo Simulation are powerful tools for statistical analysis and decision-making, especially when dealing with complex data and uncertainty.

# What is Meta-analysis and its relation to effect size
- Meta-analysis is a statistical technique for combining the findings from independent studies. 
- It is often used to assess the effectiveness of healthcare interventions. 
- Effect size is a measure of the strength of the relationship between two variables. 
- In meta-analysis, effect sizes from different studies are combined to get an overall estimate of the effect.

# Difference between CDF and ECDF
- CDF (Cumulative Distribution Function) describes the probability that a random variable takes on a value less than or equal to a certain value.
- ECDF (Empirical Cumulative Distribution Function) is a step function that estimates the CDF from a sample of data.

# Weekly Article: Write about the different classification metrics, why and when we use them and give examples
[Here](https://dev.to/eugeniuss/classification-metrics-understanding-their-role-usage-and-examples-4c5f) is my article.