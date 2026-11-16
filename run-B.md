# run-B — Validation Results

> Student B's independent review against the supplied SRS (v0.1 checklist). Answers are Yes, No, or N/A; `?` marks an uncertain answer. Student B should verify each answer against the SRS and enter their own actual times.

**Student:** ____________________  
**Date:** ____________________  
**Start time:** ____________________  
**End time:** ____________________

| ID | Item | Answer | Evidence | Where question came from |
|---|---|---|---|---|
| **CL-001** | Does each requirement contain only one “shall” or “may” statement? | No | R-07 combines “may cancel” with “shall update the doctor’s schedule and notify the receptionist”: a permission plus two system actions in one requirement. | Rule: Clear |
| **CL-002** | Is every requirement free of undefined vague words (e.g. “quickly”, “user-friendly”, “securely”, “normal”, “policy”)? | No | R-02 “quickly”, R-08 “user-friendly for all age groups”, R-09 “securely”, R-12 “normal working hours” and R-13 “clinic policy” are all used without definition. | Rule: Clear |
| **CL-003** | Does every speed or time requirement state a number and a unit? | No | R-02 gives no response time, R-06 says “before appointments” with no lead time, and R-12 gives no hours; only R-04 and R-05 state minutes. | Rule: Testable |
| **CL-004** | Could a pass/fail test be written for every requirement? | No | R-02, R-08, R-09, R-12 and R-13 have no measurable criterion, and R-04/R-05 conflict so the expected appointment length cannot be tested. | Rule: Testable |
| **CL-005** | Does the SRS define how simultaneous booking requests are handled? | No | R-03 only says “prevent double bookings”; it gives no rule for two requests for the same slot at the same moment (e.g. first-wins, slot locking, message to the loser). | Risk: Double bookings |
| **CL-006** | Does the SRS define a single consistent appointment-duration rule? | No | R-04 fixes every appointment at 15 minutes while R-05 lets doctors choose 10–30 minutes, so the two requirements contradict each other. | Contradiction: R-04 and R-05 |
| **CL-007** | Does the SRS state how long before an appointment reminders are sent? | No | R-06 says reminders are sent “before appointments” but gives no lead time (hours or days). | Risk: Forgotten appointments |
| **CL-008** | Does the SRS identify the channel used to send reminders? | No | R-06 does not say whether reminders go by SMS, email, phone call or app notification. | Completeness: R-06 |
| **CL-009** | Does the SRS define the conditions under which a patient may cancel an appointment? | No? | R-07 says only “at any time”, which is an unbounded permission rather than defined conditions: no cutoff before the slot, nothing on cancelling after the start time, and no link to R-13 overdue payments. Uncertain because “at any time” could be read as the intended condition. | Completeness: R-07 |
| **CL-010** | Does the SRS state which roles may view a patient’s medical records? | No | R-09 covers only storage of “patient records”; no requirement assigns view access to any of the five listed users, including the Data protection officer. | User: Data protection officer; Risk: Privacy |
| **CL-011** | Does the SRS specify security measures for protecting patient records? | No | R-09 says records are “stored securely” but names no measure (e.g. encryption, authentication, audit logging). | Risk: Medical information privacy |
| **CL-012** | Does the SRS provide a booking route for patients who cannot book online? | No? | R-01 covers online booking only, and R-10 is limited to “walk-in patients”; no requirement covers phone or assisted booking for patients unable to use the online route. Uncertain because walk-in booking by a receptionist may serve some of these patients. | User: Patient; Risk: Elderly patients |
| **CL-013** | Does the SRS define how emergency walk-in patients are handled? | No | R-10 lets receptionists book walk-ins but says nothing about emergencies, priority or referral. | Risk: Emergency walk-ins |
| **CL-014** | Does the SRS define the expected system capacity during busy periods? | No | No requirement states peak users or bookings; the context mentions only “about 400 patients per week”, and the closest requirement, R-02, is not quantified. | Risk: Monday-morning demand |
| **CL-015** | Does the SRS specify the exact days and hours when the system is available? | No | R-12 says only “during normal working hours” with no days, clock times or time zone. | Rule: Clear; R-12 |
| **CL-016** | Does the SRS identify the clinic policy used for overdue payments? | No | R-13 refers to “clinic policy” without stating or referencing the policy, and defines no overdue period or consequence. | Completeness: R-13 |
| **CL-017** | Does the SRS define how patients are informed that a booking was successful? | No | R-01 allows online booking but no requirement covers a confirmation; R-06 concerns reminders, not booking confirmation. | User: Patient; Completeness: R-01 |
| **CL-018** | Does the SRS define how doctors’ unavailable periods are handled? | No | R-14 only lets doctors view their daily schedule; no requirement covers leave or blocked time, or what happens to existing bookings. | User: Doctor; Completeness: R-14 |
| **CL-019** | Does the SRS define the appointment-booking permissions of receptionists? | No | R-10 covers only booking for walk-in patients; it does not say whether receptionists can book, change or cancel for other patients, or whether the R-11 limit of 3 active appointments applies to them. | User: Receptionist; R-10 |
| **CL-020** | Does the SRS define the functions available to the clinic administrator? | No | The administrator is listed under Users, but none of R-01 to R-14 mentions administrator functions. | User: Clinic administrator |
