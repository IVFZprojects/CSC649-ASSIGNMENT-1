# User Stories and Acceptance Criteria

Each story is linked to a requirement in [Requirement.md](Requirement.md).

---

## User Story 1 (linked to FR1 and FR3)

> As a patient, I want to scan a QR code at the clinic and get a queue number on my phone, so that I do not need a paper ticket or a separate app.

**Acceptance criteria**

1. Scanning the QR code opens the check-in page in a phone browser. No app download is needed.
2. After I enter my name and choose a service, my queue number and current position are shown on screen.
3. The queue position updates automatically when patients ahead of me are called.

---

## User Story 2 (linked to FR4 and FR5)

> As a patient, I want to see an estimated waiting time and get an alert before my turn, so that I can wait somewhere comfortable instead of sitting in the crowded clinic.

**Acceptance criteria**

1. My queue ticket shows an estimated waiting time that updates when the queue changes.
2. I receive a notification on my phone when three patients are ahead of me.
3. The notification arrives within 10 seconds of the queue change.

---

## User Story 3 (linked to FR7)

> As a clinic staff member, I want to call the next patient from one dashboard, so that I do not need to call names aloud or use a separate system for each stage.

**Acceptance criteria**

1. Pressing "Next" on the dashboard updates the patient's screen and moves the queue forward.
2. The dashboard shows the current status of each patient (waiting, in consultation, at pharmacy).
3. Only logged-in staff can access and use the dashboard.
