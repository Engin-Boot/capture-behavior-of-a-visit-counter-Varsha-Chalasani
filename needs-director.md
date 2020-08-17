# Visit-counter for a Director

Scenario: Show patient visits during working days and holidays

  Given: Entry-card issuer type sensor, works throughout the week, entry-card issued to patients alone-not relatives, visiting doctors.
  When: Patient enters.
  Then : Sensor identifies patient,  Issues a card specific to the patient, increments the patient-visit-counter.

Scenario: Compute parking slots to reserve for visiting specialists

  Given :
  When
  Then
