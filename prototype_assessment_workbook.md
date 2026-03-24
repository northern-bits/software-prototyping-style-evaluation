# Prototype Assessment Workbook

## Purpose

Use this workbook to decide **which assessment style or combination of styles** best fits a given software problem statement.

This workbook helps you determine whether a problem should be approached primarily through:

- **Practical Builder assessment**
- **Architect assessment**
- **Consumer-First assessment**
- **Risk-Killer assessment**

It is designed to be reusable for software packages, internal tools, frameworks, services, SDKs, platform components, and automation projects.

---

# How to use this workbook

1. Write the problem statement clearly.
2. Answer the multiple-choice questions.
3. Score the selected answers using the key.
4. Total the results by assessment style.
5. Use the interpretation guide to choose one primary style and, if needed, one or two supporting styles.
6. Complete the planning page for your chosen style mix.

---

# Assessment Styles

## 1. Practical Builder
Best when the fastest path to clarity is building something thin and tangible.

Optimizes for:
- momentum
- quick validation
- learning by implementation
- finding the smallest useful version

## 2. Architect
Best when the key issue is package boundary, abstraction quality, extensibility, or long-term maintainability.

Optimizes for:
- strong interfaces
- clean responsibilities
- internal structure
- future sustainability

## 3. Consumer-First
Best when adoption, ergonomics, onboarding, and usability matter most.

Optimizes for:
- developer experience
- intuitive usage
- low friction
- documentation and examples

## 4. Risk-Killer
Best when uncertainty, feasibility, performance, security, or integration risk could invalidate the concept.

Optimizes for:
- sharp risk reduction
- efficient testing of assumptions
- fast elimination of bad directions
- disciplined decision-making

---

# Page 1 — Problem Statement

## Problem statement

Write the problem in 3–6 lines.

- What are you trying to create?
- Who is it for?
- What problem does it solve?
- Why are you considering prototyping it?

### Notes

```
[Write here]
```

---

# Page 2 — Multiple Choice Self-Assessment

For each question, choose the answer that fits best.

## Q1. What is most important to figure out first?

A. Whether I can build a useful working version quickly.  
B. Whether this is the right abstraction and package boundary.  
C. Whether people will find it easy and natural to use.  
D. Whether the idea fails due to technical, security, or performance risk.  

## Q2. What would make this effort feel most successful in the next step?

A. A thin working demo.  
B. A clear contract and clean design.  
C. A usage flow that feels obvious.  
D. Evidence that the biggest risk is either valid or invalid.  

## Q3. What is the biggest danger right now?

A. Spending too much time planning instead of building.  
B. Building the wrong structure and regretting it later.  
C. Creating something technically correct but painful to consume.  
D. Building on assumptions that may be false.  

## Q4. Which statement sounds most like your current need?

A. “I need to make this real enough to see it.”  
B. “I need to define what belongs inside and outside this package.”  
C. “I need to understand what the user experience should feel like.”  
D. “I need to attack the uncertainty first.”  

## Q5. If you only had one day, what would you most want to walk away with?

A. A working prototype.  
B. A clean API and module design.  
C. A README or example flow users can follow.  
D. A spike, benchmark, or feasibility result.  

## Q6. Which kind of question is most dominant in this problem?

A. “What is the smallest thing that proves usefulness?”  
B. “What is the right system shape?”  
C. “What will the user actually do?”  
D. “What assumption could kill this?”  

## Q7. How much does long-term maintainability matter right now?

A. Somewhat, but not yet more than proving the core idea.  
B. A lot; poor design now will be expensive later.  
C. It matters, but ease of use is more important at first.  
D. It matters, but first I need to know whether this is viable at all.  

## Q8. What kind of package or system is this closest to?

A. An internal helper, script, tool, or automation component.  
B. A shared library, framework, platform component, or reusable core service.  
C. An SDK, CLI, developer tool, or workflow package meant for adoption.  
D. A security, infra, data, integration-heavy, or performance-sensitive component.  

## Q9. What is your preferred way of gaining clarity?

A. Build and inspect.  
B. Model and define.  
C. Simulate user behavior.  
D. Test assumptions directly.  

## Q10. What would be the most useful first artifact?

