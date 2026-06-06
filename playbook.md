# The Playbook

Four phases. The calendar will vary by org size and regulatory weight; the order should not. Each phase has an exit test, and skipping a phase does not save time, it just moves the failure later.

## Phase 1: Foundation

Get the boring blockers out of the way before announcing anything.

- **Pick the tools.** A small set, chosen by people who will use them daily. One coding agent, one chat assistant, the APIs. Resist the urge to evaluate twelve vendors for six months. You can switch later; the workflows transfer.
- **Settle the data questions in writing.** What can go to the model, what cannot, where the logs live, what the vendor retains. Do this with security and legal once, publish the answer, and stop relitigating it per team.
- **Wire up access.** SSO, billing, provisioning through the normal request path. If getting an AI tool takes a ticket and two weeks, the rollout is already dead.

**Exit test:** any engineer can get the approved tools working in under an hour, and the data policy fits on one page.

## Phase 2: Ignition

Make usage visible and normal.

- **Leadership works in the open.** Directors and senior engineers do real tasks with AI in shared channels: a refactor, an incident writeup, a migration script. Not demos. Actual work, including the parts where the model is wrong and gets corrected.
- **Seed every team, not a tiger team.** One or two genuinely enthusiastic engineers per team beats a centralized AI guild. Centralized groups produce guidelines; embedded enthusiasts produce converted neighbors.
- **Run working sessions, not training.** An hour with your own backlog and someone who is two months ahead of you converts better than any course. Schedule them weekly and keep them informal.
- **Set the expectation plainly.** This is how we work now. Said by the top engineering leader, in writing, with the reasons. People can disagree with a strategy; they cannot orient to a secret.

**Exit test:** in any team channel, AI assisted work appears daily without anyone remarking on it.

## Phase 3: Integration

This is the phase that separates lasting change from a hype cycle. AI moves from something people use to something the system does.

- **Deploy pipeline:** AI review on changes before human review, summarizing risk and catching the mechanical issues so humans review judgment instead of syntax
- **Incident response:** an agent in the incident channel pulling telemetry, drafting timelines, and writing the first postmortem draft while responders respond
- **Infrastructure work:** AI drafted Terraform and Kubernetes changes as the default starting point, with humans owning intent and approval
- **Documentation:** runbooks and onboarding docs generated from the systems themselves and refreshed continuously, instead of rotting in a wiki

Each integration follows the same pattern: the AI does the first draft, the human owns the decision, and the workflow makes that ordering automatic.

**Exit test:** an engineer who personally dislikes AI tools still benefits from them daily, because they are in the pipeline, not just the editor.

## Phase 4: Compounding

- **Measure outcomes, not activity.** Deployment frequency, time to resolve incidents, onboarding time for new engineers. Usage metrics told you adoption happened; outcome metrics tell you whether it mattered.
- **Retire the scaffolding.** The working sessions and seeded enthusiasts were ignition equipment. When AI fluency becomes part of how you interview and onboard, you can stop pushing.
- **Keep raising the ceiling.** The frontier moves every quarter. Somebody senior owns watching it, and the org expects its workflows to be rebuilt around what becomes possible. The orgs that treated their first integration as the finish line are one model generation from being behind again.

**Exit test:** there is no AI initiative anymore. There is just how the org works.

## What fails

Every one of these is a postmortem I have either written or read:

- **The mandate without the workflow.** "Everyone must use AI" plus zero pipeline integration equals malicious compliance and a chatbot tab nobody looks at.
- **The pilot that never ends.** Six months of evaluation, three pilot teams, a steering committee. Meanwhile the engineers who care have personal subscriptions and your data policy is being violated daily, politely.
- **The theater metric.** Announcing a usage percentage to the board and quietly defining usage as having logged in this month. You are lying to yourself with extra steps.
- **Treating the skeptics as the problem.** Your most senior skeptic, won over by results, is worth ten enthusiasts. Give them the hardest real problem you have and the best tooling, then get out of the way.
- **Letting it be free.** Cheap tools and capped usage produce learned helplessness. If the org's experience of AI is the budget model with a rate limit, the org's conclusion will be that AI does not work.
