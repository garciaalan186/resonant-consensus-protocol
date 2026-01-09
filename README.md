# The Resonant Consensus Protocol

**A method for introducing structured uncertainty into multi-agent AI systems.**

## The Problem

Large language models face a fundamental tension: they're trained to sound confident, even when they shouldn't be. This leads to two failure modes:

1. **Hallucination**: The model generates plausible but incorrect content with unwarranted certainty.
2. **Sycophancy**: The model adapts responses to match what it thinks the user wants to hear.

Both problems share a root cause: the model lacks a principled way to represent genuine uncertainty. When multiple valid perspectives exist, or when a query is ambiguous, the model typically picks one framing and commits—leaving the user unaware they're seeing a contestable position rather than established fact.

## The Solution

The Resonant Consensus Protocol provides an external signal that's harder to game than internal confidence estimates. Rather than asking a single model "how confident are you?", the protocol:

1. Solicits evaluations from multiple agents with **adversarial perspectives**
2. Classifies artifacts based on **cross-cluster resonance**—which opposing groups endorsed them
3. Returns a structured assessment that treats **contestation as information, not failure**

The key insight: **endorsement from parties with opposing incentives is stronger evidence than endorsement from parties with aligned incentives.**

## How It Works

1. **Set up adversarial clusters.** Divide your AI agents into groups with different perspectives—for example, an "advocate" cluster (C⁺) and a "critic" cluster (C⁻).

2. **Generate responses.** Each agent answers the question from their perspective.

3. **Cross-evaluate.** Each agent votes on whether they endorse the other agents' responses.

4. **Classify by resonance pattern.** Responses fall into four tiers:

   | Tier | C⁺ | C⁻ | Contestation | Risk |
   |------|----|----|--------------|------|
   | **Positive Consensus** | ✓ | ✓ | Low | Low |
   | **Negative Consensus** | ✗ | ✗ | Low | High |
   | **Positive Polar** | ✓ | ✗ | High | Moderate |
   | **Negative Polar** | ✗ | ✓ | High | Moderate |

5. **Return multi-dimensional assessment.** The orchestrator receives not just tier classification, but contestation level, bias direction, and epistemic risk—enabling context-appropriate decisions.

## Why It Matters

When the protocol reveals disagreement, the orchestrator gains a principled basis for:

- **Surfacing uncertainty**: "These perspectives disagree on..."
- **Requesting clarification**: "Could you specify whether you mean X or Y?"
- **Presenting multiple views**: "From one perspective... from another..."
- **Acknowledging limitations**: "Both approaches have concerns about..."

This moves from **guessing the right answer** to **accurately representing the epistemic landscape**.

## Example

Imagine asking a panel about a business decision:

- The "advocate" cluster says: *"This will double revenue!"* → **Positive Polar**
- The "critic" cluster says: *"This has serious risks."* → **Negative Polar**
- Both clusters agree: *"The core technology is sound, but the timeline is aggressive."* → **Positive Consensus**
- Both clusters reject: *"We can guarantee 10x returns."* → **Negative Consensus**

A smart orchestrator leads with Positive Consensus, presents Polar views with attribution, and flags Negative Consensus as a claim that failed cross-examination.

## Learn More

See the [full paper](resonant_consensus_protocol.pdf) for the mathematical formulation, algorithm details, and implementation guidance.

## Citation

If you use this work, please cite:

```bibtex
@article{garcia2025resonant,
  title={The Resonant Consensus Protocol: Cross-Cluster Resonance Classification for Multi-Agent Systems},
  author={Garcia, Alan J.},
  year={2025}
}
```

## License

[CC BY 4.0](https://creativecommons.org/licenses/by/4.0/) — Free to use and adapt with attribution.
