---
{
  "title": "SignalBrief",
  "description": "Long podcasts into structured research questions.",
  "weight": 5,
  "category": "Applied AI",
  "status": "V0.3 research prototype",
  "cardimage": "/images/signal.svg",
  "repo": "https://github.com/SherryHuProducts/signal-brief",
  "tags": [
    "Python",
    "RSS",
    "Speech-to-text",
    "Structured extraction"
  ],
  "showtoc": true,
  "tocopen": false,
  "hidemeta": true
}
---


## The problem
A two- or three-hour business podcast contains more material than a reliable one-shot summary can comfortably handle. Facts, opinions, forecasts, and uncertainty can blur together.

## The approach
SignalBrief V0.3 retrieves podcast audio through RSS, chunks long audio for transcription, extracts structured findings, and synthesizes those findings into a research brief.

## Two stages
1. Extract entities, numbers, claims, opinions, forecasts, contradictions, and follow-up questions from manageable chunks.
2. Deduplicate and synthesize findings across the episode, preserving uncertainty and separating facts from predictions.

The machine-readable findings are retained alongside the transcript and brief so later work can build on them.

## Current scope
A personal research prototype focused on podcasts. Retries, checkpoint/resume, timestamps, and cost tracking are on the roadmap. It is not an automated trading system or a source of personalized investment instructions.


[Explore the repository →](https://github.com/SherryHuProducts/signal-brief)
