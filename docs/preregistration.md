# Preregistration: Study Time and Final Grade

## Research question
Among secondary school students in Portugal, do students who
study 5+ hours per week have a higher final math grade (G3)
than students who study less than 5 hours per week?

## Population
Students in the UCI Student Performance dataset (math file),
school year 2005-2006.

## Exposure vs comparator
- Exposure: high study time (studytime = 3 or 4)
- Comparator: low study time (studytime = 1 or 2)

## Outcome
G3 (final grade, scale 0 to 20)

## Hypothesis
H1: Mean G3 of the high study group is higher than the low
study group.
H0: There is no difference.
H1 is NOT supported if the 95% confidence interval of the
difference includes 0.

## Exclusion rules
- Remove rows with missing values.
- Remove students with G3 = 0 (they did not take the exam).

## Tests
- Main test: Welch t-test
- Effect size: Cohen's d
- Backup test: Mann-Whitney U

## Robustness checks
1. Include G3 = 0 students and check if the result changes.
2. Linear regression: G3 ~ studytime group + failures + absences + school.

## Rule
No changes to this plan after looking at results.
Any change must be written as a "deviation" note.
