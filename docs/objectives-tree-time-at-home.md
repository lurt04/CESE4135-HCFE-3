# Objectives Subtree — "Keep them home for longer"

Date: 2026-09-10
Owner: Vladimir
Scope: one requirement out of four (ease of use, minimize cost, minimize
maintenance, **keep them home for longer**) for the sub-problem "unintrusively
assist elderly with mild cognitive decline in staying home longer."
Primary case: living alone. Cost/maintenance/ease-of-use trade-offs are owned
by other requirements and intentionally not scored here.

## Objective tree

**Top objective: Maximize years living independently at home**

1. **Prevent safety incidents that force admission**
   1.1 Prevent falls
   1.2 Prevent medication errors
   1.3 Prevent home accidents (fire, water, gas, unattended exits)
2. **Slow functional & cognitive decline**
   2.1 Maintain daily structure/routine
   2.2 Provide cognitive stimulation
   2.3 Maintain physical activity
3. **Sustain caregiver/family capacity**
   3.1 Reduce caregiver burden/fatigue
   3.2 Protect caregiver sleep and wellbeing
   3.3 Give caregivers visibility without requiring presence
4. **Enable timely intervention**
   4.1 Detect deterioration early
   4.2 Alert the right person fast enough to treat at home instead of escalating to hospital/admission

Each branch below has: why it matters (evidence), and candidate subproblems/
solutions — including your dispenser/faucet ideas, expanded with what the
literature and nursing-home practice suggest.

## 1. Prevent safety incidents

Why: falls are the primary reason for 40% of nursing home admissions
(general elderly); adults with MCI fall at **>60%/year — 2-3x the rate** of
cognitively healthy peers, and living alone or in low-income/socially
vulnerable settings is itself a top risk factor. Up to 23% of admissions are
linked to inability to self-manage medication.

Candidate subproblems:
- **Passive fall-risk monitoring**: in-home passive sensors (e.g. depth
  sensors) + ML to flag rising fall risk before a fall happens, paired with
  a coach/caregiver alert — unintrusive (no wearable required). Evidence:
  feasibility study (Sense4Safety) showed sensor-based risk score correlated
  r=0.94 with a standard physical-performance test and produced timely
  alerts. Caveat: overall evidence that tech *reduces* falls in dementia/MCI
  is still rated "limited, inconclusive" — good for detection, not proven
  yet for prevention.
- **Smart medication dispenser** (your idea): automatic pill dispenser with
  reminders/alarms, app connectivity for remote caregiver monitoring of
  missed doses. Well-established product category; main open question is
  ease-of-use/UI for MCI users (owned by the "ease of use" requirement).
- **Auto-shutoff appliances** (your faucet idea, also seen for stoves):
  motion/presence-based auto shutoff after a timeout, caregiver lock mode,
  mobile alert on trigger. Commercial precedent: stove auto-shutoff devices
  with 5-minute no-presence timeout.
- **Unattended-exit (wandering) detection**: door/exit sensors that alert a
  caregiver if the person leaves during unusual hours — flagged in smart-home
  dementia reviews as one of the outcomes technology can plausibly affect.

## 2. Slow functional & cognitive decline

Why: multi-domain, non-pharmacological home interventions (diet, physical
activity, stress reduction, cognitive stimulation) show measurable benefit to
memory, verbal fluency, executive function, and global cognition — more so
than single-domain interventions (meta-analysis, 28 studies, 2711
participants). Nursing homes lean heavily on **structured daily routine**
tied to the resident's pre-existing habits to reduce anxiety/confusion
(including "sundowning") and preserve independence in tasks like dressing or
light chores.

Candidate subproblems:
- **Routine/structure assistant**: gentle, personalized prompts for
  waking/meals/activity/rest timed to the person's own historical habits
  (not a generic schedule) — directly mirrors nursing-home practice, and is
  inherently unintrusive if framed as a reminder rather than a command.
- **Home-based cognitive stimulation companion**: lightweight
  puzzles/reminiscence/conversation prompts, deliverable via a simple device;
  literature shows caregiver-delivered home cognitive stimulation is feasible
  and meaningful, so a device that scaffolds this (rather than replacing
  the caregiver) fits the evidence.
- **Nudges for physical activity**, tied into the same routine assistant.

## 3. Sustain caregiver/family capacity

Why: this is the branch most teams miss. Caregiver **burden, emotional
fatigue, and perceived entrapment predict nursing home entry at least as
strongly as the patient's own functional/cognitive decline**. In other
words, the system may need to serve the family as much as the elderly
person — directly answers your question about living-with-family cases:
even where relatives are present, reducing their burden extends time at
home.

