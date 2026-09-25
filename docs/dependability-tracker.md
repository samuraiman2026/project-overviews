# Dependability Tracker

## The problem

A difference between a planned shift and a time record does not explain why it happened. Treating every discrepancy as an employee issue can confuse scheduling changes, coverage, corrected records, and events that need a manager's review.

## What it does

Dependability Tracker compares schedule and time-record data, assembles discrepancies into a review queue, and summarizes staffing and coverage patterns. It is designed to make exceptions visible and give managers a consistent place to classify them.

## Product choices

- Preserve the complete discrepancy queue instead of hiding records when there are more exceptions than expected.
- Keep uncertain cases in review until a manager supplies context.
- Separate staffing impact from accountability decisions. The software does not infer performance issues or make disciplinary decisions.
- Leave source scheduling and timekeeping records unchanged.

This is an operational review aid, not a payroll source of truth or an automated employee evaluation system. The implementation and any organization-specific operating details remain private.
