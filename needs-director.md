# Visit-counter for a Director

Scenario: Show patient visits during working days and holidays

  Given: Entry-card issuer type sensor
  And works throughout the week
  And sensor counts patient visits
  
  When: director requests report
  
  Then : shows patient visits

Scenario: Compute parking slots to reserve for visiting specialists

  Given : Entry-card issuer type sensor
  And sufficient visiting trends of doctors
  
  When : Before doctor visits.
  
  Then : Reserve parking lots.
