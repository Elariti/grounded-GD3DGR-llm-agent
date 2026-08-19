# Grounded 3D Gaussian Splatting LLM Agent

A tool-using LLM agent for grounded analysis of a 3D Gaussian Splatting
LEGO scene using persistent `grain_id` identities.

## Features

- Persistent grain spatial queries
- 3DGS opacity/scale decoding
- Geometry-based region hypotheses
- Persistent-ID temporal comparison
- Synthetic damage validation
- ΔH surface-change analysis
- Evidence-grounded LLM responses
- Explicit refusal and provider-error handling

## Results

- 194,018 Gaussians in the baseline PLY
- 35,731 persistent grain IDs
- 11,090 Gaussians removed in the controlled synthetic-damage scan
- 2,117 missing persistent grain IDs detected
- 160 partially reduced grains detected
- 2 damage zones identified
- 122 flagged ΔH cells

## Requirements

- Python 3.x
- Jupyter / Google Colab
- Groq API key
- Required Python packages listed in the notebook

## Dataset

The source PLY is not included in this repository.
Place the supplied PLY at the path configured in the notebook.

## Notes

Semantic region labels are not present in the supplied PLY.
Detected regions are therefore geometric hypotheses, not ground-truth
semantic labels.

Synthetic damage is controlled validation data and should not be
interpreted as real-world damage ground truth.

Live LLM evaluation may be affected by provider availability or
rate limits.

## Results

- 194,018 Gaussians in the baseline PLY
- 35,731 persistent grain IDs
- 11,090 Gaussians removed in the controlled synthetic-damage scan
- 2,117 missing persistent grain IDs detected
- 160 partially reduced grains detected
- 2 damage zones identified
- 122 flagged ΔH cells
