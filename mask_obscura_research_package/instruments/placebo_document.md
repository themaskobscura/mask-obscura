# Internal Documentation Standards — Reference Memo

*Standards Committee — current revision*

## Purpose

This memo sets the standards governing internal documentation: reports, procedures, technical notes, and records of decisions. Its aim is uniformity of practice, not uniformity of voice. A document that follows these standards can be read, trusted, and acted on by someone who was not present when it was written. That is the only test that matters; every rule below serves it.

## Scope

These standards apply to all documents intended to outlive the conversation that produced them. They do not apply to informal chat, drafts circulated for comment, or personal working notes — though authors are encouraged to apply the naming and dating conventions everywhere, since drafts have a habit of becoming records.

## General Principles

**1. Write for the absent reader.** Assume the reader was not in the meeting, does not know the project's history, and cannot ask you questions. Define abbreviations at first use. Name systems and people by full identifiers, not nicknames. State dates absolutely (12 March 2026), never relatively ("last Tuesday").

**2. One document, one purpose.** A document should answer a single question: what was decided, how a procedure runs, what an investigation found. Documents that mix purposes lose all of them. If two purposes arise, write two documents and cross-reference.

**3. State status on the face of the document.** Every document carries one of four statuses in its header: DRAFT, REVIEW, APPROVED, SUPERSEDED. A document without a status is treated as DRAFT. When a document is superseded, the header must name its successor.

**4. Record decisions with their reasons.** A decision recorded without its rationale is half a record. Future readers need to know not only what was chosen but what was rejected and why, in two or three sentences. This is the part most often skipped and most often needed.

**5. Distinguish fact from judgment.** Observations, measurements, and quotations are facts; interpretations, estimates, and recommendations are judgments. Both belong in documents, clearly separated. Phrases like "it appears that" and "we estimate" are not weakness; they are accuracy.

## Structure and Format

Documents longer than one page carry a summary at the top, no more than five sentences, written last. Headings are descriptive, not clever. Numbered sections are used wherever a document will be cited by section. Tables are used for genuinely tabular material only; prose forced into tables loses its qualifications and caveats, which are usually the most important part.

Version numbers follow the pattern major.minor: a major increment for changes of substance, a minor increment for corrections that change no meaning. The version history table at the foot of the document lists every version, its date, its author, and a one-line description of what changed. Deletions are listed as explicitly as additions; a reader comparing versions should never need to discover a removal by accident.

## Review and Approval

Every document moving from DRAFT to APPROVED passes through at least one reviewer who is not its author. The reviewer's task is not stylistic polish but verification: are the facts checkable, the references live, the numbers consistent across the document? Reviewers sign with name and date. A review that proposes no changes states explicitly what was checked.

Approved documents are stored in the document register, named according to the convention `area_topic_status_version`, and never edited in place: corrections produce a new version through the same review path. The register entry, not the file on someone's machine, is the document of record.

## Retention and Retirement

Documents are retained according to their class: decision records permanently, procedures for the life of the procedure plus two years, technical notes for five years. Retirement is an action, not an absence: a retired document is marked SUPERSEDED with a pointer forward, and remains readable. Deleting a record is a separate, logged act requiring sign-off, because a gap in a record sequence is itself information that something happened.

## Closing Note

These standards are deliberately modest. They do not ask for elegant prose or exhaustive detail; they ask that every document say what it is, who stands behind it, what changed since last time, and how a stranger can verify it. Documents written this way age well. Documents written otherwise generate meetings.
