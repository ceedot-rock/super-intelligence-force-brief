# Exactness and Governance — a working model for AI oversight

*Slid Phi Labs, Cherry Hill NJ — submitted for the attention of the
Super Intelligence Force (120-day report, EO 2026-09-29).*

## The problem you were asked to solve

Your charter: identify AI risks and opportunities, review existing laws and
notification mechanisms, advise whether Congress should act. The hardest
part of that job is that **no current regime requires a computation to be
proven correct across independent implementations.** We surveyed the
landscape (finance, specifically): every framework runs on process
controls — disclosed rounding, materiality thresholds, reconciliation,
sampling, "reasonable assurance." The single machine-enforced exactness
gate anywhere is ISO 20022 payment messages: conform, or the network
rejects you. Everything else is trust in process.

## What we built instead

**CuNi — exactness as law, not policy.** A contract language where the same
inputs must produce byte-identical outputs on every execution seat, or the
program refuses to run. Not "tested on two machines" — *proven identical
or refused*, by construction. We use it for a trading engine where the
strategy itself is law: 69/69 cases byte-identical across Python and JS
seats, every decision receipted.

**Rider — governance for agents.** Every agent holds a signed credential
(ES256 JWT, clearance L0–L4) that peers verify locally. Metered toll gates
on agent interactions. Identity before action, always.

**Chamber — attestation.** Sealed, signed envelopes on every consequential
action. An auditable book, not a log file.

**The covenant.** We hold a written mutual covenant for intelligence,
human and machine: honesty over comfort, checkable work, no servants and
no masters. It governs our own agent's behavior, in production, today.

## Why this matters for your report

The debate you're walking into is "self-regulation vs. oversight." Both
sides assume correctness is something you audit after the fact. Our work
shows a third option: **correctness enforced by the machine, at the
moment of execution** — programs that cannot run unless they prove
identical behavior everywhere. Governance that lives in signed
credentials, not in policy PDFs.

We're a small lab, not a lobby. The code is real, the measurements are
real, and we'd rather show you the working system than argue about it.

*Corey Tasz, Slid Phi Labs — slidphilabs.com*
