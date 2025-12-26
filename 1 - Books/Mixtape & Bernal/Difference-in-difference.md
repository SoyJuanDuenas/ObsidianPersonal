#quasi-experimental
The Difference-in-differences method is a [[quasi-experimental method]] approach that use [[longitudinal data]] to compare the changes in outcomes over time between a population enrolled in a program like a state intervention (the treatment group) and a population that is not (the comparison group), as we can see, this method try to mimic a experimental research design using a [[natural experiment]]. It is a useful tool for [[data analysis]].

Difference-in-differences takes the before-after difference in treatment group’s outcomes. This is the first difference. In comparing the same group to itself, the first difference controls for factors that are constant over time in that group. Then, to capture time-varying factors, difference-in-differences takes the before-after difference in the control group, which was exposed to the same set of environmental conditions as the treatment group. This is the second difference. Finally, difference-in-differences “cleans” all time-varying factors from the first difference by subtracting the second difference from it. This leaves us with the impact estimation – or the difference-in-differences.
# When we use Difference in Difference ?

DID usually is used to estimate the treatment effect on the treated (causal effect in the exposed) We use this technique in observational settings where we have to measure the effects of a intervention in which exchangeability between the treatment and control groups cannot be assumed, that means that in absence of treatment the unobserved differences between treatment and control groups are the same overtime. Also Difference-in-difference is a useful technique to use when randomization on the individual level is not possible. DID requires data from pre-/post-intervention, such as cohort or panel data (individual level data over time) or repeated cross-sectional data (individual or group level).
## Assumptions

In order to estimate any causal effect, three assumptions must hold: exchangeability, positivity, and Stable Unit Treatment Value Assumption ([[SUTVA]]) DID estimation also requires that:

- Intervention unrelated to outcome at baseline (allocation of intervention was not determined by outcome) 
- Treatment/intervention and control groups have Parallel Trends in outcome (in the absence of treatment, the difference between the ‘treatment’ and ‘control’ group is constant over time)  
- Composition of intervention and comparison groups is stable for repeated cross-sectional design (part of [[SUTVA]])    
- No spillover effects (part of [[SUTVA]])

 In order to increase the likelihood of the parallel trend assumption holding, a difference-in-differences approach is often combined with [matching](https://en.wikipedia.org/wiki/Matching_(statistics) "Matching (statistics)")

# Implementation

Assume that the event of treatment in question occurs between periods one an two, Type B
is treated, type a is the control.

$\delta_{DD} = (\overline{Y}_{B,2} - \overline{Y}_{A,2}) - (\overline{Y}_{B,1} - \overline{Y}_{A,1})$
$\delta_{DD}$ = Effect of treatment on outcome $Y$ (Average Treatment Effect)

So, that's mean that $\delta_{DD}$ is the difference across types **after** treatment, and the difference **before** treatment.

We can resume the meaning of $Y$ types in the next table:


|                        |     Control (A)      |     Treated (B)      |
| :--------------------: | :------------------: | :------------------: |
| **Pre-Treatment (1)**  | $\overline{Y}_{A,1}$ | $\overline{Y}_{B,1}$ |
| **Post-Treatment (2)** | $\overline{Y}_{A,2}$ | $\overline{Y}_{B,2}$ |




# Bibliography

- World Bank https://dimewiki.worldbank.org/Difference-in-Differences#:~:text=The%20difference%2Din%2Ddifferences%20method,useful%20tool%20for%20data%20analysis.
- Columbia https://www.publichealth.columbia.edu/research/population-health-methods/difference-difference-estimation
- Wikipedia https://en.wikipedia.org/wiki/Difference_in_differences



