# Carrier-Mediated All-Optical Channel Attention for Diffractive Neural Computing

**English** | [简体中文](README.zh-CN.md)

An ongoing research project exploring input-dependent channel attention in optical neural computing. Fixed diffractive optics extract spatial feature channels, while an optical control branch adjusts their response through carrier-mediated modulation in a broad-area vertical-cavity semiconductor optical amplifier (VCSOA).

## Architecture overview

[![Carrier-mediated all-optical channel-attention pipeline](assets/optical-channel-attention-pipeline.svg)](assets/optical-channel-attention-pipeline.svg)

*Conceptual architecture. Click the vector figure to view it at full size.*

- **Feature path (blue):** The front-end diffractive network produces two-dimensional feature channels. After VCSOA modulation, a second diffractive network and detector array produce class scores.
- **Attention path (orange):** Optical squeeze and cross-channel mixing generate input-dependent control light for the VCSOA.
- **Carrier-mediated modulation (green):** Control light changes the carrier state and optical response, reweighting each feature channel while retaining its two-dimensional spatial field under the illustrated operating assumptions.

The optical masks and mixer are learned offline and remain fixed during inference; attention varies with the current optical input through the control branch.

## Project status

Research is in progress. The figure presents a proposed architecture; it does not report experimental validation or benchmark results. Further materials will accompany future research releases.

For collaboration enquiries, please contact the project maintainer.
