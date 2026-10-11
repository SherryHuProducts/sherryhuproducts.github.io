---
{
  "title": "Why I separate a score from a decision",
  "date": "2026-10-10",
  "tags": [
    "Applied AI"
  ],
  "description": "A single score is convenient, but it can hide what a system actually knows.",
  "summary": "A single score is convenient, but it can hide what a system actually knows.",
  "draft": false,
  "ShowReadingTime": true
}
---

> Working draft · Initial site copy based on my public project.


A single score is convenient, but it can hide what a system actually knows.

In JobFit AI, I keep four concepts separate: Fit Score, Gap Severity, Recommendation, and the person's final decision. A job discovered by the scanner is a lead. It still needs review. A recommendation is decision support. It does not authorize an application.

This separation helps me ask more useful evaluation questions. Did discovery miss a plausible role? Did triage exclude it for the wrong reason? Was the evaluation supported by evidence? Did the recommendation make uncertainty visible?

I am also exploring blind human labeling: record a person's judgment before showing the AI output. That order helps reduce anchoring on the system's score.

My takeaway: inspect the stages and the evidence, not just the final number.

[View the project](/projects/jobfit-ai/)
