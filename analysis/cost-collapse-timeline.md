---
layout: default
---

# Cost Collapse Timeline: When AI Makes Floor-Raising Economically Inevitable

## Summary

AI inference costs are dropping at approximately 10x per year, and faster since early 2024. Services built on this infrastructure — diagnosis, education, legal assistance, administration — inherit the decline. This analysis traces the historical pattern (cost collapse drives universal provision), documents the current trajectories, examines four domains where the floor is actively falling, and estimates when the economic logic inverts: when providing baseline services universally becomes cheaper than managing the consequences of withholding them. The cost curves are well-evidenced. The institutional adoption timelines are genuinely uncertain.

---

## Historical Pattern: Cost Collapse Drives Universality

Every foundational service now considered a basic right followed the same arc: expensive novelty, declining cost, universal provision. The transition was never smooth and was always resisted by incumbents. It happened anyway because the economics eventually became undeniable.

### Electricity

In the 1920s, most American cities were electrified, but fewer than 10% of farm households had electricity. Private utilities refused to extend lines to rural areas — the per-capita infrastructure cost was too high relative to expected revenue. By 1936, the Rural Electrification Administration began extending credit for connections and appliances, guaranteeing demand that made economies of scale viable. Within 30 years, rural electrification was nearly universal. The economic returns exceeded costs even in the lowest-density areas. Counties that gained early access experienced economic growth that persisted for decades after the rest of the country caught up.

The pattern: production costs fell to the point where exclusion became more expensive than provision — not because anyone's moral argument won, but because the math changed.

### Clean Water

Municipal water treatment followed the same curve. Cholera and typhoid epidemics in the 19th century killed across class lines, creating an economic case for universal provision that pure altruism could not. The cost of filtration and chlorination dropped steadily through the early 20th century. Cities that invested in universal clean water saw mortality declines of 30-40% and productivity gains that vastly exceeded infrastructure costs. The argument stopped being "should we provide clean water to the poor" and became "we cannot afford not to."

### Telecommunications

AT&T's universal service mandate (codified in the Communications Act of 1934) emerged after decades in which telephone access was a luxury. Cross-subsidization — urban customers effectively subsidized rural lines — made universal provision cheaper than maintaining two tiers of economic participation. The cost of a phone call dropped by orders of magnitude over the 20th century. By the time it was cheap, exclusion was already economically indefensible.

### Internet Access

The pattern is repeating now. The FCC's broadband subsidies, municipal broadband initiatives, and Starlink's satellite coverage are all responses to the same dynamic: internet access became so foundational to economic participation that exclusion costs more than provision. The E-Rate program (1996) subsidized school and library internet because the alternative — a generation without digital literacy — was economically catastrophic.

### The Common Thread

In every case:
1. The technology starts expensive and exclusive.
2. Production costs fall through scale and innovation.
3. The cost of exclusion becomes visible (disease, lost productivity, economic isolation).
4. Universal provision becomes the cheaper option.
5. Incumbents resist until the accounting is undeniable, then claim credit.

The transition typically takes 20-40 years from cost viability to near-universal provision. The question for AI-driven services is whether this timeline compresses, and by how much.

---

## Current AI Cost Trajectories

The data here is unusually clean. API pricing is public, versioned, and timestamped. The trends are not projections from thin data — they are observed prices from the largest providers over a four-year period.

### The Core Numbers

**GPT-3.5-equivalent performance:**
- November 2022: ~$20 per million tokens
- October 2024: ~$0.07 per million tokens
- Reduction: **280x in 24 months**

**GPT-4-equivalent performance:**
- March 2023: ~$60 per million tokens (input)
- Early 2026: ~$0.40 per million tokens
- Reduction: **~150x in 36 months**

**Aggregate trend (Epoch AI analysis):** For models of equivalent capability, inference cost is declining at approximately **10x per year** as a median rate. Post-January 2024, when competition and architectural innovation accelerated, the median rate increased to **~200x per year** for the fastest-moving capability tiers.

