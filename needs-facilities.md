# Visit-counter for a Facilities Manager

Scenario: Report visitor trends during a week of operation

  Given : Entry-card issuer type sensor,
  sensor differentiates among patients, relatives and visiting doctors.
  Separate counters maintained for different types of visitors.
  Reset counter everyday.
  
  When : asked for report.
  
  Then : Compute and present trends.

Scenario: Alert when seating capacity is full

  Given : Seating meant for visitors alone, entry-card issuer
  sensor type, visitors-exit log maintained. compute present
  count using entry and exit logs and check with maximum
  seat capacity. Maximum city capacity filled.
  
  When : every 15 minutes.
  
  Then : trigger an alert.
