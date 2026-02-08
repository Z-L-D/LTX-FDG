# FDG For LTX2

Implementation of Guidance in the Frequency Domain Enables High-Fidelity Sampling at Low CFG Scales for the LTX2 model inside ComfyUI.

Thanks to the FDG researchers for making their code public.

FDG improves image quality at low guidance scales and avoids the drawbacks of high CFG scales by design.

Paper: https://arxiv.org/abs/2506.19713

# Usage

To use FDG, just place open the workflow (/workflows/LTX_FDG_v1.0.json) and copy and paste the included dense graph node into your workflow to replace your ksampler or custom sampler nodes either in your stage 1 or as you single stage sampler in your LTX2 workflow. This sampler replacement expects that you either use the distill model or the full model with the distill lora enabled to function.