### What Is Driving This

The decline is not from a single source. It is the compounding of multiple independent drivers:

- **Algorithmic efficiency:** Mixture-of-experts architectures, quantization, speculative decoding, and distillation reduce compute per token at equivalent quality.
- **Hardware competition:** Nvidia H100 cloud pricing fell 64-75% from Q4 2024 ($8-10/hour) to Q1 2026 ($2.99/hour). TPUs and specialized ASICs are projected to capture 70-75% of production inference workloads by 2028, further driving prices down.
- **Open-source pressure:** Open-weight models (Llama, Mistral, Qwen, DeepSeek) create a price floor competitors must beat or match, compressing margins at every tier.
- **Scale effects:** As deployment volume increases, fixed costs amortize across more queries, dropping per-unit costs further.

### The Jevons Paradox Note

Despite per-token costs dropping ~1000x since 2022, total spending on foundation model APIs reached $18 billion in 2025. Cheaper intelligence generates more demand for intelligence. This is the Jevons paradox — the same dynamic that made electricity usage increase as it got cheaper. It is not evidence against cost collapse. It is evidence that the services being built on cheap inference are proliferating, which is exactly the mechanism by which cost collapse reaches end users.

---

## Domain Analysis

### Medical Diagnosis and Triage

**Current state (well-evidenced):**
- Nearly 400 FDA-approved AI algorithms exist for radiology alone.
- In breast cancer detection, AI sensitivity reaches 0.85 vs. 0.77 for physicians in controlled studies.
- AI triage can double detection of malignant nodules when combined with a human reader.
- In dermatology, AI algorithms demonstrate comparable or superior performance to dermatologists in diagnosing skin lesions, including melanoma. Accuracy ranges from 47.6% to 87.5% depending on context, with no compromise in specificity.
- The EU AI Act (effective January 2026) classifies medical AI as high-risk, requiring rigorous evaluation of accuracy, explainability, and bias.

**Cost implications:**
- Average ER visit: $1,389. Average primary care visit: $167. AI triage consultation: approaching $0 at the marginal cost level.
- An estimated $8.3 billion is spent annually in the US on emergency department care that could be provided in lower-cost settings. AI triage and remote diagnostic tools directly address this by enabling earlier, cheaper intervention.
- 28% of US adults delayed or skipped care due to cost in 2023. 26% expect to defer procedures in 2025. AI diagnostics do not replace treatment, but they can replace the most expensive step in the diagnostic pipeline — the specialist consultation — and route patients to appropriate care earlier and cheaper.

**What remains uncertain:**
- Regulatory approval timelines for autonomous (non-physician-supervised) AI diagnosis vary dramatically by jurisdiction.
- Liability frameworks for AI-assisted medical decisions are unresolved in most countries.
- A prospective clinical trial found that when AI tools were removed after six months of use, human detection rates dropped below pre-AI baselines — suggesting dependency risks that regulators will need to address.
- AI matching specialist accuracy on average does not mean matching the best specialists, and does not mean performing well on rare or atypical presentations. The long tail matters in medicine.

**Floor-raising potential:** High. The people most harmed by diagnostic access barriers — uninsured, rural, low-income — are precisely the population where AI diagnostics provide the largest marginal improvement. The gap between "no diagnosis" and "AI-quality diagnosis" is larger than the gap between "AI-quality diagnosis" and "top specialist."

### Education

**Current state (well-evidenced):**
- A 2025 randomized controlled trial (published in *Scientific Reports*) found AI tutoring outperformed in-class active learning with an effect size of 0.73-1.3 standard deviations. Students using AI completed equivalent learning in 49 minutes vs. 60 minutes for classroom instruction.
- Students using supervised AI tutors solved new problems successfully 66.2% of the time, compared to 60.7% with human tutors alone.
- The Coursera AI in Higher Education Report (February 2026) found 80% of students report AI improved their academic performance.
- A systematic review of intelligent tutoring systems in K-12 found generally positive effects on learning and performance, though effects are moderated when compared against other (non-AI) tutoring systems specifically.

