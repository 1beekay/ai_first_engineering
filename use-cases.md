# Where AI Lands in Platform Work

Concrete applications, ordered by how quickly they pay off. This list is platform and infrastructure flavored because that is the work I lead; most of it generalizes.

## Immediate payoff

**Incident summaries and timelines.** An agent in the incident channel that assembles the timeline from alerts, deploys, and chat as the incident unfolds. Responders respond; the paperwork writes itself. This is consistently the first place skeptics convert, because the value arrives during the worst hour of their week.

**Postmortem first drafts.** The agent drafts from the timeline, the humans add the judgment: contributing factors, what we are changing. Postmortem quality goes up and the completion rate goes to nearly 100%, because the blank page problem is gone.

**Code review preprocessing.** AI review before human review on every change: mechanical issues, missed edge cases, a plain language summary of what the change does and what it risks. Humans stop being linters and review intent instead.

**Runbook generation.** Point the model at the system, the alerts, and the last three incidents, and get a runbook draft that is current. Rotting documentation is a solved problem if you treat docs as build artifacts.

## Builds over a quarter

**Infrastructure as code drafting.** Terraform modules, Kubernetes manifests, CI pipelines: AI drafts from a description of intent, humans review and own the apply. The win is not typing speed, it is that the org's IaC patterns get applied consistently because the model is prompted with your standards.

**Deploy risk assessment.** A model that reads the diff, the blast radius, and recent incident history, and annotates every deploy with a risk summary. Pairs naturally with progressive delivery: low risk changes flow, flagged changes get eyes.

**Alert triage.** First pass classification of pages: known noisy alert, known failure mode with a runbook link, or genuinely novel. On call fatigue drops measurably when the obvious 60% arrives pre sorted.

**Cost anomaly explanation.** Not just "spend went up" but "spend went up because this autoscaling group doubled after Tuesday's deploy of this service." The investigation that took a senior engineer half a day becomes a paragraph in the morning report.

## The compounding layer

**Onboarding.** A new engineer with an agent that knows the codebase, the runbooks, and the org's decisions reaches productive faster than any buddy system I have run. Onboarding time is one of the most underrated metrics in engineering; this moves it dramatically.

**Institutional memory.** Postmortems, design docs, and decision records become a corpus the whole org can interrogate in plain language. "Have we tried this before and what happened" stops being a question only the longest tenured person can answer.

**The standards enforcer that never tires.** Every org has standards that exist in a doc and not in the code. An agent that reviews against your actual written standards closes that gap without a single architecture council meeting.

## A note on what not to automate

Keep humans owning intent, approval, and anything customer irreversible. The pattern that works is boring and consistent: AI drafts, human decides, system enforces the order. Every place I have seen that inverted, with AI deciding and humans rubber stamping, the rubber stamping degraded to not reading within a month. Design the workflow so the human's judgment is the scarce input being spent well, not a checkbox being collected.
