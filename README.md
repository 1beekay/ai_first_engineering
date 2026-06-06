# AI First Engineering

How to take an engineering organization from scattered AI experimentation to AI as the default way work gets done. I led this shift at a company of roughly 100 engineers, taking daily AI usage from about 30% of people to effectively 100%, across engineering and the business teams around it. This repo is the genericized playbook: what worked, what order to do it in, and what fails.

The core claim: AI adoption is not a tooling problem. Every failed AI initiative I have seen bought the tools first and assumed behavior would follow. It does not. AI adoption is a change to how work flows through your organization, and it has to be led the way any operating change is led.

## What is in this repo

| File | Contents |
|---|---|
| [playbook.md](playbook.md) | The rollout, phase by phase |
| [use-cases.md](use-cases.md) | Where AI actually lands in platform and infrastructure work |

## The principles

**Leaders go first, visibly.** The single highest leverage act in the whole rollout: engineering leadership doing real work with AI in front of people. Demos from the platform team read as marketing. A director debugging a production issue with an AI agent in a shared channel reads as permission.

**Default on, not opt in.** As long as AI usage is a personal choice, you get the same 30% of natural enthusiasts forever. The shift happens when AI is wired into the workflows everyone already lives in: the deploy pipeline, the incident channel, code review, documentation. People should have to opt out, not in.

**Pay for the good tools and stop counting seats.** Seat anxiety kills adoption. The cost of frontier AI tooling for an entire engineering org is roughly the cost of one engineer, and a fraction of the productivity it returns. Decide once, at the top, and remove the per seat conversation entirely.

**Measure usage honestly, not performatively.** Track real signals: agent sessions per engineer, AI involvement in merged changes, time to resolve incidents with and without AI assistance. Do not build a leaderboard. The point of measurement is to find where adoption is stuck, not to shame people.

**Quality bars do not move.** AI written code goes through the same review, testing, and deployment gates as human written code. Saying this loudly and early disarms the most common objection before it organizes.

**Expect and absorb the dip.** Weeks two through six look worse before they look better, while people learn what the tools are good for. Leaders who lose their nerve in the dip and let the initiative quietly die have run the most expensive pilot in company history.

## Why platform teams should own this

AI transformation initiatives die in two places: legal review and infrastructure friction. A platform organization is positioned to kill both. It already owns the deployment pipeline, the incident tooling, the developer experience, and the security posture. That means it can wire AI into the paths everyone uses and make the secure way the easy way. If your AI initiative lives in a slide deck instead of the deploy pipeline, it is not an initiative yet.