**Cost implications:**
- Human tutoring costs $40-100/hour in most US markets. AI tutoring at current inference prices costs fractions of a cent per interaction.
- The relevant comparison is not "AI tutor vs. human tutor" but "AI tutor vs. nothing" — because the students at the lowest educational floor do not have access to human tutors at all.
- Bloom's famous 2-sigma finding (1984) showed that one-on-one tutoring produced a two standard deviation improvement over classroom instruction. AI tutoring is approaching this threshold at near-zero marginal cost. If it reaches it, the most effective known educational intervention becomes universally available.

**What remains uncertain:**
- Long-term outcomes. The studies are measuring near-term learning gains, not lifetime educational trajectories.
- Motivation and engagement. AI tutors can teach content effectively, but the relational dimension of education — a human who cares whether you show up — is not replicated and may matter more than content delivery for at-risk students.
- The digital divide. AI tutoring requires devices and connectivity. The students who need it most are the students least likely to have reliable access.

**Floor-raising potential:** Very high, with caveats. For content knowledge and skill building, AI tutoring is already floor-raising at scale. For the social and motivational dimensions of education, it is a complement, not a replacement.

### Legal Assistance

**Current state (moderately evidenced):**
- AI legal tools can reduce entity creation time from 45 minutes to under 10 minutes. Paralegals report saving 5+ hours per claim on specific case types.
- Document review, the most labor-intensive phase of litigation, is increasingly automatable — though the actual reduction in billable hours has been modest so far (13% among firms reporting positive results).
- The legal AI market reached $1.2 billion in 2025 and is growing rapidly.

**The justice gap (well-evidenced):**
- Low-income Americans receive no or insufficient legal help for **92% of their substantial civil legal problems** (Legal Services Corporation).
- Californians seek legal help for just 18% of their legal problems overall, and 29% of problems that substantially impact their lives (2024 California Justice Gap Study).
- The World Justice Project's 2024 Rule of Law Index ranks the US **107th out of 142 countries** on accessibility and affordability of civil justice — a drop of 42 spots from 2015.
- Of business owners with unmet legal needs, 85% reported significant financial consequences.

**Cost implications:**
- The justice gap is not primarily a knowledge gap — it is a cost gap. Legal information exists. The barrier is that navigating it requires professional assistance that costs $200-500/hour.
- AI can provide basic legal guidance, benefits navigation, form completion, and document preparation at marginal costs approaching zero. This does not replace courtroom representation, but the vast majority of unmet legal needs never reach a courtroom. They are administrative: understanding rights, completing forms, navigating eligibility, responding to notices.

**What remains uncertain:**
- Unauthorized practice of law (UPL) regulations in most US states prohibit non-lawyers from providing legal advice. Whether AI-generated guidance constitutes "practice of law" is being actively litigated and varies by jurisdiction.
- Quality floor. Bad legal advice is worse than no legal advice. AI legal tools need to be reliable enough that errors do not create new harm. Hallucination rates in legal applications are a genuine concern.
- The Bloomberg Law finding that AI has done "little to reduce law firm billable hours" is important context — cost collapse at the production level is not yet translating to cost collapse at the consumer level. Firms are capturing the efficiency gains as margin, not passing them through.

**Floor-raising potential:** High in the long run, moderate in the near term. The 92% unmet legal needs figure represents an enormous gap that AI can partially address even with current capabilities. The regulatory and liability obstacles are real but are also self-evidently absurd when the alternative is 92% of legal needs going completely unmet.

### Administrative Overhead

