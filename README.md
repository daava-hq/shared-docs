# shared-docs

Shareable Daava specifications and product documentation for reviewers.

---

## Documents

| Document | Covers |
| --- | --- |
| [`docs/dental-insurance-claims-specification.md`](./docs/dental-insurance-claims-specification.md) | End-to-end dental insurance and claims lifecycle — intake and coverage triage, EDI 270/271 eligibility, Open Dental write-back, clinical sign-off, AI CDT scrubbing, human-in-the-loop EDI 837D transmission, and STAX balance reconciliation. Includes a seven-phase Mermaid decision tree. |

---

## Rendering

All workflow diagrams are written in [Mermaid](https://mermaid.js.org/) and render natively on GitHub. To render them locally, use the [Mermaid CLI](https://github.com/mermaid-js/mermaid-cli):

```bash
npx -p @mermaid-js/mermaid-cli mmdc -i diagram.mmd -o diagram.svg
```

---

## Scope and status

- These documents describe planned and in-flight product behaviour. They are provided for review and are not contractual commitments.
- Nothing in this repository contains patient health information. Clinical examples use procedure codes and sample values only.
- For questions or corrections, open an issue or contact the document owner listed in the document header.