A. A thin implementation.  
B. An interface sketch or architecture note.  
C. A usage example or README-first draft.  
D. A benchmark, spike, or experiment design.  

## Q11. If this prototype went badly, what would bother you most?

A. I spent time but still have nothing concrete.  
B. I created technical debt by locking in a weak design.  
C. I made something nobody enjoys using.  
D. I missed an obvious fatal risk too late.  

## Q12. Which outcome would give you the most confidence to proceed?

A. The main workflow works end to end.  
B. The package boundary and API make structural sense.  
C. A user could succeed with minimal guidance.  
D. The biggest uncertainty has been objectively tested.  

---

# Page 3 — Scoring Key

For each selected answer, score as follows:

- **A = Practical Builder**
- **B = Architect**
- **C = Consumer-First**
- **D = Risk-Killer**

## Score sheet

| Question | Choice | Style |
|---|---|---|
| Q1 |   |   |
| Q2 |   |   |
| Q3 |   |   |
| Q4 |   |   |
| Q5 |   |   |
| Q6 |   |   |
| Q7 |   |   |
| Q8 |   |   |
| Q9 |   |   |
| Q10 |   |   |
| Q11 |   |   |
| Q12 |   |   |

## Totals

- Practical Builder: ___
- Architect: ___
- Consumer-First: ___
- Risk-Killer: ___

---

# Page 4 — Interpretation Guide

## If one style clearly leads by 3 or more points
Use that as the **primary assessment style**.

## If two styles are close within 1–2 points
Use a **hybrid approach**.

Common useful pairings:

- **Builder + Risk-Killer**  
  Best for fast technical spikes where feasibility is uncertain.

- **Architect + Consumer-First**  
  Best for shared packages where design quality and usability both matter.

- **Architect + Risk-Killer**  
  Best for foundational systems where structural choices and technical risk both matter.

- **Builder + Consumer-First**  
  Best for lightweight tools, CLIs, or internal developer tooling.

- **Consumer-First + Risk-Killer**  
  Best for tools that must be both easy to adopt and proven under constraints.

## If all four are close
The problem likely needs a staged assessment:

1. Risk-Killer first  
2. Architect second  
3. Consumer-First third  
4. Builder fourth  

That usually means the concept is broad enough that you should not jump straight into implementation.

---

# Page 5 — Action Planning Page

## Primary style selected

```
[Write here]
```

## Supporting style(s)

```
[Write here]
```

## Why these fit this problem

```
[Write here]
```

## What to do first

```
[Write here]
```

## What not to do yet

```
[Write here]
```

## Prototype exit criteria

```
[Write here]
```

---

# Page 6 — Style-Specific Guided Prompts

## Practical Builder prompts

- What is the smallest useful version?
- What is the golden path workflow?
- What can I hardcode or fake for now?
- What thin implementation would prove basic usefulness?
- What does “done enough to learn” look like?

## Architect prompts

- Why should this be a package at all?
- What belongs inside vs outside the package?
- What is the public contract?
- What extension points are needed?
- What design choice would be expensive to change later?

## Consumer-First prompts

- Who is the user?
- What are the top 3 user tasks?
- What should first-use experience feel like?
- What defaults, naming, and examples reduce friction?
- What would frustrate a user immediately?

## Risk-Killer prompts

- What assumption is carrying the most risk?
- What could invalidate the idea entirely?
- What is the cheapest test for that?
- What evidence would justify continuing?
- What should be deferred until after the risk is tested?

---

# Page 7 — Reusable Blank Example Template

## Example name

```
[Write here]
```

## Problem statement

```
[Write here]
```

## Answer selections

- Q1:
- Q2:
- Q3:
- Q4:
- Q5:
- Q6:
- Q7:
- Q8:
- Q9:
- Q10:
- Q11:
- Q12:

## Totals

- Practical Builder:
- Architect:
- Consumer-First:
- Risk-Killer:

## Recommended style mix

```
[Write here]
```

## Why this mix fits

```
[Write here]
```

## First prototype move

```
[Write here]
```

## Exit criteria

```
[Write here]
```

---

# Filled-In Example 1 — Internal Python package for standardizing auth middleware

## Problem statement