**Current state (moderately evidenced):**
- Government agencies are beginning to use AI for eligibility determination, claims processing, and benefits administration. Virginia established an AI Innovation Fund; Arkansas launched a statewide pilot for public benefits administration.
- Oracle Intelligent Advisor and similar tools automate policy rules into decision models for benefits eligibility and entitlement calculation.
- The federal government has identified 94 AI-related government-wide requirements as of 2025.
- New York's LOADinG Act forbids new automated decision-making in public assistance programs — illustrating that the regulatory landscape is actively contested.

**Cost implications:**
- Administrative overhead is a significant fraction of total program cost for many social services. Eligibility determination, case management, documentation, and compliance reporting consume resources that could otherwise be directed to service delivery.
- The irony of means-testing: in many programs, the cost of determining whether someone qualifies for assistance approaches or exceeds the cost of simply providing the assistance. This is well-documented for programs like SNAP and Medicaid, where administrative costs per participant are substantial relative to benefit amounts.
- AI can reduce these costs dramatically — not by replacing human judgment on complex cases, but by handling the routine processing that constitutes the majority of volume.

**What remains uncertain:**
- Bias and fairness. Automated eligibility systems have a documented history of producing discriminatory outcomes (e.g., Michigan's unemployment fraud detection system, Indiana's automated welfare eligibility). AI systems trained on historical data can replicate and amplify these biases.
- Accountability. When an AI system denies benefits, the appeals process must remain accessible and human. Automating the front end while maintaining human oversight on exceptions is the right architecture, but it is harder to implement than full automation.
- Political will. Ten states have introduced bills requiring AI impact assessments for government decision-making. The regulatory landscape is forming in real time and could either accelerate or stall adoption.

**Floor-raising potential:** Moderate to high. Administrative automation is less glamorous than AI diagnosis or tutoring, but it may have a larger near-term impact on floors simply because so much current spending goes to managing the system rather than helping people. Reducing administrative friction is a direct floor raise.

---

## The Inversion Point

The inversion point is when providing a service universally becomes cheaper than managing the consequences of not providing it. This is not a single moment — it arrives at different times for different services in different contexts.

### The Math of Withholding

The cost of not providing basic services is already well-documented:

- **Healthcare:** $8.3 billion annually in preventable ER visits. $74 billion borrowed annually for medical expenses. Average ER visit ($1,389) vs. average primary care visit ($167) — an 8x multiplier that the uninsured pay because they lack the cheaper option.
- **Legal:** 92% of low-income legal needs unmet. 85% of affected business owners report significant financial consequences. The downstream costs — evictions that lead to homelessness, benefits denials that lead to ER visits, wage theft that goes unremedied — cascade across every public budget.
- **Education:** The lifetime earnings gap between a high school graduate and a dropout is approximately $400,000. The cost of remedial education, criminal justice involvement, and social services for under-educated populations dwarfs the cost of providing quality education.
- **Administration:** Every dollar spent determining whether someone qualifies for a $50/month benefit is a dollar not spent on the benefit itself. When administrative costs exceed 15-20% of program budgets, the system is spending more on gatekeeping than it saves by excluding the ineligible.

### When Does the Math Flip?

The inversion happens when:

**Cost of universal AI-assisted provision < Cost of managing consequences of non-provision**

For triage and basic diagnostics, we may already be past this point. An AI triage system that routes 10% of ER visits to appropriate lower-cost settings saves more than it costs to operate, even at current prices. The barrier is not cost but regulatory approval and institutional adoption.

For education, the math is favorable now for supplementary tutoring. Providing AI tutoring access to every student costs less per year than remediating a single student who falls behind. The barrier is infrastructure (devices, connectivity) and institutional willingness.

For legal guidance, the inversion point is near for administrative legal tasks (form completion, benefits navigation, rights information) but further away for complex legal representation. The 92% gap is so large that even partial AI coverage shifts the economics.

For administrative overhead, the inversion has arguably already occurred in principle — we spend more on means-testing some programs than universal provision would cost. AI automation accelerates this by making the contrast more visible and more extreme.

