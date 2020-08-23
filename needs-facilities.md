# Visit-counter for a Facilities Manager

Scenario: Report visitor trends during a week of operation

  Given : Entry-card issuer type sensor
  And sensor differentiates among patients, relatives and visiting doctors
  And separate counters maintained for different types of visitors.
  And counter reset everyday.
  
  When : asked for report.
  
  Then : Compute and present trends.

Scenario: Alert when seating capacity is full

  Given : Seating meant for visitors alone
  And entry-card issuer sensor type
  And visitors-exit log maintained.
  And compute present count using entry and exit logs and
  check with maximum seat capacity.
  
  When : seat capacity filled
  
  Then : trigger an alert.
