# Decisions and Open Questions

**Status:** Initial design record for an unimplemented concept. Entries document current proposals and unresolved choices, not finalized product decisions.

## Current concept-level decisions

| Topic | Current direction | Status |
| --- | --- | --- |
| Product purpose | Windows troubleshooting and maintenance assistance grounded in system evidence | Proposed |
| Capability status | Describe all capabilities as proposed until implemented and evaluated | Current documentation rule |
| Diagnostics | Consider telemetry, logs, performance metrics, and error information | Proposed; sources undecided |
| AI role | Assist diagnosis and recommendations; preserve uncertainty and evidence | Proposed |
| Local inference | Explore as an optional privacy-oriented mode | Open feasibility question |
| System changes | Require permission-controlled execution | Proposed safety requirement; mechanism undecided |
| Verification | Re-observe relevant state and report outcomes | Proposed |
| Recovery | Explore rollback only for operations where support can be established | Open feasibility question |
| Extensibility | Consider plugins and automation as later possibilities | Not in initial scope |

## Open questions

### Product scope

- Which single user problem and audience should be addressed first?
- What issues should be expressly unsupported?
- What evidence does a user need to trust or challenge a diagnosis?

### Windows and collection

- Which Windows versions and editions should be in scope?
- Which event channels, metrics, and system facts are necessary for an initial use case?
- How should collection be consented to, minimized, stored, inspected, and deleted?
- How should sensitive values and secrets be excluded or redacted?

### AI and privacy

- Which tasks need AI, and which can be handled by deterministic diagnostics?
- Which local models and hardware requirements, if any, are suitable?
- Would any cloud inference be offered? If so, what data may leave the device and under what user controls?
- How will unsupported conclusions, uncertainty, and conflicting evidence be represented?

### Safety and operations

- Which actions, if any, are safe enough to support first?
- How will approval be scoped to an action and expire or be revoked?
- What privilege model, allowlist, and policy enforcement are appropriate?
- What qualifies as successful verification?
- Which actions have reliable rollback, and how will irreversible effects be explained?

### Engineering and governance

- What languages, frameworks, update mechanism, and storage format fit the requirements?
- How would diagnostic rules and potential plugins be reviewed, signed, versioned, and isolated?
- What security review, testing, telemetry governance, and support process would be required?
- What legal, privacy, accessibility, and regulatory obligations apply to the eventual product and its distribution?

## Change process

As the concept changes, update the relevant document with a dated explanation. If a decision becomes sufficiently concrete, record its rationale, alternatives considered, and consequences here. Repository commits may provide supporting change history, but do not establish legal ownership or priority by themselves.
