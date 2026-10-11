# s1mm

Small, fast multimodal decision models.

A decision model does not write text. It takes a screenshot, a question and a short list of options,
and returns one answer with a calibrated probability for every option, in one forward pass. Agents,
test pipelines and automation loops make thousands of these decisions: is the field filled, which
element is the target, did the page change, is a dialog in the way. Today most of them go to a large
model that is slow, expensive and never says how sure it is.

s1mm builds small multimodal models for that job and, with it, the harness that proves a model actually
looks at the image rather than at the text around it. We start with screens, where a small model can beat
large ones today, and we publish every number with its controls.

## What we are working on

- A sub-250M-parameter decision model for GUI state, element choice and step verification, trained on
  public and programmatically labelled screen data.
- Calibrated probabilities with an abstain contract, so a loop can decide what to trust and what to
  send back to a planner.
- Latency measured on ordinary hardware, published next to accuracy.
- An audit harness that runs the same image-use, order and calibration controls on any decision model
  that accepts images, ours included.

## Status

Early. Weights, benchmarks and the harness will be released when they pass our own gates, with the
failures reported alongside the results.

## Contact

hello@s1mm.com · [s1mm.com](https://s1mm.com)
