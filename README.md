# Experimental-Design-A-B-Testing-for-Learning-Strategy-Optimization

# Optimizing Learning Strategies: Active vs. Passive Learning

This repository presents the results and methodology of an experimental study evaluating the effects of **active vs. passive learning** on student engagement, comprehension, and classroom participation.

**Study Title**: *Optimizing Learning Strategies: Evaluating the Impact of Active vs. Passive Learning on Student Engagement and Comprehension*

---

## Research Question

**Does active learning lead to higher student engagement and perceived preparedness compared to passive learning?**

---

## Summary

We conducted a randomized controlled trial among MSBA students at Boston University, comparing:
- **Control Group (Passive Learning)**: Received pre-written notes on a case study.
- **Treatment Group (Active Learning)**: Completed an interactive quiz with instant feedback.

Surveys before and after the learning task — and again post-class — measured:
- Perceived preparedness
- Recall of the material
- Class participation

---

## Experimental Design

- **Randomization**: Stratified random assignment by gender.
- **Survey Platform**: Qualtrics with BU email authentication.
- **Pre-Experiment Survey**: Captured demographics and baseline covariates.
- **Intervention**:
  -  Passive: Notes
  -  Active: Quiz with scoring, feedback
- **Post-Experiment Surveys**: Measured recall, understanding, and engagement.

---

## Outcome Metrics

| Variable                         | Description                                                | Scale       |
|----------------------------------|------------------------------------------------------------|-------------|
| `Post_Class_Recall_Val`          | Self-reported recall of case material                      | 0–100       |
| `Post_Class_Participation_Val`   | Participation in class discussion                          | 0–100       |
| `RQ1_Understand_Material_Val`    | Pre-class understanding of the content                     | 0–100       |

---

## Key Findings

### Treatment Effect (ATE)
| Metric                    | ATE    | P-Value | Interpretation                      |
|--------------------------|--------|---------|-------------------------------------|
| Post Class Recall        | -2.65  | 0.75    | No significant effect               |
| Class Participation      | +4.34  | 0.71    | Slight, non-significant increase    |
| Understanding Material   | +5.03  | 0.20    | Small, non-significant improvement  |

### Heterogeneous Effects (CATE)
- **Gender**:
  - Males showed higher participation & perceived understanding in the active group.
  - Females showed better comprehension but no change in participation.

- **Case Reading**:
  - Students who **didn't read the case** but received active learning:
    - +53% participation
    - -35% recall (suggesting cognitive overload)
  - Students who **read the case** saw modest improvements in both recall and comprehension.

---

## Regression Insights

- **Active learning** slightly benefited students who were already engaged or had prior knowledge.
- **Pre-existing intent to participate** was the strongest predictor of actual class participation.
- **Gender and prior exposure** significantly moderated the treatment effect.
- Model R² values were low (≈ 0.10), suggesting other unexplored variables influence outcomes.

---

## Limitations

- Limited sample size (N < 60) led to low statistical power.
- Higher dropout rate in active group due to survey length or complexity.
- Self-reported measures are subject to bias.
- Potential spillover between treatment/control groups.

---

## Conclusion

While **active learning** did not significantly outperform **passive learning** overall, its effectiveness varied:
- Works better for students with prior preparation or intrinsic motivation
- May increase engagement but not necessarily comprehension
- Design and demographic considerations are critical to effectiveness

---

## Business Implications

- **Corporate training** and **onboarding programs** can benefit from adaptive content tailored by demographic.
- **Gamified quizzes** and **interactive modules** improve engagement when learners are primed.
- Customizing training delivery based on employee baseline knowledge may improve ROI.

---

## Future Work

- Explore larger, more diverse samples
- Use objective outcome measures (e.g., quiz scores vs. self-report)
- Investigate adaptive learning models that respond to learner profiles
- Examine long-term retention and behavioral changes
