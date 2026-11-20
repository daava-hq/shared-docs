# shared-docs

Shareable Daava specifications and product documentation for reviewers.

---

## Documents

| Document | Covers |
| --- | --- |
| [`docs/dental-insurance-claims-specification.md`](./docs/dental-insurance-claims-specification.md) | End-to-end dental insurance and claims lifecycle — intake and coverage triage, EDI 270/271 eligibility, Open Dental write-back, clinical sign-off, AI CDT scrubbing, human-in-the-loop EDI 837D transmission, and STAX balance reconciliation. Includes a seven-phase Mermaid decision tree. |
| [`docs/addendum_i_dental_imaging_radiograph_integrations.md`](./docs/addendum_i_dental_imaging_radiograph_integrations.md) | Addendum I to the claims spec. Dental imaging and radiograph systems (Dexis, Carestream, Open Dental imaging, and others), and how claim attachments reach the clearinghouse. |
| [`docs/addendum_ii_clearinghouses_patient_payments_financing_tools.md`](./docs/addendum_ii_clearinghouses_patient_payments_financing_tools.md) | Addendum II to the claims spec. Clearinghouses (Vyne, DentalXChange, Stedi), patient payments and financing (STAX, Pearly, CareCredit, Cherry), and messaging status, with two-way SMS marked as planned. |
| [`docs/office-number-texting-report.md`](./docs/office-number-texting-report.md) | How Daava could text patients from each practice's own phone number, as Solutionreach does. Starts on a toll-free while each office number is reviewed, with a required fallback to the toll-free and then email. Includes vendors, setup steps, lead times, and open questions. |
| [`docs/sms-and-picture-messages.md`](./docs/sms-and-picture-messages.md) | SMS versus MMS. Short texts go as SMS, and images and long texts go as MMS on the same number. Covers two-way picture replies, which need Telnyx or Bandwidth, and what Solutionreach and other platforms publish about pictures. |

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
