# run-A — Validation Results

> Draft evidence for review against the supplied SRS. Student A and Student B must complete their reviews independently, verify the answers, mark uncertain items with `?`, and enter their own actual times.

**Student:** ____________________  
**Date:** ____________________  
**Start time:** ____________________  
**End time:** ____________________

| ID | Item | Answer | Evidence | Where question came from |
|---|---|---|---|---|
| **CL-001** | Does each requirement contain only one “shall” or “may” statement? | No | R-07 contains multiple actions: cancel appointments, update the doctor’s schedule, and notify the receptionist. | Rule: Clear |
| **CL-002** | Is every requirement free of undefined vague words (e.g. “quickly”, “user-friendly”, “securely”, “normal”, “policy”)? | No | R-02 uses “quickly”; R-08 uses “user-friendly”; R-09 uses “securely”; R-12 uses “normal working hours”; R-13 uses “as per clinic policy”. | Rule: Clear |
| **CL-003** | Does every speed or time requirement state a number and a unit? | No | R-02 gives no response-time number or unit; R-12 gives no specific working hours. | Rule: Testable |
| **CL-004** | Could a pass/fail test be written for every requirement? | No | Several requirements are not objectively testable as written, including R-02, R-08, R-09, R-12, and R-13. | Rule: Testable |
| **CL-005** | Does the SRS define how simultaneous booking requests are handled? | No | R-03 says the system shall prevent double bookings but does not describe behaviour when two users request the same slot simultaneously. | Risk: Double bookings |
| **CL-006** | Does the SRS define a single consistent appointment-duration rule? | No | R-04 fixes each appointment at 15 minutes, while R-05 lets doctors set appointment length from 10 to 30 minutes. | Contradiction: R-04 and R-05 |
| **CL-007** | Does the SRS state how long before an appointment reminders are sent? | No | R-06 says reminders are sent before appointments but does not specify how long before. | Risk: Forgotten appointments |
| **CL-008** | Does the SRS identify the channel used to send reminders? | No | R-06 does not identify whether reminders are sent by SMS, email, app notification, or another channel. | Completeness: R-06 |
| **CL-009** | Does the SRS define the conditions under which a patient may cancel an appointment? | No | R-07 says patients may cancel at any time but does not define any cancellation conditions or limits. | Completeness: R-07 |
| **CL-010** | Does the SRS state which roles may view a patient’s medical records? | No | R-09 says records are stored securely but does not identify which roles may view medical records. | User: Data protection officer; Risk: Privacy |
| **CL-011** | Does the SRS specify security measures for protecting patient records? | No | R-09 uses the word “securely” without specifying any security measures. | Risk: Medical information privacy |
| **CL-012** | Does the SRS provide a booking route for patients who cannot book online? | No | R-01 only describes online patient booking; no alternative assisted route for patients who cannot use it is stated. | User: Patient; Risk: Elderly patients |
| **CL-013** | Does the SRS define how emergency walk-in patients are handled? | No | R-10 allows receptionists to book walk-ins but does not explain how emergency walk-ins are handled or prioritised. | Risk: Emergency walk-ins |
| **CL-014** | Does the SRS define the expected system capacity during busy periods? | No | No requirement specifies the expected number of concurrent users, booking volume, or peak-period capacity. | Risk: Monday-morning demand |
| **CL-015** | Does the SRS specify the exact days and hours when the system is available? | No | R-12 says “normal working hours” but gives no days or clock times. | Rule: Clear; R-12 |
| **CL-016** | Does the SRS identify the clinic policy used for overdue payments? | No | R-13 refers to “clinic policy” without identifying or including that policy. | Completeness: R-13 |
| **CL-017** | Does the SRS define how patients are informed that a booking was successful? | No | R-01 requires online booking but does not say how a patient receives confirmation of a successful booking. | User: Patient; Completeness: R-01 |
| **CL-018** | Does the SRS define how doctors’ unavailable periods are handled? | No | No requirement explains how doctor leave or other unavailable periods affect appointment availability. | User: Doctor; Completeness: R-14 |
| **CL-019** | Does the SRS define the appointment-booking permissions of receptionists? | No | R-10 says receptionists can book walk-in appointments but does not define their broader booking permissions. | User: Receptionist; R-10 |
| **CL-020** | Does the SRS define the functions available to the clinic administrator? | No | The clinic administrator is listed as a user, but no requirement describes administrator functions. | User: Clinic administrator |
