# Predicting Answer Features Before the Model Speaks

## Hypothesis

Train maps from context activations to upcoming answer-feature probes.

## Approach

Local open-weight pilot with a measured path when weights are available and an
explicit synthetic smoke path. Claims are gated when measurements are proxy-grade.

## Primary metrics

- Pilot metric with confidence interval
- `claim_ok` / honesty stamps
- Synthetic contamination rate
