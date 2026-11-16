# Findings

The following issues are indicated by the checklist review of the supplied SRS. Confirm them during the pair’s comparison of the two independent runs.

| Finding | Related requirement(s) | Problem | Suggested clarification |
|---|---|---|---|
| F-01 | R-02 | “Quickly” is not measurable. | Set a response-time target and define the load conditions under which it applies. |
| F-02 | R-03 | Double-booking prevention is stated but not testably defined. | Specify the required behaviour for concurrent booking attempts and slot locking/confirmation. |
| F-03 | R-04, R-05 | Appointment duration is potentially contradictory: fixed at 15 minutes versus configurable from 10 to 30 minutes. | State whether 15 minutes is the default, a standard, or a restriction, and how doctor-specific durations work. |
| F-04 | R-06 | Reminder timing and delivery channel are missing. | Specify channel(s), timing, retry/failure behaviour, and any patient preferences. |
| F-05 | R-07 | “At any time” cancellation is broad and the effects are only partly described. | Define cancellation conditions, confirmation, and handling of near-start or missed appointments. |
| F-06 | R-09 | “Stored securely” is vague; access permissions and security controls are absent. | Define role-based access, authentication, protection, retention, and audit requirements. |
| F-07 | R-01, R-10 | Online booking and walk-in booking are covered, but an assisted route for patients unable to use online booking is not explicit. | Clarify whether receptionists can book on behalf of such patients and how this works. |
| F-08 | R-10 | Walk-in booking does not explain emergency handling or priority. | Define how emergency walk-ins are triaged or prioritised; identify any out-of-scope clinical decision. |
| F-09 | R-02, R-12 | Busy Monday-morning capacity and availability hours are not quantified. | Define expected peak demand, capacity/performance targets, and exact operating days/hours. |
| F-10 | R-13 | The referenced clinic policy is not included or identified. | Reference and make the applicable policy available, including the overdue-payment rules. |
| F-11 | R-01 | Booking confirmation behaviour is not specified. | Define the confirmation shown/sent to the patient and what happens if booking fails. |
| F-12 | R-14 | Doctors can view a daily schedule, but unavailable-doctor/leave handling is not specified. | Define how availability changes affect existing and future appointments. |
| F-13 | All / user roles | The administrator and data protection officer are listed as users, but their system capabilities are not described. | Specify the functions and permissions required for each role, including access review/audit needs. |

## Pair comparison record

Complete this section after Student A and Student B compare their independently completed runs.

- **Items where answers differed:** __________________________________
- **Items marked `?` and how they were resolved:** ____________________
- **Agreed final problems:** _________________________________________
- **Date/time of comparison:** _______________________________________
