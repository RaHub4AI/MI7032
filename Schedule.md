# 📘 Course Schedule (MI7032)

```mermaid
gantt
    title Dataanalys – Verktyg för miljövetare (Autumn 2025)
    dateFormat  YYYY-MM-DD
    axisFormat  %d %b

    section Week 40
    [Introduction](./Introduction_to_R_and_Python)       :a1, 2025-10-02, 0.5d
    [Getting Started Workshop](./Introduction_to_R_and_Python) :a2, after a1, 0.5d
    [Tools Workshop](./Introduction_to_R_and_Python)     :a3, 2025-10-03, 1d

    section Week 41
    [Descriptive Statistics](./Descriptive_Statistics_and_Data_Visualization) :b1, 2025-10-06, 0.5d
    [Self-study HW1](./Homeworks)                        :b2, after b1, 1.5d
    [Data Distributions](./Descriptive_Statistics_and_Data_Visualization) :b3, 2025-10-07, 0.5d
    [Statistical Thinking](./Descriptive_Statistics_and_Data_Visualization) :b5, 2025-10-08, 0.5d
    [Hypothesis Testing I (t-test)](./Hypothesis_Testing) :b7, 2025-10-09, 0.5d
    [Self-study HW2](./Homeworks)                        :b8, after b7, 1.5d
    [HW I Submission 🔴](./Homeworks)                    :milestone, after b2, 2025-10-09, 0d
    [Hypothesis Testing I (F-test, Normality)](./Hypothesis_Testing) :b9, 2025-10-10, 0.5d

    section Week 42
    [Hypothesis Testing II](./Hypothesis_Testing)        :c1, 2025-10-13, 0.5d
    [Self-study HW2](./Homeworks)                        :c2, after c1, 1d
    [ANOVA & p-hacking](./Hypothesis_Testing)            :c3, 2025-10-14, 0.5d
    [Longitudinal Data Analysis](./Hypothesis_Testing)   :c5, 2025-10-15, 0.5d
    [Covariance & Correlation](./Regression_and_Correlation) :c7, 2025-10-16, 0.5d
    [Self-study HW3](./Homeworks)                        :c8, after c7, 1d
    [HW II Submission 🔴](./Homeworks)                   :milestone, after c2, 2025-10-16, 0d
    [Regression (Linear)](./Regression_and_Correlation)  :c9, 2025-10-17, 0.5d

    section Week 43
    [Regression (Logistic)](./Regression_and_Correlation):d1, 2025-10-20, 0.5d
    [Self-study HW3](./Homeworks)                        :d2, after d1, 1d
    [Confidence Intervals](./Regression_and_Correlation) :d3, 2025-10-21, 0.5d
    [Supervised Learning](./Introduction_to_Machine_Learning) :d5, 2025-10-22, 0.5d
    [Self-study HW4](./Homeworks)                        :d6, after d5, 1d
    [HW III Submission 🔴](./Homeworks)                  :milestone, after d2, 2025-10-22, 0d
    [Unsupervised Learning](./Introduction_to_Machine_Learning) :d7, 2025-10-23, 0.5d
    [Performance Metrics](./Introduction_to_Machine_Learning) :d9, 2025-10-24, 0.5d

    section Week 44
    [Take-home Exam](./Project)                          :e1, after d9, 2025-10-27, 5d
    [HW IV Submission 🔴](./Homeworks)                   :milestone, after d6, 2025-10-27, 0d
    Mid-Exam Presentations                               :e2, 2025-10-29, 0.5d
    Q&A Session                                          :e3, after e2, 0.5d
    [Final Exam Submission 🔴](./Project)                :milestone, after e1, 2025-10-31, 0d