Candidate subproblems:
- **Remote reassurance dashboard**: lets a family caregiver check in without
  being physically present (medication taken? routine followed? any alerts
  today?) — reduces need for constant in-person supervision.
- **Sleep-protecting night monitoring**: an RCT of an in-home monitoring/
  alerting system (People Power Caregiver, 162 caregivers, 6 months) found
  it protected caregiver sleep efficiency — a system that only alerts on
  real anomalies (unintrusive) rather than constant checking directly
  targets this.
- Validated screening exists (NHA-Burden / NHA-Depression tools, ~75-77%
  sensitivity) for *identifying* at-risk caregivers — useful for later
  validating whether our system is actually working.

## 4. Enable timely intervention

Why: catching deterioration early can mean home treatment instead of a
hospital admission that cascades into a nursing-home placement. A pilot
program (SMART4MD) specifically targets MCI patients with a monitoring +
reminder platform for both patient and informal carer. A broader scoping
review (5 systems, 617 community-dwelling people with dementia) found
plausible effects on falls risk, agitation, sleep, cognitive functioning,
and unattended exits — but flagged **low methodological quality across the
field**, so treat specific effect sizes cautiously; the direction of
evidence is positive, the rigor isn't there yet.

Candidate subproblems:
- **Deterioration trend detection**: combine routine-adherence, activity,
  and sleep signals already collected by branches 1-3 into a single trend
  alert, rather than a new sensor — reuse over redundancy.
- **Escalation-appropriate alerting**: make sure alerts reach the right
  person (family vs. GP vs. emergency) at the right threshold — avoids
  both under-reaction and alert fatigue.

## Cross-cutting notes

- Several "candidate subproblems" above are really one shared platform
  (routine engine + sensor/alert layer + caregiver dashboard) feeding all
  four branches — worth flagging to the team before the group locks
  individual ownership of solutions.
- Evidence quality caveat to carry into the report: most cited studies are
  feasibility/pilot-stage, not large trials proving reduced nursing-home
  admission. Frame claims as "plausible, evidence-backed direction," not
  "proven to keep people home longer."

## Sources

- [Feasibility/Acceptability of Tech-Mediated Fall Risk Prevention for MCI (Sense4Safety)](https://pmc.ncbi.nlm.nih.gov/articles/PMC12340378/)
- [Digital technologies to prevent falls in dementia/MCI — systematic overview](https://pmc.ncbi.nlm.nih.gov/articles/PMC10788098/)
- [A technology supported fall prevention intervention for MCI](https://pmc.ncbi.nlm.nih.gov/articles/PMC10738719/)
- [Effect of home-based lifestyle interventions on cognition in MCI — systematic review](https://pmc.ncbi.nlm.nih.gov/articles/PMC10900825/)
- [Home-based individual cognitive stimulation RCT](https://www.frontiersin.org/journals/psychology/articles/10.3389/fpsyg.2021.741955/full)
- [Routine in Dementia Care: A Path to Emotional Well-Being](https://www.maplewoodseniorliving.com/blog/routine-in-dementia-care-a-path-to-emotional-well-being/)
- [Dementia Care Plan: Guide for Caregivers (NCCDP)](https://www.nccdp.org/dementia-care-plan-guide-for-caregivers/)
- [Predictors of change in caregiver burden following nursing home admission](https://pubmed.ncbi.nlm.nih.gov/19485656/)
- [Clinically significant changes in burden and depression among dementia caregivers post-admission](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC3012012/)
- [Identifying at-risk dementia caregivers — NHA-Burden/NHA-Depression tools](https://pubmed.ncbi.nlm.nih.gov/24965720/)
- [In-home assistive technology protects dementia caregivers' sleep efficiency (RCT)](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC11692845/)
- [Effectiveness of smart home technologies for community-dwelling people with dementia — scoping review](https://www.sciencedirect.com/science/article/abs/pii/S1386505621001398)
- [SMART4MD pilot RCT protocol (mild dementia/MCI monitoring + reminders)](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC6611150/)
- [Assistive technology for persons with dementia & caregivers — device overview incl. stove auto-shutoff](https://www.dementiacarecentral.com/caregiverinfo/other-assistive-technology/)

Also carried over from the earlier scoping survey (see
[literature-survey.md](literature-survey.md)): falls = 40% of NH admissions,
medication self-management issues = up to 23%.
