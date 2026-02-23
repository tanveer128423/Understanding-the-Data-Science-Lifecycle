# Understanding the Data Science Lifecycle

## Part A: README Documentation

### 1 Explaining the Question → Data → Insight Lifecycle

Data science should begin with a **question**, not a tool. A clear question defines the decision that needs support, the people affected, and what success looks like. If the question is vague, even strong analysis can become noise because it may answer something technically correct but practically useless.

Once the question is clear, **data** becomes evidence. Data is not just a spreadsheet to run through charts or models. It has context: how it was collected, what each field means, what might be missing, and what biases may exist. “Understanding data before analyzing it” means checking whether the data actually represents the real-world process behind the question. If it does not, the analysis can look precise while still being wrong.

**Insights** are the result of connecting evidence back to the original decision. Insight is not “we found a correlation” or “the model has high accuracy.” Insight is a meaningful explanation that can guide action, such as where to intervene, what to prioritize, or what trade-off exists. In other words, insight emerges from exploration + context + interpretation, not from numbers alone.

These steps connect tightly:

- The question tells us what data is relevant.
- Data quality and context determine whether findings are trustworthy.
- Insight is only valuable when it answers the original decision problem.

If we skip or weaken any step, the whole lifecycle breaks: unclear question leads to irrelevant data work, weak data understanding leads to misleading results, and weak interpretation leads to decisions with low impact.

---

### 2) Applying the Lifecycle to a Project Context

#### Project Context: Student Retention in an Online Learning Program

**Question**

Which early learning behaviors best predict whether a student is at risk of dropping out in the first 6 weeks, so support teams can intervene early?

**Data needed (source + representation)**

- Learning platform logs (LMS): login frequency, session duration, assignment submission timing, quiz attempts.
- Academic records: baseline performance, course load, prior completion history.
- Student support interactions: tutoring usage, advisor contact frequency, unresolved support tickets.
- Optional survey/check-in data: motivation level, time constraints, self-reported confidence.

This data represents engagement, performance trajectory, and support access. Together, these dimensions help explain not only _who_ is struggling, but _why_.

**Useful insight for decision-making**

A useful insight would be: students who miss two consecutive weekly assignments and show a sharp drop in login activity are significantly more likely to withdraw unless contacted within one week. This helps decision-makers create targeted retention actions (automated alerts + advisor outreach) instead of broad, less effective interventions.

The goal is not just prediction; the goal is actionable understanding that improves student outcomes.

---

## Part B: Video Walkthrough (~2 Minutes)

### Suggested Talk Track

1. Briefly explain that your README is organized around Question → Data → Insight.
2. Explain why a clear question must come first (decision-focused, avoids random analysis).
3. Explain that data is evidence with context (quality, meaning, limits, bias).
4. Explain how insights must be actionable, not just statistical outputs.
5. Walk through your project example (student retention) and connect each lifecycle stage.
6. Conclude with why this lifecycle reduces wasted effort and improves decision quality.

### Scenario-Based Reasoning (Mandatory)

**Scenario:** You receive a dataset with many columns but no clear problem statement, and a teammate wants to build visualizations/models immediately.

**How I would respond using Question → Data → Insight:**

I would pause model-building and first clarify the decision context: _What decision are we trying to support, for whom, and on what timeline?_ Without that, we may optimize for interesting patterns instead of useful outcomes.

Next, I would assess the dataset against that question: which columns are relevant, how fields were collected, what missingness exists, and whether there are bias or leakage risks. Dozens of columns can create false confidence if we do not understand representativeness and meaning.

Risks of skipping steps include:

- Building models that solve the wrong problem.
- Producing visually impressive but non-actionable dashboards.
- Making decisions from biased or low-quality signals.
- Wasting time and stakeholder trust when results cannot be translated into action.

To realign the work, I would propose a short framing step: define the question, define success criteria, map needed variables, then do focused exploration tied to that question. That keeps analysis purposeful and increases the chance of generating insights that decision-makers can actually use.

---

## Submission Checklist

- README updated with both required sections.
- Explanation uses reasoning and clear lifecycle flow.
- One realistic project context included.
- Video (~2 minutes) covers README and scenario response.
