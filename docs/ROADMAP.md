# Possible Roadmap

**All milestones below are possible future work. None is completed, scheduled, or committed.** Sequence and scope may change after research and feasibility review.

## 0. Clarify the problem

- Interview potential Windows users and support practitioners.
- Identify initial use cases and explicitly out-of-scope problems.
- Define user expectations for evidence, consent, privacy, and reporting.

## 1. Feasibility and requirements

- Review Windows diagnostic data sources and required permissions.
- Define a privacy and security threat model, data minimization goals, and retention expectations.
- Assess whether local inference is practical for candidate use cases and what cloud options would entail.
- Define safety criteria for recommendations and system-changing operations.

## 2. Architecture and interaction design

- Select an initial diagnostic workflow and component boundaries.
- Specify evidence provenance, uncertainty communication, policy checks, and audit records.
- Design user review and approval flows before considering execution.
- Decide whether a limited prototype is justified.

## 3. Controlled prototype, if approved

- Prototype read-only collection and evidence presentation for a narrow use case.
- Evaluate diagnostic quality and false or unsupported hypotheses.
- Keep remediation disabled until the action boundary, consent model, and safeguards are reviewed.

## 4. Safety evaluation

- If remediation is pursued, select narrowly scoped actions with documented preconditions and failure handling.
- Evaluate permission boundaries, verification, recovery support, and user comprehension.
- Conduct appropriate security and reliability review before broader use.

## 5. Potential expansion

- Consider additional diagnostic domains, modular extensions, or automation workflows only after the initial scope is validated.
- Reassess privacy, compatibility, support, and maintenance costs as capabilities expand.

No dates, release commitments, or completion claims are implied by these stages.
