# Take Home Task — Damage Review Copilot

A human-controlled prototype for reviewing visible vehicle damage. The AI proposes; the claims agent decides item by item; a senior adjuster authorises.

**[Open the live prototype](https://ryhanhussain.github.io/take-home-task/)** · **[Read the two-page PRD](PRD.pdf)**

> This is a product prototype. The review workflow is functional; damage assessments, repair guidance, pricing, and source records are simulated fixtures.

## Reviewer quick start — about 3 minutes

1. Open the live prototype and select claim `CLM-2026-04182`.
2. Inspect the raw photo and pass the evidence gate.
3. Confirm, correct, or reject each proposed finding individually.
4. Compare the immutable AI proposal with the agent-reviewed subtotal.
5. Send the handoff packet to the senior adjuster.
6. In the labelled senior view, authorise the repair or return the claim with a reason.
7. Select **Reset demo** to restore the starting state.

## What the prototype demonstrates

The queue, background state changes, evidence gate, sequential review, corrections, estimate recalculation, cited source fixtures, audit history, senior handoff, and authorisation/return flow are functional.

Media checks, damage findings, repair mappings, prices, source excerpts, and assessment completion are deterministic demo fixtures. No live AI model, repair database, claims system, analytics, or backend is connected.

## Scope and limitations

The proposed V1 covers simple, visible exterior damage only. Hidden or structural damage routes to human review. Coverage, fraud, denial, payment, and automated settlement decisions are out of scope.

All seeded claims, identifiers, estimates, and source excerpts are fictional and illustrative.

Custom images are previewed locally in the browser and are not transmitted or persisted by the application. They receive the same disclosed fixture response regardless of image content. Do not use real claimant or confidential data.

## Run locally

No build step or package installation is required.

```bash
git clone https://github.com/ryhanhussain/take-home-task.git
cd take-home-task
python3 -m http.server 8000
```

Then open <http://localhost:8000>.

## Repository contents

| File | Purpose |
|---|---|
| `index.html` | Static, self-contained application code |
| `assets/sample-a-bumper.jpg` | Public-domain sample claim image |
| `PRD.pdf` | Two-page product requirements document |

The public repository intentionally contains only the submission artifacts needed to review and run the prototype.

## Image credit

[“Jetta Mk. IV Bumper Damage”](https://commons.wikimedia.org/wiki/File:Jetta_Mk._IV_Bumper_Damage.jpg) by TWikisto, released into the public domain via Wikimedia Commons.
