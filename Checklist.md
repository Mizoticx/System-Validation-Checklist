# MediTrack Validation Checklist — v0.1

Use the SRS to answer each item. Write Yes, No, or N/A. **Yes must always be the good answer.** For each No, record the relevant requirement ID and a short reason in Evidence.

| ID | Item | Answer | Evidence | Where question came from |
|---|---|---|---|---|
| **CL-001** | Does each requirement contain only one “shall” or “may” statement? |  |  | Rule: Clear |
| **CL-002** | Is every requirement free of undefined vague words (e.g. “quickly”, “user-friendly”, “securely”, “normal”, “policy”)? |  |  | Rule: Clear |
| **CL-003** | Does every speed or time requirement state a number and a unit? |  |  | Rule: Testable |
| **CL-004** | Could a pass/fail test be written for every requirement? |  |  | Rule: Testable |
| **CL-005** | Does the SRS define how simultaneous booking requests are handled? |  |  | Risk: Double bookings |
| **CL-006** | Does the SRS define a single consistent appointment-duration rule? |  |  | Contradiction: R-04 and R-05 |
| **CL-007** | Does the SRS state how long before an appointment reminders are sent? |  |  | Risk: Forgotten appointments |
| **CL-008** | Does the SRS identify the channel used to send reminders? |  |  | Completeness: R-06 |
| **CL-009** | Does the SRS define the conditions under which a patient may cancel an appointment? |  |  | Completeness: R-07 |
| **CL-010** | Does the SRS state which roles may view a patient’s medical records? |  |  | User: Data protection officer; Risk: Privacy |
| **CL-011** | Does the SRS specify security measures for protecting patient records? |  |  | Risk: Medical information privacy |
| **CL-012** | Does the SRS provide a booking route for patients who cannot book online? |  |  | User: Patient; Risk: Elderly patients |
| **CL-013** | Does the SRS define how emergency walk-in patients are handled? |  |  | Risk: Emergency walk-ins |
| **CL-014** | Does the SRS define the expected system capacity during busy periods? |  |  | Risk: Monday-morning demand |
| **CL-015** | Does the SRS specify the exact days and hours when the system is available? |  |  | Rule: Clear; R-12 |
| **CL-016** | Does the SRS identify the clinic policy used for overdue payments? |  |  | Completeness: R-13 |
| **CL-017** | Does the SRS define how patients are informed that a booking was successful? |  |  | User: Patient; Completeness: R-01 |
| **CL-018** | Does the SRS define how doctors’ unavailable periods are handled? |  |  | User: Doctor; Completeness: R-14 |
| **CL-019** | Does the SRS define the appointment-booking permissions of receptionists? |  |  | User: Receptionist; R-10 |
| **CL-020** | Does the SRS define the functions available to the clinic administrator? |  |  | User: Clinic administrator |
