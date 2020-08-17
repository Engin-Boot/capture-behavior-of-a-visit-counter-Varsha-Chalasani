# Visit-counter for a Director

Scenario: Show patient visits during working days and holidays

  Given: Entry-card issuer type sensor, works throughout the week,
  differentiates patients from relatives, visiting doctors
  When: Patient enters.
  Then : Sensor identifies as patient, , Issues a card specific to 
  the patient, increments the patient-visit-counter.

Scenario: Compute parking slots to reserve for visiting specialists

  Given : Entry-card issuer type sensor, differentiates visiting 
  doctors from relatives, patients
  When : Visiting doctor enters.
  Then : Sensor identifies as a visiting doctor, issues an entry card,
  increments visiting-doctor-counter. Computes average number of visits.
