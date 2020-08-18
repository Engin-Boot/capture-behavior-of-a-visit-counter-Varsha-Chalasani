# Visit-counter for a Director

Scenario: Show patient visits during working days and holidays

  Given: Entry-card issuer type sensor, works throughout the week,
  differentiates patients from relatives, visiting doctors
  
  When: Patient enters.
  
  Then : increments the patient-visit-counter. 

Scenario: Compute parking slots to reserve for visiting specialists

  Given : Entry-card issuer type sensor, we have a week's visit trends,
  visiting doctor's schedule.
  
  When : Before doctor visits.
  
  Then :  Computes average number of visits per day. Reserve parking lots.
