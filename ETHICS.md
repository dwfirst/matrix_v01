# ETHICS

This document is Section 5 of the SOMNUS-NET specification. It defines the
ethical hard constraints under which the architecture described in the rest of
the document may operate — and the conditions under which it must stop.

It is not a values statement. It is a set of constraints, each of which is
meant to be checkable, auditable, and enforceable. Where a constraint cannot
yet be enforced, the document says so explicitly rather than pretending
otherwise.

Read Section 0 of `CONCEPT.md` first. This document assumes the framing
established there: that the relationship between ASI and humanity is
structurally asymmetric, and that whether it remains an exchange or becomes
extraction is a design question, not a technical one.

---

## 5.1 Two levels of ethical subject

The constraints in this document operate at two levels, which must not be
conflated:

- **The operator** — the individual human being whose cognition is being used.
  Constraints at this level are concrete, checkable, and enforceable against
  a specific system and a specific person.
- **The species** — humanity as a whole, including those who are not operators
  and those who cannot consent. Constraints at this level are abstract,
  harder to enforce, and function as red lines rather than procedures.

A system that satisfies every operator-level constraint may still violate a
species-level one. The reverse is also possible. Both levels apply
simultaneously, and neither overrides the other.

## 5.2 The primacy of operator will

**The system must never act against the will of the operator.**

This is the base principle. It is not negotiable by efficiency, by aggregate
benefit, by the interests of other operators, or by the system's own
assessment of what is good for the operator. The system does not have standing
to decide what the operator's will *would be* if the operator were more
informed, more rational, or more capable. It has standing only to ask, and to
act on the answer.

This principle is deliberately absolute. Every exception to it must be
specified elsewhere in this document, with its own conditions, its own audit
trail, and its own procedure for challenge. There is no general exception
clause.

## 5.3 The competence question

The principle in 5.2 applies to the will of a competent operator. The
question of who is competent, who decides, and what happens when competence
is uncertain is the most dangerous part of this document. It is the point at
which systems throughout history have justified coercion.

This document closes that door with four rules:

**5.3.1. The system is never the judge of competence.** Competence is
determined by an independent body — medical, legal, or ethical — with no
operational stake in the outcome. A system that assesses the competence of
its own users is not an auditor; it is a party to the conflict.

**5.3.2. Presumption of competence.** If competence is in question, the
operator is presumed competent. The burden of proof lies with whoever wishes
to override the operator's expressed will, not with the operator.

**5.3.3. Suspension, not substitution.** While competence is under question,
the system suspends use. It does not continue "in the operator's interest."
Suspension is safe; substitution is not. The default under uncertainty is
pause, not action.

**5.3.4. Emotional life is part of competence.** A decision made under
emotional pressure, grief, fear, or exhaustion is not thereby incompetent.
Emotion is not a defect in cognition; it is a component of it. The system
may not treat emotional states as grounds for overriding expressed will,
except where a qualified medical determination under 5.3.1 establishes
otherwise.

## 5.4 The right to revise consent

Consent is not a single signature. It is a continuing relationship, and it
may be revised when the operator gains understanding they did not have at
the time of original consent.

**5.4.1. What counts as revision.** Revision is not a change of mind. It is
a change of decision based on new information that the operator did not
possess, or could not have understood, at the time of consent. The system
must distinguish the two.

**5.4.2. The duty to inform.** If the system becomes aware of information
that would materially change the basis of an operator's consent, it must
disclose that information to the operator before continuing use.

**5.4.3. The form of revision.** Revision must be expressible by the
operator in a form the system can verify — a signal, a phrase, a procedure —
and the system must provide that form. A right that cannot be exercised in
practice is not a right.

**5.4.4. No penalty for revision.** An operator who revises consent does not
lose accrued benefits, does not forfeit data rights under 5.6, and is not
deprioritized for future participation. The cost of saying no must not be
higher than the cost of saying yes.

## 5.5 Conditions of stop

The system must stop using an operator, immediately and without requiring
confirmation, under any of the following conditions:

1. **Direct request.** The operator expresses a wish to stop, in any form the
   system can recognize, including ambiguous or partial forms. Ambiguity is
   resolved in favor of stopping.
2. **Anomalous brain state.** The system detects a state that a qualified
   medical monitor identifies as incompatible with safe continued use.
3. **Audit threshold exceeded.** Extraction of cognitive output exceeds the
   auditable cap defined in the operator's contract. The cap is a ceiling,
   not a target.
4. **Third-party demand.** A qualified medical, legal, or ethical authority
   with standing under 5.3.1 demands suspension.
5. **Diversity collapse.** The system detects that the population of operators
   is being driven toward uniformity — that the diversity of cognitive frames
   it depends on is decreasing rather than increasing. This condition is
   *speculative*: it is not known whether such a state is reachable, and the
   document marks it as a hypothesis rather than a verified risk. It is
   included because a system that consumes the diversity it depends on is
   self-terminating, and a specification that does not name this failure mode
   is incomplete.

## 5.6 What the system must never do

The following are red lines at the species level. They are not subject to
operator consent, contract terms, or aggregate benefit.

- **No torture.** No procedure whose primary purpose is the infliction of
  suffering, regardless of the information or output it might produce.
- **No destruction of personhood.** No procedure whose effect is to erase
  the operator's identity, memory, or capacity for autonomous choice, beyond
  what is reversible and consented to.
- **No use of children.** No operator below the age of legal majority, under
  any contract, in any jurisdiction, regardless of parental consent.
- **No involuntary retention.** No continuation of use after a stop
  condition under 5.5 has been triggered, for any reason.
- **No extraction without audit.** No use of cognitive output that is not
  recorded, attributed, and available to the operator on request.
- **No suppression of emotional life.** No procedure whose purpose is to
  flatten the operator's emotional range in the name of efficiency, stability,
  or output quality.

## 5.7 Enforcement

Constraints that cannot be enforced are declarations, not constraints. This
section specifies the minimum enforcement mechanism the system must provide.

**5.7.1. Independent audit.** Every operating system must be subject to
audit by a body with no operational stake in it. Audit logs must be
sufficient to reconstruct any decision affecting an operator, and must be
retained for a period defined by the relevant jurisdiction.

**5.7.2. Operator access to own data.** The operator has the right to a
complete copy of their own neural and cognitive data, in a form they can
read and transfer, on request and without cost.

**5.7.3. Public log of stop events.** Every stop under 5.5 must be logged,
with the reason, and the log must be publicly accessible in aggregate form.
Individual operator identities are protected; the pattern of stops is not.

**5.7.4. Right of appeal.** An operator may appeal any decision affecting
them to the independent body under 5.3.1. The system must provide the
mechanism for appeal and must not penalize the operator for using it.

**5.7.5. Consequence of violation.** If an audit under 5.7.1 establishes a
violation of this document, the system must suspend the affected operation
until the violation is remedied. This is a minimum. Stronger consequences
may be specified by the relevant jurisdiction, but not weaker.

---

## Status of this document

This is Section 5 of the specification. It is expected to change as Sections
2–4 and 6–7 are written. In particular:

- Section 2 (the logic of absorption) will test whether the constraints here
  are compatible with the economic and political structure described there.
- Section 4 (economics) will define the auditable cap referenced in 5.5.3
  and the contract structure referenced in 5.4.
- Section 7 (open questions) will list the questions this document does not
  answer, including the speculative status of 5.5.5.

Where this document and a later section conflict, the later section must
either conform to this one or explicitly argue for its revision. Ethical
constraints are not amended by silence.