Create a reusable internal Python package that standardizes request authentication and authorization checks across multiple internal services. It should reduce duplication, enforce secure defaults, and be simple for backend teams to integrate.

## Answer selections

- Q1: B
- Q2: B
- Q3: B
- Q4: B
- Q5: B
- Q6: B
- Q7: B
- Q8: B
- Q9: B
- Q10: B
- Q11: B
- Q12: B

## Totals

- Practical Builder: 0
- Architect: 12
- Consumer-First: 0
- Risk-Killer: 0

## Recommended style mix

Architect primary, Risk-Killer secondary.

## Why this mix fits

The main challenge is defining the correct package boundary, public API, responsibilities, and extension model. Because auth-related packages are difficult to change later and can create widespread technical debt if designed poorly, architecture must lead. A secondary Risk-Killer pass is useful to test trust-boundary assumptions and integration realities before wider rollout.

## First prototype move

Write the public contract first: middleware entry points, configuration model, error model, and extension hooks. Then build one thin integration into a sample service.

## Exit criteria

- Draft public API defined
- One sample service integrated successfully
- Security assumptions documented
- Key ownership boundaries clarified
- Decision made on whether the package should remain generic or be framework-specific

---

# Filled-In Example 2 — CLI tool for helping developers scaffold small automation jobs

## Problem statement

Create a CLI package that helps internal engineers quickly scaffold small automation jobs with a standard folder layout, config file, logging, and test starter files. It should be simple enough that an engineer can use it without reading much documentation.

## Answer selections

- Q1: C
- Q2: C
- Q3: C
- Q4: C
- Q5: C
- Q6: C
- Q7: C
- Q8: C
- Q9: C
- Q10: C
- Q11: C
- Q12: C

## Totals

- Practical Builder: 0
- Architect: 0
- Consumer-First: 12
- Risk-Killer: 0

## Recommended style mix

Consumer-First primary, Practical Builder secondary.

## Why this mix fits

The main success factor is adoption and ease of use. The tool will only succeed if developers can discover commands, understand outputs, and generate value with minimal friction. A Practical Builder secondary style helps produce a thin working CLI quickly and refine it through direct usage.

## First prototype move

Write three example user flows first: create a new job, add logging, and generate starter tests. Then implement the thinnest CLI that supports those flows.

## Exit criteria

- A user can install and run the CLI locally
- Three common flows work cleanly
- Command names and flags feel intuitive
- README supports first use without extra explanation
- At least one user can succeed from the docs alone

---

# Filled-In Example 3 — Data ingestion package for pulling findings from multiple security APIs

## Problem statement

Create a package that ingests vulnerability and asset findings from multiple external security APIs, normalizes them into a common schema, and stores them for downstream analysis. The package may need to handle rate limits, inconsistent schemas, retries, and high-volume ingestion.

## Answer selections

- Q1: D
- Q2: D
- Q3: D
- Q4: D
- Q5: D
- Q6: D
- Q7: D
- Q8: D
- Q9: D
- Q10: D
- Q11: D
- Q12: D

## Totals

- Practical Builder: 0
- Architect: 0
- Consumer-First: 0
- Risk-Killer: 12

## Recommended style mix

Risk-Killer primary, Architect secondary.

## Why this mix fits

The main threat is not whether the package can be coded, but whether the underlying assumptions about source behavior, normalization, throughput, idempotency, and failure handling are valid. If these are wrong, the package will fail regardless of implementation effort. Once those risks are tested, architectural structure becomes the next concern because schema handling and connector boundaries must remain maintainable.

## First prototype move

Run a technical spike against two representative APIs using a stripped-down normalization path. Measure schema mismatch frequency, retry behavior, and throughput before broadening scope.

## Exit criteria

- At least two source APIs ingested successfully
- Core schema mapping validated
- Throughput and retry behavior observed
- Failure modes documented
- Decision made on connector model and normalization strategy

---

# Closing Notes

This workbook is meant to help you choose the **right thinking mode before you choose the implementation path**.

The goal is not to force every problem into one style. The goal is to identify:

- what kind of uncertainty dominates the problem
- what kind of evidence you need next
- what style of assessment should lead your prototype

Over time, you may discover your default preferences. That is useful. But the most effective prototyping practice is usually situational, not ideological.

