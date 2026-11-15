# Requirements

In the requirements below, **the system** means the Clinic Management System (CMS), including the patient web page, the staff dashboard, and the machine learning waiting time module.

---

## B1. Functional Requirements

| ID | Requirement |
|---|---|
| FR1 | The system shall let a walk-in patient get a queue number by scanning a QR code at the clinic, without downloading an app. |
| FR2 | The system shall let a patient book an appointment online by choosing a service type and an available time slot. |
| FR3 | The system shall show the patient's current queue position on their phone and update it in real time. |
| FR4 | The system shall show a machine learning estimate of the waiting time on each queue ticket. |
| FR5 | The system shall send a push notification to the patient when three patients are ahead of them. |
| FR6 | The system shall use one ticket to track a patient through registration, consultation, and pharmacy in order. |
| FR7 | The system shall let authorised staff call the next patient and update the ticket status from a web dashboard. |
| FR8 | The system shall let patients cancel their queue number at any time before their turn. |

---

## B2. Non-Functional Requirements

| ID | Type | Requirement |
|---|---|---|
| NFR1 | Performance | The system shall update the queue position on the patient's screen within 5 seconds of a staff action. |
| NFR2 | Usability | A first-time patient shall complete check-in and receive a queue number in no more than 3 steps. |
| NFR3 | Security | The system shall use HTTPS for all connections and automatically log out staff after 15 minutes of no activity. |
| NFR4 | Privacy | The system shall ask the patient for consent before saving any personal data, following PDPA 2010 (Malaysia). |
| NFR5 | Accuracy | The machine learning waiting time estimate shall have a Mean Absolute Error (MAE) of 10 minutes or less when tested on clinic queue data. |

---

## Traceability

| User Story | Functional Requirement | Related Non-Functional Requirement |
|---|---|---|
| US1 | FR1 | NFR2 |
| US2 | FR4, FR5 | NFR1, NFR5 |
| US3 | FR7 | NFR3 |

The user stories are in [User-Stories.md](User-Stories.md).

---

## Planned Features Beyond the Current System

| # | Feature | Why it helps | Requirement |
|---|---|---|---|
| 1 | Real-time queue position on the patient's phone | Patient does not need to watch the display screen in the clinic | FR3 |
| 2 | Machine learning waiting time estimate | More accurate than a fixed average; supports the alert | FR4 |
| 3 | "Leave now" alert when 3 patients are ahead | Patient can wait outside; reduces crowding in the waiting room | FR5 |
| 4 | One ticket across registration, consultation, and pharmacy | No re-registration; smoother flow for the patient | FR6 |
| 5 | Staff dashboard to call next patient | Removes the need to call names aloud; easier for staff | FR7 |
| 6 | Cancel queue from phone | Reduces ghost queue numbers; keeps the estimate accurate | FR8 |
