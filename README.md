## Will the New web page invite more users and increase Purchase Conversion rate?
### Introduction
A/B testing is a Randomized controlled experiment in which a number of samples (e.g A and B) of different versions are compared with an aim **to measure and track certain 
metrics of Key Performance Indicators (KPIs)**, of various lines of business such as E-commerce.
It involves splitting a sample into sub-samples, one group being the **Control group** which does not receive the intervention, and the
other group being the **Treatment group** which actually receive the intervention and predict or track a given metric, such as Conversion rate.
There are two main approaches to A/B testing:
1. Frequentist Approach.
2. Bayesian Approach whis is based on the [Bayes Theorem](https://en.m.wikipedia.org/wiki/Bayes%27_theorem).
More about the two methods can be found here: [website](https://www.redjournal.org/article/S0360-3016(21)03256-9/fulltext).
---
### Overview
The dataset is for a certain E-commerce company that has developed a new web page in order to try and increase the number of users who "convert," meaning the
number of users who decide to make a product purchase. I aim this to assist the company understand if they should implement this new page or keep using the old page,
so as to improve or increase their [Purchase Conversion rate](https://www.hotjar.com/blog/website-conversion/).
The dataset had 294478 rows each representing a user interaction session/ Exposure, as well as five columns:
- *user_id* - The user ID of each exposure
- *timestamp* - The time at which the user was exposed
- *group* - The group the user was assigned to for that exposure {control, treatment)
- *landing_page* - The web version each user was exposed to
- *converted* - Whether the user actually made a purchase or not, after the exposure {0:not converted, 1:converted}.
1. **The two sub-sample groups are**:
* Control: Users who got the old web page.
* Treatment: Users who got the new web page.
2. **The metric we want to track**:
* Purchase Conversion rate = Converted users (users that actually made a purchase) / Exposed users (total users exposed)
I opted for The Bayesian Approach
### Conclusion
Running the entire experiment for 4 weeks, I found out that the **Purchase Conversion Rate** for the Control group was always higher than that for the Treatment group.
The confidence level kept on increasing which each new experiment data hence we become more confident that the Control Purchase Conversion rate is greater than that for the treatment group.
Also the variances of both the Control Posterior and the Treatment Posterior distributions reduces from the previous week results. This means that the distributions are getting narrower and more distinct hence making it easier to even quantify small differences.
Overall since the Purchase Conversion Rate of the Control group (Users who received the old web page) is **always greater** than that for the Treatment group (Users who got the new web page), it would be more effective for the E-commerce to keep using the old web page rather than introducing the new web page.
The new web page would not improve the Purchase Conversion Rate by any chance.

