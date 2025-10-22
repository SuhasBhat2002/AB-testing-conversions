# A-B-testing-conversions

## Why A/B Testing Matters
Data-Driven Decision Making: Rather than relying on intuition or assumptions about what users might prefer, A/B testing provides tangible evidence of actual user behavior and preferences. This approach ensures that product decisions are grounded in reality rather than speculation, significantly reducing the risk of implementing changes that could negatively impact user engagement or business metrics.

## A/B Test Dataset Description
The dataset used for the A/B test contains information about user interactions with the new feature. It includes four primary columns: user_id, views, clicks, and group. Each record represents an individual user’s exposure and response to the feature during the experiment period.

user_id: A unique identifier for each participant in the test. It ensures that individual-level interactions can be tracked without revealing personal information.

views: The number of times a user was shown the feature or had the opportunity to interact with it. This serves as the exposure variable used to calculate engagement metrics such as click-through rate (CTR).

clicks: The number of times the user actually clicked or engaged with the feature. This represents the action being tested and is the core measurement of user interest or conversion.

group: Indicates whether the user belonged to the control or variant group. The control group represents the original version of the product or feature, while the variant group contains users who experienced the new version being tested.

## Report 
============================================================
A/B TEST EVALUATION REPORT
============================================================

1. STATISTICAL SIGNIFICANCE
   Chi-square statistic: 43.0898
   P-value: 0.000000
   Degrees of freedom: 1
   ✅ Result: STATISTICALLY SIGNIFICANT (p < 0.05)

2. CONVERSION RATES
   Control: 21.5292% (95% CI: [21.2149%, 21.8469%])
   Treatment: 23.0462% (95% CI: [22.7240%, 23.3715%])

3. LIFT ANALYSIS
   Absolute lift: +1.5169% (1.52 percentage points)
   Relative lift: +7.05%

4. PRACTICAL SIGNIFICANCE
   Business threshold: 10%
   ⚠️ Result: NOT PRACTICALLY SIGNIFICANT
      Lift (7.05%) below threshold (10%)

5. RECOMMENDATION
   🛑 DON'T SHIP: Statistically significant but lift too small
============================================================


