# Registry design

## Purpose
The registry is the canonical structured index of the 200 approved JD IQ investigations.

## Data integrity rules
- Investigation numbers are stable identifiers from 1 through 200.
- The programme is closed at #200. Do not create #201 without explicit approval.
- Unknown titles, identifiers and descriptions remain null until recovered from an approved source.
- A conversation-history summary is provenance, not independent verification.
- Do not mark a record verified until it has been checked against its original approved record.
- Preserve historical duplicate warnings until reviewed; do not silently merge or renumber records.

## Record lifecycle
1. `needs_source_recovery`: original details are not currently available.
2. `partial_source_recovery_required`: some metadata is preserved, but the full source record is incomplete.
3. `source_recovered`: the original approved record has been recovered and its provenance recorded.
4. `verified`: the recovered record has been checked for fidelity and consistency.

## Current limitations
This initial registry contains only the information available in the project handover summary. Most investigation descriptions and several numbered entries require recovery from earlier approved records. The registry deliberately does not fabricate them.

## Future extensions
Subject to review, later versions may add discipline tags, research objectives, relationships, dependencies, status history, review notes and source citations.
