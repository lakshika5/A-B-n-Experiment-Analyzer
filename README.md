# A/B/n Experiment Analyzer

## Overview
Excel-based A/B/n testing framework comparing 3 variants (Control, Test_A, Test_B) with n=150 users.

## Key Features
- **Summary Metrics**: Conversion rate, Revenue per user, Lift vs Control
- **Statistical Tests**: t-test (pairwise) + ANOVA (overall)
- **Decision Framework**: Launch / Retest / Reject logic
- **Business Impact**: Revenue analysis with significance

## Results
| Variant | Conversion | Revenue/User | Lift | Significant |
|---------|------------|--------------|------|-------------|
| Control | 32% | $10.60 | - | Baseline |
| Test_A | 32% | $12.00 | 0% | No (p=1.00) |
| Test_B | 30% | $8.38 | -6.25% | Yes (p=0.0048) |

## Decision
**❌ REJECT** - No variant outperformed Control. Test_B performed significantly worse.

## Recommendation
Run new experiment with different variants.

## Tools Used
Excel: COUNTIFS, SUMIF, T.TEST, ANOVA Single Factor, Conditional Formatting
