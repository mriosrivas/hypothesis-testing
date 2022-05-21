# Hypothesis and A/B testing

This repository contains information about hypothesis and A/B testing for future reference. Here I describe basic concepts and deploy two Jupyter Notebooks:



1. [Hypothesis testing definition and example](Hypothesis_Testing.ipynb).

2. [A/B testing](AB_Testing.ipynb)



## Null and Alternative Hypothesis

Null hypothesis $H_0$:

* Considered to be true before we collect data.

* Holds some sort of equals sign $= \leq \geq$



Alternative hypothesis $H_1$:

* What we want to be true.

* Holds the opposite sign $\neq < >$



Examples:

$H_0$: The average height of all people in the world is less than or equal to 68 inches tall.

$H_1$: The average height of all people in the world is different than 68 inches tall.

$H_0$: The impact of Drug A is on average the same as Drug B.

$H_1$: Drug A will have on average a larger impact than Drug B.



## Error Types

Type I Errors ($\alpha$):

* Choosing $H_1$ when $H_0$ is true.

* False positives

Type II Error ($\beta$):

- Choosing $H_0$ when $H_1$ is true.

- False negatives



## Case Example

Consider you are testing a new cancer drug to see if it reduces tumor sizes in patients. Let $\mu_n$ be the **average reduction** in tumor size under the **new** drug. Let $\mu_o$ be the **average reduction** in tumor size under the **old** drug.



We set up the null and alternative hypotheses in the following way:



The average reduction in tumor size under the new drug **is less or equal** than the average reduction in tumor size under the old drug.

$H_0: \mu_n-\mu_o \leq 0$



The average reduction in tumor size under the new drug **is greater** than the average reduction in tumor size under the old drug.

$H_1: \mu_n-\mu_o \gt 0$

![Alt text](/media/manuel/storage/Courses/Udacity/Notes/confussion_matrix.png "a title")

Example of a Type I error can be:

Based on the study results we decide the new drug ($H_1$) is better, but really the old drug ($H_0$) is better at reducing tumor sizes.



Example of a Type II error can be:

Based on the study results we decide the old drug ($H_0$) is better, but really the new drug ($H_1$) is better at reducing tumor sizes.
