# The Resonant Consensus Protocol

**A method for finding genuine agreement among AI agents with different perspectives.**

## The Problem

When you ask multiple AI experts for their opinion, you get multiple answers. Some answers might be biased toward a particular viewpoint. Others might represent genuine insight that everyone can agree on. 

How do you tell the difference?

## The Solution

The Resonant Consensus Protocol solves this by checking *who* agrees with each answer, not just *how many* agree.

Here's the key insight: **an idea that's only popular with one group is probably biased, but an idea that resonates across opposing groups is probably sound.**

## How It Works

1. **Set up adversarial teams.** Divide your AI agents into groups with different perspectives—for example, an "advocate" team and a "critic" team.

2. **Generate responses.** Each agent answers the question from their perspective.

3. **Cross-evaluate.** Each agent votes on whether they endorse the other agents' responses.

4. **Classify by agreement pattern.** Responses fall into three categories:

   | Category | What it means | What to do |
   |----------|---------------|------------|
   | **Consensus** | Both teams approve | Use this—it's robust |
   | **Polar** | Only one team approves | Use with caution, note the bias |
   | **Reject** | Neither team approves | Discard it |

5. **Return to orchestrator.** The system tells you not just what was said, but how it held up to cross-examination.

## Why It Matters

Most AI systems treat all outputs equally, or just pick the most confident one. This protocol recognizes that **cross-cutting agreement is a signal of quality**—ideas that survive scrutiny from opposing viewpoints are more likely to be genuinely useful.

## Example

Imagine asking a panel about a business decision:

- The "optimist" team says: *"This will double revenue!"*
- The "skeptic" team says: *"This has serious risks."*
- Both teams agree: *"The core technology is sound, but the timeline is aggressive."*

The third response is **Consensus**—it survived cross-examination. The first two are **Polar**—valid perspectives, but biased toward one viewpoint.

A smart orchestrator leads with the consensus and presents the polar views as "on one hand... on the other hand..."

## Learn More

See the [full paper](resonant_consensus_protocol.pdf) for the mathematical formulation, algorithm details, and implementation guidance.

## Citation

If you use this work, please cite:

```bibtex
@article{garcia2025resonant,
  title={The Resonant Consensus Protocol: Cross-Cluster Agreement Classification for Multi-Agent Systems},
  author={Garcia, Alan J.},
  year={2025}
}
```

## License

[CC BY 4.0](https://creativecommons.org/licenses/by/4.0/) — Free to use and adapt with attribution.
