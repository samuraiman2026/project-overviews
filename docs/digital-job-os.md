# Digital Job OS

## The problem

A job search can turn into a collection of disconnected tabs, notes, drafts, and half-finished follow-ups. The difficult part is rarely finding a job listing. It is deciding where to spend time, keeping the next action clear, and carrying useful context from first look to follow-through.

Digital Job OS is a private, personal workflow system built to make that work more deliberate.

## What I built

The product pairs a browser extension with a companion workspace. Together, they support a connected flow:

1. Review a role where it is posted.
2. See a transparent initial-fit assessment and the factors behind it.
3. Queue promising roles into a pipeline without re-entering the job description.
4. Surface possible warm paths before defaulting to a cold application.
5. Prepare role-specific application and outreach materials.
6. Track follow-ups and outcomes, then use those outcomes to question whether the scoring is actually helping.

It is intentionally more than a prompt collection. The useful unit is the workflow: a decision, its context, and the next responsible action.

## Design choices that matter

### Keep the first score inspectable

The initial assessment is rule-based and explains the match, gaps, and disqualifying requirements. An optional model-assisted assessment is presented separately, so a polished explanation does not masquerade as a deterministic score.

### Make the warm path visible early

The system checks an imported professional network for potential first-degree connections at a company. That changes the operating question from “Should I apply?” to “What is the most credible path into this conversation?”

### Treat outcomes as feedback, not decoration

The workflow records outcomes across opportunities and outreach. That makes it possible to compare predicted fit with real progression and revise the evaluation logic, rather than quietly trusting a score because it looks precise.

### Preserve the user’s agency and data boundary

Personal context, application materials, contact data, and sensitive job-search state remain private. The system provides structured prompts and recommendations; it does not send messages or apply to jobs on the user’s behalf.

## Implementation at a glance

- Browser extension for in-context job review and workflow handoff
- Companion dashboard for pipeline, application, and follow-up work
- Shared scoring logic with regression checks to prevent the extension and dashboard from drifting apart
- Local persistence, export, and recovery paths for user-owned workflow state
- Optional model API for deeper analysis, clearly separated from deterministic assessment

## What this project demonstrates

This is a product-management problem as much as a software problem: choosing what to automate, keeping automated judgment legible, and designing for the work people actually have to do after an answer appears.

The source repository and personal data remain private.