### Why the Inversion Is Not Sufficient

Reaching the inversion point does not guarantee the transition. Electricity reached the economic inversion point for rural America in the 1920s, but universal provision did not arrive until the 1960s — a 40-year gap between when it made economic sense and when it actually happened. The delay was not technical or economic. It was political and institutional.

The same delay is likely for AI-driven floor-raising. The math may be undeniable within a decade. The institutional response may take another decade or two.

---

## Obstacles

### Regulatory Capture

Professional licensing regimes exist to protect quality. They also protect incumbents. The American Medical Association's historical opposition to telemedicine, the legal profession's UPL restrictions, and teacher certification requirements all serve dual functions: quality assurance and market protection. Separating the two is politically difficult because incumbents have more lobbying power than unserved populations.

AI-driven services will face the same resistance. Radiology AI that matches human accuracy will still face deployment barriers from professional organizations that control licensure and reimbursement decisions. The question is not whether the resistance occurs but how long it delays adoption.

### The Distribution Problem

Cost collapse at the production level does not automatically reach consumers. This is the most important obstacle and the one most easily overlooked.

When AI makes document review 10x cheaper, law firms can either pass the savings to clients or maintain prices and increase margins. The Bloomberg Law finding that AI has done "little to reduce billable hours" suggests the latter is happening first. The same dynamic applies in healthcare (AI reducing provider costs without reducing patient costs) and education (AI platforms charging subscription fees that capture most of the cost savings).

The historical pattern is that competition eventually forces pass-through — but "eventually" can mean decades, and the people at the lowest floors cannot wait decades.

### Infrastructure Access

AI services require devices and connectivity. The populations most in need of floor-raising are the populations least likely to have reliable access. The digital divide is not a separate problem — it is a prerequisite that must be addressed in parallel.

### Quality and Safety

AI systems that are "good enough on average" may not be good enough for the cases that matter most. Medical misdiagnosis, bad legal advice, and incorrect benefits determinations cause real harm. The quality floor must be high enough that AI assistance is reliably better than the status quo alternative (which, for the underserved populations in question, is often no assistance at all).

### Institutional Inertia

Healthcare systems, school districts, courts, and government agencies are among the slowest-moving institutions in society. They have legitimate reasons for caution (patient safety, due process, equity) and illegitimate reasons (bureaucratic self-preservation, budget protection, change aversion). Both produce the same outcome: slow adoption even when the economics are favorable.

---

## Timeline Assessment

### What Is Well-Evidenced

- AI inference costs are dropping at ~10x/year (documented 2022-2026).
- AI diagnostic accuracy matches or exceeds average specialist performance in specific, well-studied domains (radiology, dermatology screening, some pathology applications).
- AI tutoring produces measurable learning gains comparable to human tutoring in controlled studies.
- The justice gap (92% unmet legal needs) and healthcare access gap (28% delaying care due to cost) are large enough that even partial AI coverage shifts the economics.
- Historical cost-collapse-to-universality transitions took 20-40 years from technical viability to near-universal provision.

### What Is Projection

Everything below involves institutional adoption rates, regulatory timelines, and political dynamics that are inherently unpredictable. These estimates represent ranges, not predictions.

### Conservative Scenario (Institutions Resist, Adoption Is Slow)

| Domain | AI capability parity | Regulatory framework | Widespread deployment | Universal floor impact |
|--------|---------------------|----------------------|----------------------|----------------------|
| **Diagnostics/triage** | 2024-2026 (now) | 2028-2032 | 2032-2038 | 2035-2045 |
| **Education (tutoring)** | 2025-2027 (now) | 2027-2030 | 2030-2035 | 2033-2040 |
| **Legal guidance** | 2026-2028 | 2030-2035 | 2035-2040 | 2038-2045 |
| **Administrative** | 2025-2027 (now) | 2028-2033 | 2033-2040 | 2035-2045 |

