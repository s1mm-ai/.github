# s1mm

Small, fast multimodal decision models.

A decision model does not write text. It takes an image, a question and a short list of options,
and returns one answer with a calibrated probability for every option, in one forward pass. Agents,
test pipelines and automation loops make thousands of these decisions a day. Today most of them go
to a large model that is slow, expensive and never says how sure it is.

s1mm builds small multimodal models for that job and, with them, the harness that proves a model
actually looks at the image rather than at the text around it. We publish every number with its
controls.

## What we are working on

- Decision models that answer typed questions over images: a choice, a yes or no, a score, each with
  a calibrated probability.
- An abstain contract, so a loop can decide what to trust and what to send back to a planner.
- Latency measured on ordinary hardware, published next to accuracy.
- An audit harness that runs the same image-use, order and calibration controls on any decision
  model that accepts images, ours included.

## Status

Early. Weights, benchmarks and the harness will be released when they pass our own gates, with the
failures reported alongside the results.

## Contact

hello@s1mm.com · [s1mm.com](https://s1mm.com)
