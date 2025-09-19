# Udacity Free Trial Screener A/B Testing Project

This project analyzes an A/B test conducted by Udacity to assess the impact of an additional screening step during free trial enrollment in their courses.

---

## Experiment Overview

- **Control Group:** Standard course overview page. Students can choose "Start free trial" or "Access course materials".
- **Treatment Group:** After clicking "Start free trial", students are asked how much time they can devote per week. If less than 5 hours, they're encouraged to access course materials for free but can still continue with the trial.

---

## Experiment Design

- **Unit of Diversion:** Cookie (browser/device).
- **Invariant Metrics:**  
  - Number of cookies (pageviews)  
  - Number of clicks  
  - Click-through probability
- **Evaluation Metrics:**  
  - **Gross Conversion:** Enrollments per click  
  - **Net Conversion:** Paid conversions per click

*Retention* was considered but rejected as a main metric due to sample size and duration constraints.

---

## Key Findings

- **Sanity checks:** Passed for all invariant metrics.
- **Gross conversion:** Decreased by ~2% (statistically & practically significant).
- **Net conversion:** No statistically or practically significant change.

**Interpretation:**  
The experiment reduced free trial enrollments—filtering out less committed users—but did not increase the proportion of paying users. Therefore, the change does not provide a clear business benefit.

---

## Recommendations

- **Do not launch** the tested screener as-is.
- Consider a follow-up experiment:
  - Improve the pre-enrollment screener to include prerequisite knowledge checks.
  - Make free course materials more accessible to users with low time/commitment or lacking prerequisites.
  - For enrolled users, experiment with forming student groups led by mentors to boost retention.

---

## Credits

- [baumanab/udacity_ABTesting](https://github.com/baumanab/udacity_ABTesting#summary)
- [Kaggle: Udacity A/B Testing Final Course Project](https://www.kaggle.com/mariusmesserschmied/udacity-a-b-testing-final-course-project)

---
