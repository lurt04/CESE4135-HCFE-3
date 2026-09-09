# Literature Survey — Problem Scoping

Date: 2026-09-09
Status: draft, sub-problem not yet chosen (team decision pending)

## Purpose

Support convergence on a specific sub-problem within "home care for the elderly"
(CLAUDE.md). Four candidate risk areas were researched for evidence that they
are (a) real drivers of nursing home admission and (b) tractable for a team
with CS, embedded systems, computer engineering, mechanical engineering, and
electrical engineering backgrounds, budget 5000 EUR/person.

## Candidate areas

### 1. Falls & mobility

- ~1/3 of home-dwelling adults 65+ fall at least once a year; ~1/2 of those 80+.
- ~1 in 10 falls results in a serious injury.
- Falls are the primary reason for **40%** of nursing home admissions.
- ~20% of frail home-dwelling older adults in Dutch primary care are at risk
  of a fall incident (more often men).
- NL lifetime risk of nursing home admission after age 65: 24.5% (±1.5%);
  after age 80: 31.0% (±1.5%).
- 2015 Dutch LTC reform (aging-in-place policy) reduced adjusted NH admission
  rate from 88.80 to 69.82 per 100,000 older adults.

Sources:
- [Safety risks among frail older people living at home in the Netherlands](https://pmc.ncbi.nlm.nih.gov/articles/PMC9292903/)
- [Predicting falls in elderly receiving home care](https://pmc.ncbi.nlm.nih.gov/articles/PMC12878167/)
- [The effect of frailty on residential/nursing home admission in the Netherlands](https://link.springer.com/article/10.1007/s10433-005-0011-z)
- [Utilisation of nursing home care before/after the 2015 Dutch reform](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC11791781/)

### 2. Medication management

- Pill-count adherence in Dutch home care nursing patients: 88.3%
  (self-report: 94.6%); mean possession ratio for chronic polypharmacy: 82.9%.
- Among hospitalized elderly on home nursing after discharge: 30.6%
  under-adherent (<70%), 18.4% over-adherent.
- **Up to 23%** of nursing home admissions may be due to inability to
  self-manage prescription medications at home.
- Non-adherence linked to 33–69% of hospital admissions and ~125,000 deaths/yr
  (broader, non-NL-specific figure).
- Main non-adherence drivers: forgetting, regimen complexity, poor cognition,
  higher drug count, depression.

Sources:
- [Medication Status and Adherence of the Elderly under Home Care Nursing](https://www.rcphn.org/journal/view.php?id=10.12799/jkachn.2011.22.3.290)
- [Multiple Medication Adherence in Community-Dwelling Older People on Chronic Polypharmacy](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC9099923/)
- [Medication adherence in elderly patients receiving home health services after discharge](https://pubmed.ncbi.nlm.nih.gov/11346058/)
- [Promoting Medication Adherence in the Elderly](https://onlinelibrary.wiley.com/doi/full/10.1002/agm2.70053)

### 3. Cognitive decline / dementia

- Dementia is one of the strongest single predictors of nursing home
  admission; NL admissions for dementia are typically moderate/severe stage.
- Median time from dementia diagnosis to NH admission (NL): 3.9 years.
- 2015 Dutch LTC reform was negatively associated with NH admission rates
  among 270,706 older adults with dementia — fewer admissions, longer
  waiting lists.
- No NL-specific "% of admissions caused by dementia" figure found in this
  pass — flagged as a gap if this area is chosen.

Sources:
- [Impact of the 2015 Dutch LTC Reform on Nursing Home Use for People With Dementia](https://pmc.ncbi.nlm.nih.gov/articles/PMC12968352/)
- [Time from dementia diagnosis to nursing-home admission and death](https://journals.plos.org/plosone/article?id=10.1371%2Fjournal.pone.0243513)
- [Costs of Persons with Dementia Living in Nursing Homes in the Netherlands](https://pmc.ncbi.nlm.nih.gov/articles/PMC9535598/)

### 4. Social isolation / loneliness

- Pre-pandemic: 31.2% of Dutch adults 45+ felt (somewhat) lonely.
- Living alone, low neighbour contact, perceived exclusion, and psychological
  distress consistently associated with loneliness.
- Loneliness linked to diabetes, cardiovascular disease, sleep disorders,
  Alzheimer's disease; mortality risk comparable to obesity/substance abuse.
- Loneliness correlates with more GP visits and higher healthcare use.
- No direct "% of NH admissions caused by isolation" figure found — isolation
  appears more as a health-outcome amplifier than a direct admission trigger.

Sources:
- [Age differences in factors associated with loneliness in the Netherlands](https://pmc.ncbi.nlm.nih.gov/articles/PMC7409622/)
- [Cumulative Effect of Loneliness and Social Isolation on Health Outcomes](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC8681973/)
- [Loneliness and Mental Health During COVID-19: Dutch Older Adults](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC7454922/)

## Comparison

| Area | Direct link to NH admission | Team skill fit (CS/embedded/mech/EE) |
|---|---|---|
| Falls & mobility | Strong — 40% of admissions | High — sensors, wearables, mobility aids |
| Medication management | Strong — up to 23% of admissions | High — smart dispensers, reminders |
| Cognitive decline | Strong predictor, no NL % found | Medium — safety tech only, can't treat cause |
| Social isolation | Indirect (health amplifier) | Low — mostly a social, not technical, fix |

## Recommendation

Falls & mobility: strongest quantified causal link to nursing home admission
and clearest fit for the team's engineering mix. Medication management is a
close second. Final choice pending team discussion.

## Open gaps for next pass

- NL-specific % of admissions attributable to dementia.
- Cost/complexity estimate per candidate against the 5000 EUR/person budget.
- Existing product landscape (competition/novelty check) per candidate.