In this scenario, the primary delays are regulatory approval cycles, professional resistance, and the infrastructure gap. The technology is ready or nearly ready in every domain, but institutional adoption adds 10-20 years. This mirrors the electricity timeline: the technology was ready in the 1920s, universal provision arrived in the 1960s.

### Optimistic Scenario (Crisis Accelerates Adoption)

| Domain | AI capability parity | Regulatory framework | Widespread deployment | Universal floor impact |
|--------|---------------------|----------------------|----------------------|----------------------|
| **Diagnostics/triage** | 2024-2026 (now) | 2026-2028 | 2028-2032 | 2030-2035 |
| **Education (tutoring)** | 2025-2027 (now) | 2026-2028 | 2027-2030 | 2029-2033 |
| **Legal guidance** | 2026-2028 | 2028-2030 | 2029-2033 | 2031-2036 |
| **Administrative** | 2025-2027 (now) | 2026-2029 | 2028-2032 | 2030-2035 |

This scenario assumes that a combination of fiscal pressure (healthcare costs, education costs, administrative costs becoming unsustainable), visible disparities (AI-assisted populations outperforming unassisted ones), and competitive dynamics (countries that adopt faster gaining economic advantages) compresses the regulatory and adoption timelines. Historical precedent exists: COVID compressed telemedicine adoption by 5-10 years in 6 months.

### The Key Variable

The difference between the scenarios is not technology. It is whether institutions are forced to change by crisis or choose to change by foresight. The historical record strongly favors crisis as the mechanism. The framework's insight — from the seed document — holds: "the solution is visible now, before the crisis. But it likely requires the crisis to become politically viable."

### What Could Accelerate the Timeline

- A country (likely not the US) achieves dramatically better health/education outcomes through aggressive AI deployment, creating competitive pressure.
- A major fiscal crisis forces governments to seek cheaper service delivery models.
- Open-source AI models make deployment possible outside of incumbent institutional channels.
- A generation that grew up with AI tutoring and ChatGPT enters the workforce and enters politics, treating AI-assisted services as a baseline expectation rather than a novelty.

### What Could Delay the Timeline

- A high-profile AI failure (misdiagnosis causing death, algorithmic bias denying benefits at scale) triggers regulatory backlash that freezes deployment for years.
- Incumbents successfully lobby for regulations that require human involvement in every AI-assisted interaction, eliminating the cost advantage.
- The distribution problem persists: AI makes services cheaper to produce but not cheaper to access, and the savings are captured by intermediaries.
- The digital divide widens rather than narrows, leaving the target population unable to access AI-driven services.

---

## Sources

### AI Cost Trajectories
- [LLM inference prices have fallen rapidly but unequally across tasks](https://epoch.ai/data-insights/llm-inference-price-trends) — Epoch AI
- [Welcome to LLMflation](https://a16z.com/llmflation-llm-inference-cost/) — Andreessen Horowitz
- [The Price of Progress: Algorithmic Efficiency and the Falling Cost of AI Inference](https://arxiv.org/html/2511.23455v1) — arXiv
- [AI Inference's 280x Slide: 18-Month Cost Optimization Explained](https://www.aicerts.ai/news/ai-inferences-280x-slide-18-month-cost-optimization-explained/) — AI CERTs
- [The Inference Cost Paradox](https://www.arturmarkus.com/the-inference-cost-paradox-why-generative-ai-spending-surged-320-in-2025-despite-per-token-costs-dropping-1000x-and-what-it-means-for-your-ai-budget-in-2026/) — AI Unfiltered

### Medical Diagnosis
- [AI Diagnostics: Revolutionizing Medical Diagnosis in 2026](https://www.scispot.com/blog/ai-diagnostics-revolutionizing-medical-diagnosis-in-2025) — SciSpot
- [AI in Radiology: 2025 Trends, FDA Approvals & Adoption](https://intuitionlabs.ai/articles/ai-radiology-trends-2025) — IntuitionLabs
- [Diagnostic performance of artificial intelligence for dermatological conditions](https://pmc.ncbi.nlm.nih.gov/articles/PMC12481837/) — PMC
- [Artificial intelligence in modern clinical practice](https://pmc.ncbi.nlm.nih.gov/articles/PMC12715461/) — PMC

### Education
- [AI tutoring outperforms in-class active learning: an RCT](https://www.nature.com/articles/s41598-025-97652-6) — Scientific Reports / Nature
- [What the research shows about generative AI in tutoring](https://www.brookings.edu/articles/what-the-research-shows-about-generative-ai-in-tutoring/) — Brookings
- [AI Tutors, With a Little Human Help, Offer 'Reliable' Instruction](https://www.the74million.org/article/ai-tutors-with-a-little-human-help-offer-reliable-instruction-study-finds/) — The 74
- [A systematic review of AI-driven intelligent tutoring systems in K-12 education](https://www.nature.com/articles/s41539-025-00320-7) — Nature / npj Science of Learning

### Legal Access
- [The Justice Gap Report](https://justicegap.lsc.gov/) — Legal Services Corporation
- [2024 Justice Gap Study](https://www.calbar.ca.gov/news/2024-justice-gap-study-shows-growing-unmet-legal-needs-amid-shifting-attorney-workforce) — State Bar of California
- [How AI Enhances Legal Document Review](https://www.americanbar.org/groups/law_practice/resources/law-technology-today/2025/how-ai-enhances-legal-document-review/) — American Bar Association
- [AI Does Little to Reduce Law Firm Billable Hours](https://news.bloomberglaw.com/in-house-counsel/ai-does-little-to-reduce-law-firm-billable-hours-survey-shows) — Bloomberg Law

### Healthcare Access and Costs
- [Preventable ED Use Costs $8.3 Billion Annually](https://www.hfma.org/payment-reimbursement-and-managed-care/payment-trends/63247/) — HFMA
- [How does cost affect access to healthcare?](https://www.healthsystemtracker.org/chart-collection/cost-affect-access-care/) — Peterson-KFF Health System Tracker
- [Unmet needs for healthcare](https://www.oecd.org/en/publications/health-at-a-glance-2025_8f9e3f98-en/full-report/unmet-needs-for-healthcare_c994e8b1.html) — OECD Health at a Glance 2025

### Government and Administrative AI
- [AI and Government Workers: Use Cases in Public Administration](https://rooseveltinstitute.org/publications/ai-and-government-workers/) — Roosevelt Institute
- [Modernizing government: The role of AI and automation](https://www.route-fifty.com/artificial-intelligence/2026/01/modernizing-government-role-ai-and-automation-government-innovation/410929/) — Route Fifty
- [The 2026 GT100: What It Will Take to Scale AI in Government](https://www.govtech.com/biz/the-2026-gt100-what-will-it-take-to-scale-ai-in-government) — GovTech

### Historical Precedent
- [Electrifying Rural America](https://www.richmondfed.org/publications/research/econ_focus/2020/q1/economic_history) — Federal Reserve Bank of Richmond
- [Short- and long-run impacts of rural electrification](https://www.sciencedirect.com/science/article/abs/pii/S0304387819304547) — Journal of Development Economics
- [Rural Electrification](https://www.ebsco.com/research-starters/history/rural-electrification) — EBSCO Research Starters

---

*This analysis supports the claim: [AI cost collapse makes floor-raising economically inevitable](../claims/cost-collapse.md).*

*Compiled March 2026. The cost trajectories are current as of publication. Institutional adoption timelines are estimates and should be revised as evidence accumulates. The intellectual honesty standard of this repository requires flagging: the cost data is strong, the domain performance data is solid, and the adoption timelines are educated guesses. The historical pattern is real. The speed at which it replays is the open question.*
